# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/quicksilver.png" alt=""><figcaption></figcaption></figure>

Quicksilver is a permissionless, sovereign Cosmos SDK zone providing liquid staking for the entire Cosmos Ecosystem.

**Chain ID**: rhye-1 | **Latest Version Tag**: v1.4.2-rc7 | **Wasm**: OFF

[Website](https://quicksilver.zone) | [Discord](https://discord.gg/quicksilverprotocol) | [Twitter](https://twitter.com/quicksilverzone)



Subscribe to our free [🤖 Testnet Proposal Bot](https://t.me/kjnodes_testnet_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/quicksilver-testnet](https://explorer.kjnodes.com/quicksilver-testnet)

## Public endpoints

* api: [https://quicksilver-testnet.api.kjnodes.com](https://quicksilver-testnet.api.kjnodes.com)
* rpc: [https://quicksilver-testnet.rpc.kjnodes.com](https://quicksilver-testnet.rpc.kjnodes.com)
* grpc: quicksilver-testnet.grpc.kjnodes.com:11190

## Peering

**state-sync**

```text
d5519e378247dfb61dfe90652d1fe3e2b3005a5b@quicksilver-testnet.rpc.kjnodes.com:11156
```

**seed-node**

```text
3f472746f46493309650e5a033076689996c8881@quicksilver-testnet.rpc.kjnodes.com:11159
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/quicksilver-testnet/addrbook.json > $HOME/.quicksilverd/config/addrbook.json
```

**live-peers** (30)
```bash
peers="7283ce0d1cf4fd83fe826866a90b244d943fc434@38.242.248.195:11156,60509a87fc6c97a013de3cdeadf5fd3eab22f896@65.109.23.114:11156,e0f0703e9ce343c46e0ec01b19216715e817b358@65.109.85.170:26656,d5519e378247dfb61dfe90652d1fe3e2b3005a5b@65.109.68.190:11156,5c2a752c9b1952dbed075c56c600c3a79b58c395@95.214.55.232:27026,5a3c424c19d9ab694190a7805a2b1a146460d752@65.108.2.27:26656,c02431ff1a4fe66dca2d3c8ccbbd51b9977d8c54@88.208.57.200:11156,a2aa2a6db3b240fdd093f7d8214c1cc78e212995@65.108.237.232:31656,e6bf55bc9f08958b7518bea455423375db78d1ef@65.108.13.176:26656,e6bf4eca6a11035c06be529cb8c3758c2c00908f@213.170.135.20:26656,7142a4a19a87408ea6bcaf8bc2fd0265a5ccc7ad@162.55.245.219:11156,cc18d980216d658b76112fefd49cf2bf03d2d1cb@65.109.58.237:36589,5e83e140ae6a480ec8ac714fb71e0b509227cb9a@185.144.99.18:26656,6d3319970389d88f5deee9720a44fb95cad01ea2@185.144.99.96:26656,386d9eac66143c386d645b13eb9906caeb3cb33a@82.100.58.116:26656,4abe3e468eeb3a957d34efec57b01a4add92904e@185.16.39.51:26656,8b486ec6ee6167985f6eed69817f2a04bd70bba9@65.109.61.113:22217,80a09a8ae70e893789110c7945cb8f324002bfed@88.98.195.228:16656,0a3ac40a7a4ce35978c4da97be2eb6974bc3c58b@185.252.233.217:46656,c152888de058c1ca92e43913b502b137b8c17c26@195.201.243.40:26636,2a577a2f1a3c9e6fdcf19659af4ecc48f4525274@135.181.215.115:26776,676272662f2bba070a820aacc7ab7cec446526be@65.109.80.176:20656,3e484a1e5b0e019f1c227fb1481016161825c395@213.239.215.165:11156,ba65c74ac5f3c56b450348dea59b4d815220aeca@142.132.151.99:15651,1452d484454c0f93ddf3cbf987ce1b9cadd8f23f@65.21.95.180:37656,ec9d67f7c1103afcf097c0d9e11468c32f11f0c5@65.109.144.236:32656,fff84f665140e8072724246aad79702edcb1ad48@65.108.75.174:28656,6151346f98bc4bc81c94e587f96207e73cf701c7@185.16.38.122:15656,3519e61e653db97f5d1c7f1bec9b0072bca4d5fe@144.76.45.59:16656,8e14e58b054248a04be96e4a40d6359e93b636ac@65.108.65.94:26656"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.quicksilverd/config/config.toml
```
