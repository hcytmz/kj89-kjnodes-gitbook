# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/paloma.png" width="150" alt=""><figcaption></figcaption></figure>

Paloma is a fast, permissionless, Cosmos-SDK blockchain that  moves messages securely, between any other blockchains.

**Chain ID**: messenger | **Latest Version Tag**: v0.11.6 | **Wasm**: ON

[Website](https://www.palomachain.com) | [Discord](https://discord.gg/tKVFpfdSw4) | [Twitter](https://twitter.com/paloma_chain)



Subscribe to our free [🤖 Mainnet Proposal Bot](https://t.me/kjnodes_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/paloma](https://explorer.kjnodes.com/paloma)

## Public endpoints

* api: [https://paloma.api.kjnodes.com](https://paloma.api.kjnodes.com)
* rpc: [https://paloma.rpc.kjnodes.com](https://paloma.rpc.kjnodes.com)
* grpc: paloma.grpc.kjnodes.com:10090

## Peering

**state-sync**

```text
d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@paloma.rpc.kjnodes.com:10656
```

**seed-node**

```text
400f3d9e30b69e78a7fb891f60d76fa3c73f0ecc@paloma.rpc.kjnodes.com:10659
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/paloma/addrbook.json > $HOME/.paloma/config/addrbook.json
```

**live-peers** (18)
```bash
peers="31177b544fcf1cae76e3560812f4f901cab27126@65.109.61.175:26656,15f4b11b50810b5046679a12b494e42a2c9034fd@65.109.30.12:26656,f4c43099e04b721c54a454dad85f61da49be90bc@65.108.199.222:28656,471a09da6fafb67bff3aa1f01e00fd1830e53262@136.243.94.138:26656,41a47bae18f81c1f626e4b238221b77e274424d7@45.33.65.223:26656,317141e329bc214a76ba92201f6818574ebe5323@135.181.114.98:36656,8ed8cddfac504d986a2c6545def0e57b2c6aa5db@65.109.106.172:38656,08c242d4505c5db223647069fdc0acb6e90079aa@65.109.106.214:26656,b92c94f00b46500a5ff8920acd438c0873c2f9da@50.116.13.101:26656,5321570794c61a8285505812cb7ebd6308a86583@65.109.113.253:26656,dfa0d66a3713bf6b49bc509a2a4fc75bee042a30@23.88.77.188:20009,45a3b59139f6db435c9a803c8f78eb2feda82c7c@135.181.144.214:26656,124cbe860f1eaa8084444587928db17c78ebd8f3@149.90.94.145:26658,8af8dfa817359036f55f6793b0ed4bcce8884027@85.14.245.70:26656,874ccf9df2e4c678a18a1fb45a1d3bb703f87fa0@65.109.172.249:26656,d73f7f6de427369a60245725047f49b1fd0e0a2f@65.108.199.26:31656,d9bfa29e0cf9c4ce0cc9c26d98e5d97228f93b0b@65.109.88.38:10656,ef1cd7da8319351b51ec930924929d03a5b76dc3@65.108.225.57:26656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.paloma/config/config.toml
```
