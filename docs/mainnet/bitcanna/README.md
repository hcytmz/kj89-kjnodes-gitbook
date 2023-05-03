# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/bitcanna.png" alt=""><figcaption></figcaption></figure>

BitCanna is a proof-of-stake (POS) decentralized payment network designed exclusively to serve the cannabis industry. 

**Chain ID**: bitcanna-1 | **Latest Version Tag**: v1.6.3 | **Wasm**: OFF

[Website](https://www.bitcanna.io) | [Discord](https://discord.gg/9AVrzaVQvs) | [Twitter](https://twitter.com/BitCannaGlobal)

[![Stake with kjnodes](https://i.ibb.co/cr44Q8j/button-stake-with-kjnodes.png)](https://restake.app/bitcanna/bcnavaloper1aym6s8eza7kjvnxuwxufrzccz6vqvgnsc47cc7)

Subscribe to our free [🤖 Mainnet Proposal Bot](https://t.me/kjnodes_proposal_bot) to never miss upcoming proposals

## Restake

[Restake with kjnodes](https://restake.app/bitcanna/bcnavaloper1aym6s8eza7kjvnxuwxufrzccz6vqvgnsc47cc7) (every 5 minutes)
## Chain explorer
[https://explorer.kjnodes.com/bitcanna](https://explorer.kjnodes.com/bitcanna)

## Public endpoints

* api: [https://bitcanna.api.kjnodes.com](https://bitcanna.api.kjnodes.com)
* rpc: [https://bitcanna.rpc.kjnodes.com](https://bitcanna.rpc.kjnodes.com)
* grpc: bitcanna.grpc.kjnodes.com:14290

## Peering

**state-sync**

```text
d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@bitcanna.rpc.kjnodes.com:14256
```

**seed-node**

```text
400f3d9e30b69e78a7fb891f60d76fa3c73f0ecc@bitcanna.rpc.kjnodes.com:14259
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/bitcanna/addrbook.json > $HOME/.bcna/config/addrbook.json
```

**live-peers** (10)
```bash
peers="88c6b1fa1c7fef98b4449b769eb2705476586664@65.109.92.241:21326,b15c0fade5fc0a354b4ac3fd9cdd8a716cddd24a@136.144.182.191:26656,d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@65.109.88.38:42656,07c829cf936db34be61143fabb09541d05aea899@65.108.98.124:64206,803fc66e3bd7b724921ef9c40636067f36e880c6@65.108.199.222:32656,65b12d58cc642eb8a1eb4e8344eaf26afce2e6d3@37.120.191.47:36656,dd4d3c0de38aa0575436c34c237b33bc0dda3ef2@142.132.158.93:13056,23671067d0fd40aec523290585c7d8e91034a771@65.108.43.170:26656,104d7ec9d84c8da66b97d50669b8ba58f1b60470@62.171.180.31:26656,d7322625044ad733bce4178dc397b2b9b5f68b41@43.153.27.130:26656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.bcna/config/config.toml
```
