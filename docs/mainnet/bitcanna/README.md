# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/bitcanna.png" width="150" alt=""><figcaption></figcaption></figure>

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
* grpc: bitcanna.grpc.kjnodes.com:42090

## Peering

**state-sync**

```text
d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@bitcanna.rpc.kjnodes.com:42656
```

**seed-node**

```text
400f3d9e30b69e78a7fb891f60d76fa3c73f0ecc@bitcanna.rpc.kjnodes.com:42659
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/bitcanna/addrbook.json > $HOME/.bcna/config/addrbook.json
```

**live-peers** (10)
```bash
peers="88c6b1fa1c7fef98b4449b769eb2705476586664@65.109.92.241:21326,8a210f1bcfc9015a7bc18dcc5add29c0dce3f2dc@135.181.173.65:26656,82588f011491c6100d922d133f52fc23460b9231@135.181.67.233:26656,dd4d3c0de38aa0575436c34c237b33bc0dda3ef2@142.132.158.93:13056,320d0d38559140608b72a361db44b2a8f14bf0d1@107.181.229.154:16656,89757803f40da51678451735445ad40d5b15e059@169.155.168.66:26656,7c00beb4956bc40cd33ced6e2c2ffe07d4fa32e7@95.216.242.82:36656,df99de6cec9152c517990317b340b8b9a307493c@193.34.144.156:26656,5af4f132d1c63cbe9d828d58522fdbb4bd508880@136.244.29.116:31656,d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@65.109.88.38:42656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.bcna/config/config.toml
```
