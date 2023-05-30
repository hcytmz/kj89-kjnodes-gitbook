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

**live-peers** (10)
```bash
peers="5a09c55dbbb32b870645f56993e87403dfd17467@162.55.194.205:31656,54f5df8d6516ead7099191776d9ee2048e0ec947@95.214.53.46:26656,1e3f0aeb6f2a2017b122af2461a75c9695790954@65.108.233.109:10956,9876d1b1e5b5968c1c729559325dd909f93c1d34@65.108.238.61:56656,2c0379f78b655e8a386cb477e3cf3cae700c4a7f@213.239.207.175:34656,d92268c246e02a54103f7098b901b876c88f006e@5.161.130.108:26656,d5519e378247dfb61dfe90652d1fe3e2b3005a5b@65.109.68.190:13156,28fa150b5a843c9bdf2889f31f4ff8ac75c17be9@185.196.20.153:26656,52eee2c34150d621312087e49f118969472ba55f@149.102.137.192:26656,d7c9b9a3c3a6c5f4ccdfb37a8358755b277271c1@3.110.226.164:26656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.hid-node/config/config.toml
```
