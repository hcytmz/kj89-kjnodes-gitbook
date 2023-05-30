# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/osmosis.png" alt=""><figcaption></figcaption></figure>

Osmosis is a DEX protocol, which means it uses smart contracts  to determine the price of digital assets, to produce liquidity  via a peer-to-peer (P2P) methodology, and to exact trades between users

**Chain ID**: osmosis-1 | **Latest Version Tag**: v15.0.0 | **Wasm**: ON

[Website](https://osmosis.zone) | [Discord](https://discord.gg/osmosis) | [Twitter](https://twitter.com/osmosiszone)



Subscribe to our free [🤖 Mainnet Proposal Bot](https://t.me/kjnodes_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/osmosis](https://explorer.kjnodes.com/osmosis)

## Public endpoints

* api: [https://osmosis.api.kjnodes.com](https://osmosis.api.kjnodes.com)
* rpc: [https://osmosis.rpc.kjnodes.com](https://osmosis.rpc.kjnodes.com)
* grpc: osmosis.grpc.kjnodes.com:12990

## Peering

**state-sync**

```text
d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@osmosis.rpc.kjnodes.com:12956
```

**seed-node**

```text
400f3d9e30b69e78a7fb891f60d76fa3c73f0ecc@osmosis.rpc.kjnodes.com:12959
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/osmosis/addrbook.json > $HOME/.osmosisd/config/addrbook.json
```

**live-peers** (9)
```bash
peers="f96947493f1edd08058afaeaef8f5830cc70b8f2@15.204.197.10:26656,42f42a4b3527b927d5002d45abd37f66ecdd4861@51.178.74.75:16656,1c02ae0be21e3b08d9beadf91c26aec4193d2659@135.181.22.238:26656,c5358545d951ae666c695903036c1e93578951eb@135.181.176.113:26656,82e224c9640048a6513c589e904c0d903bb99f32@74.118.140.23:26656,2048e1bc1f020fa210fb475e7a0ec0948919609f@185.217.125.64:26656,ac2fbcb5de633d136a942c28c3049e3edbc6e69a@85.239.233.61:2000,406f64a8d601e34d7311fd61ec87b0c7028bd230@138.201.23.39:46656,6178f129efa76d235436e2156959d0acb4772c6a@65.108.128.168:36656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.osmosisd/config/config.toml
```
