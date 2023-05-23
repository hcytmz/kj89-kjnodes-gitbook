# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/paloma.png" alt=""><figcaption></figcaption></figure>

Paloma is a fast, permissionless, Cosmos-SDK blockchain that  moves messages securely, between any other blockchains.

**Chain ID**: messenger | **Latest Version Tag**: v1.0.0 | **Wasm**: ON

[Website](https://www.palomachain.com) | [Discord](https://discord.gg/tKVFpfdSw4) | [Twitter](https://twitter.com/paloma_chain)



Subscribe to our free [🤖 Mainnet Proposal Bot](https://t.me/kjnodes_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/paloma](https://explorer.kjnodes.com/paloma)

## Public endpoints

* api: [https://paloma.api.kjnodes.com](https://paloma.api.kjnodes.com)
* rpc: [https://paloma.rpc.kjnodes.com](https://paloma.rpc.kjnodes.com)
* grpc: paloma.grpc.kjnodes.com:11090

## Peering

**state-sync**

```text
d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@paloma.rpc.kjnodes.com:11056
```

**seed-node**

```text
400f3d9e30b69e78a7fb891f60d76fa3c73f0ecc@paloma.rpc.kjnodes.com:11059
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/paloma/addrbook.json > $HOME/.paloma/config/addrbook.json
```

**live-peers** (10)
```bash
peers="ab6875bd52d6493f39612eb5dff57ced1e3a5ad6@95.217.229.18:10656,7e93f6409ade895fe301b502d6fb9dfb96343a34@135.125.5.34:54056,9581fadb9a32f2af89d575bb0f2661b9bb216d41@46.4.23.108:26656,7eae755c119f538e0dc99f3c37289de628bc9526@209.182.239.169:26656,8af8dfa817359036f55f6793b0ed4bcce8884027@85.14.245.70:26656,2c6772b11c1f9eff2a923eb2bf808543cdd501c5@79.143.179.196:26656,d62eda97bc071f1b91106f484e0784928985f50e@207.180.196.234:26656,0bcc8119877ba0c701cd230e35c5477da2657bef@5.78.102.204:26656,d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@65.109.88.38:11056,dfa0d66a3713bf6b49bc509a2a4fc75bee042a30@23.88.77.188:20009"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.paloma/config/config.toml
```
