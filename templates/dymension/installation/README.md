---
description: Setting up your validator node has never been so easy. Get your validator running in minutes by following step by step instructions.
---

# Installation

<figure><img src="https://raw.githubusercontent.com/kj89/testnet_manuals/main/pingpub/logos/dymension.png" width="150" alt=""><figcaption></figcaption></figure>

**Chain ID**: 35-C | **Latest Version Tag**: v0.2.0-beta | **Custom Port**: 46

### Setup validator name

{% hint style='info' %}
Replace **YOUR_MONIKER_GOES_HERE** with your validator name
{% endhint %}

```bash
MONIKER="YOUR_MONIKER_GOES_HERE"
```

### Install dependencies

#### Update system and install build tools

```bash
sudo apt -q update
sudo apt -qy install curl git jq lz4 build-essential
sudo apt -qy upgrade
```

#### Install Go

```bash
sudo rm -rf /usr/local/go
curl -Ls https://go.dev/dl/go1.19.5.linux-amd64.tar.gz | sudo tar -xzf - -C /usr/local
eval $(echo 'export PATH=$PATH:/usr/local/go/bin' | sudo tee /etc/profile.d/golang.sh)
eval $(echo 'export PATH=$PATH:$HOME/go/bin' | tee -a $HOME/.profile)
```

### Download and build binaries

```bash
# Clone project repository
cd $HOME
rm -rf dymension
git clone https://github.com/dymensionxyz/dymension.git
cd dymension
git checkout v0.2.0-beta

# Build binaries
make build

# Prepare binaries for Cosmovisor
mkdir -p $HOME/.dymension/cosmovisor/genesis/bin
mv bin/dymd $HOME/.dymension/cosmovisor/genesis/bin/
rm -rf build

# Create application symlinks
ln -s $HOME/.dymension/cosmovisor/genesis $HOME/.dymension/cosmovisor/current
sudo ln -s $HOME/.dymension/cosmovisor/current/bin/dymd /usr/local/bin/dymd
```

### Install Cosmovisor and create a service

```bash
# Download and install Cosmovisor
go install cosmossdk.io/tools/cosmovisor/cmd/cosmovisor@v1.4.0

# Create service
sudo tee /etc/systemd/system/dymd.service > /dev/null << EOF
[Unit]
Description=dymension-testnet node service
After=network-online.target

[Service]
User=$USER
ExecStart=$(which cosmovisor) run start
Restart=on-failure
RestartSec=10
LimitNOFILE=65535
Environment="DAEMON_HOME=$HOME/.dymension"
Environment="DAEMON_NAME=dymd"
Environment="UNSAFE_SKIP_BACKUP=true"

[Install]
WantedBy=multi-user.target
EOF
sudo systemctl daemon-reload
sudo systemctl enable dymd
```

### Initialize the node

```bash
# Set node configuration
dymd config chain-id 35-C
dymd config keyring-backend test
dymd config node tcp://localhost:46657

# Initialize the node
dymd init $MONIKER --chain-id 35-C

# Download genesis
curl -Ls https://raw.githubusercontent.com/dymensionxyz/testnets/main/dymension-hub/35-C/genesis.json > $HOME/.dymension/config/genesis.json

# Add seeds
sed -i -e "s|^seeds *=.*|seeds = \"c6cdcc7f8e1a33f864956a8201c304741411f219@3.214.163.125:26656 \"|" $HOME/.dymension/config/config.toml

# Set minimum gas price
sed -i -e "s|^minimum-gas-prices *=.*|minimum-gas-prices = \"0.025udym,0.025uatom\"|" $HOME/.dymension/config/app.toml

# Set pruning
sed -i \
  -e 's|^pruning *=.*|pruning = "custom"|' \
  -e 's|^pruning-keep-recent *=.*|pruning-keep-recent = "100"|' \
  -e 's|^pruning-keep-every *=.*|pruning-keep-every = "0"|' \
  -e 's|^pruning-interval *=.*|pruning-interval = "19"|' \
  $HOME/.dymension/config/app.toml

# Set custom ports
sed -i -e "s%^proxy_app = \"tcp://127.0.0.1:26658\"%proxy_app = \"tcp://127.0.0.1:46658\"%; s%^laddr = \"tcp://127.0.0.1:26657\"%laddr = \"tcp://127.0.0.1:46657\"%; s%^pprof_laddr = \"localhost:6060\"%pprof_laddr = \"localhost:46060\"%; s%^laddr = \"tcp://0.0.0.0:26656\"%laddr = \"tcp://0.0.0.0:46656\"%; s%^prometheus_listen_addr = \":26660\"%prometheus_listen_addr = \":46660\"%" $HOME/.dymension/config/config.toml
sed -i -e "s%^address = \"tcp://0.0.0.0:1317\"%address = \"tcp://0.0.0.0:46317\"%; s%^address = \":8080\"%address = \":46080\"%; s%^address = \"0.0.0.0:9090\"%address = \"0.0.0.0:46090\"%; s%^address = \"0.0.0.0:9091\"%address = \"0.0.0.0:46091\"%; s%^address = \"0.0.0.0:8545\"%address = \"0.0.0.0:46545\"%; s%^ws-address = \"0.0.0.0:8546\"%ws-address = \"0.0.0.0:46546\"%" $HOME/.dymension/config/app.toml
```

### Start service and check the logs

```bash
sudo systemctl start dymd && sudo journalctl -u dymd -f --no-hostname -o cat
```