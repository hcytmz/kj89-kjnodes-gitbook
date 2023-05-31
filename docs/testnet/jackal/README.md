# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/jackal.png" alt=""><figcaption></figcaption></figure>

The Jackal Protocol is a fast, scalable, and secure blockchain that empowers  individuals, developers, and enterprises to increase their data privacy and  cybersecurity posture without sacrificing ease of use. This protocol strives  to offer world-class applications to protect the planet's most important data–your data.

**Chain ID**: lupulella-2 | **Latest Version Tag**: v2.0.1 | **Wasm**: ON

[Website](https://jackalprotocol.com) | [Discord](https://discord.com/invite/5GKym3p6rj) | [Twitter](https://twitter.com/Jackal_Protocol)



Subscribe to our free [🤖 Testnet Proposal Bot](https://t.me/kjnodes_testnet_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/jackal-testnet](https://explorer.kjnodes.com/jackal-testnet)

## Public endpoints

* api: [https://jackal-testnet.api.kjnodes.com](https://jackal-testnet.api.kjnodes.com)
* rpc: [https://jackal-testnet.rpc.kjnodes.com](https://jackal-testnet.rpc.kjnodes.com)
* grpc: jackal-testnet.grpc.kjnodes.com:13790

## Peering

**state-sync**

```text
d5519e378247dfb61dfe90652d1fe3e2b3005a5b@jackal-testnet.rpc.kjnodes.com:13756
```

**seed-node**

```text
3f472746f46493309650e5a033076689996c8881@jackal-testnet.rpc.kjnodes.com:13759
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/jackal-testnet/addrbook.json > $HOME/.canine/config/addrbook.json
```

**live-peers** (10)
```bash
peers="2ededbdbd98580e22ae8c3676e37b6e1fc1d987b@142.132.248.253:23656,3c6d856a429224201d78c7f28026874d10a27f57@5.75.227.78:26656,3aaeda343f226f9f2f00eeda53a20db438449c8c@89.58.45.204:46656,e4e93ce4b050c9d821e15b69477f5da706121343@65.109.93.152:31656,ec78732a7d5bdc1e27e8d7ac1bffe3881c9fb271@65.108.226.183:17556,712dd67b7abe08577d394e90a4930492c8f7d2ee@65.108.124.219:41656,27238e2f804bf28a14c186a2e0f0ceaae0d2588f@176.9.98.24:30566,a0f726a3dffb45d9cbde0913701bd757fcd7e434@157.90.2.254:36656,fabb22d283df1698de657c2bf4084892362136d6@38.242.237.107:26676,d5519e378247dfb61dfe90652d1fe3e2b3005a5b@65.109.68.190:13756"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.canine/config/config.toml
```
