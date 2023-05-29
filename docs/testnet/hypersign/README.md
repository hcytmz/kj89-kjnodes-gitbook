# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/hypersign.png" alt=""><figcaption></figcaption></figure>

Hypersign is a decentralized identity layer for the internet, giving  users control of their personal data and identity whilst digital  enabling trust for businesses.

**Chain ID**: jagrat | **Latest Version Tag**: v0.1.7 | **Wasm**: OFF

[Website](https://hypersign.id) | [Discord](https://discord.gg/DmuUjMrHVw) | [Twitter](https://twitter.com/hypersignchain)



Subscribe to our free [🤖 Testnet Proposal Bot](https://t.me/kjnodes_testnet_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/hypersign-testnet](https://explorer.kjnodes.com/hypersign-testnet)

## Public endpoints

* api: [https://hypersign-testnet.api.kjnodes.com](https://hypersign-testnet.api.kjnodes.com)
* rpc: [https://hypersign-testnet.rpc.kjnodes.com](https://hypersign-testnet.rpc.kjnodes.com)
* grpc: hypersign-testnet.grpc.kjnodes.com:13190

## Peering

**state-sync**

```text
d5519e378247dfb61dfe90652d1fe3e2b3005a5b@hypersign-testnet.rpc.kjnodes.com:13156
```

**seed-node**

```text
3f472746f46493309650e5a033076689996c8881@hypersign-testnet.rpc.kjnodes.com:13159
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/hypersign-testnet/addrbook.json > $HOME/.hid-node/config/addrbook.json
```

**live-peers** (11)
```bash
peers="934324c3b4318d8438954d19a82673a3d218951b@142.132.209.236:10956,54f5df8d6516ead7099191776d9ee2048e0ec947@95.214.53.46:26656,ec5127072c252f7246fb66f7e7762423a23ff6bd@154.12.228.93:31656,610843eda2f0388cb8e75917e8c1f63350bd3bd1@154.26.131.130:16656,28fa150b5a843c9bdf2889f31f4ff8ac75c17be9@185.196.20.153:26656,e8e764fa9ecc5727038099205798520c547d7019@51.178.65.184:25656,56615e02aa90e35a20a1fc4c46e78bb00956f07b@192.118.76.199:26681,0c6758a3f4554bbc67da73993bbb697764c5c534@38.242.142.227:26656,bd2ae9f1c42183104719f7c44be078bb7d282a61@65.109.92.241:11056,d7c9b9a3c3a6c5f4ccdfb37a8358755b277271c1@3.110.226.164:26656,d5519e378247dfb61dfe90652d1fe3e2b3005a5b@65.109.68.190:13156"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.hid-node/config/config.toml
```
