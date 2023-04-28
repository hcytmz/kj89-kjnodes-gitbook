# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/paloma.png" alt=""><figcaption></figcaption></figure>

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

**live-peers** (16)
```bash
peers="4569193b58dfc6d9ca9acd4e2bcabf596e5b6b3c@65.21.7.251:10656,317141e329bc214a76ba92201f6818574ebe5323@135.181.114.98:36656,31177b544fcf1cae76e3560812f4f901cab27126@65.109.61.175:26656,08c242d4505c5db223647069fdc0acb6e90079aa@65.109.106.214:26656,2c6772b11c1f9eff2a923eb2bf808543cdd501c5@79.143.179.196:26656,e833844c00b8ce60ce6826f170becfa18e6172c2@46.4.27.59:26656,16f0d09580054101394ea08bbb48b1ad5bb91a27@95.214.52.144:10656,cb8a1e9e12ac06dbd565311137f6c93d66fd96f8@104.167.221.18:26656,41a47bae18f81c1f626e4b238221b77e274424d7@45.33.65.223:26656,b92c94f00b46500a5ff8920acd438c0873c2f9da@50.116.13.101:26656,98b54cd6696e616fe966008ebf2bac409e3e0773@65.108.194.44:26656,87b4221770495e66e772a53bbea92a15aff288c2@144.126.158.0:26656,942951ad44b974098db48432455f135a653edbb1@65.21.230.230:31656,f4c43099e04b721c54a454dad85f61da49be90bc@65.108.199.222:28656,d73f7f6de427369a60245725047f49b1fd0e0a2f@65.108.199.26:31656,19165f3248f358ded53c3f51cf97a22123560b86@65.109.69.154:38656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.paloma/config/config.toml
```
