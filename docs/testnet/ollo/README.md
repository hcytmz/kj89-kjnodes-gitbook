# Services

<figure><img src="https://raw.githubusercontent.com/kj89/cosmos-images/main/logos/ollo.png" width="150" alt=""><figcaption></figcaption></figure>

OLLO is a sovereign L1 chain built on the Cosmos network providing  next-gen trading tools & sustainable tokenomics.

**Chain ID**: ollo-testnet-1 | **Latest Version Tag**: v0.0.1 | **Wasm**: OFF

[Website](https://www.ollostation.zone) | [Discord](https://discord.com/invite/GxBqZ9mSSm) | [Twitter](https://twitter.com/OLLOStation)



Subscribe to our free [🤖 Testnet Proposal Bot](https://t.me/kjnodes_testnet_proposal_bot) to never miss upcoming proposals


## Chain explorer
[https://explorer.kjnodes.com/ollo-testnet](https://explorer.kjnodes.com/ollo-testnet)

## Public endpoints

* api: [https://ollo-testnet.api.kjnodes.com](https://ollo-testnet.api.kjnodes.com)
* rpc: [https://ollo-testnet.rpc.kjnodes.com](https://ollo-testnet.rpc.kjnodes.com)
* grpc: ollo-testnet.grpc.kjnodes.com:32090

## Peering

**state-sync**

```text
d5519e378247dfb61dfe90652d1fe3e2b3005a5b@ollo-testnet.rpc.kjnodes.com:32656
```

**seed-node**

```text
3f472746f46493309650e5a033076689996c8881@ollo-testnet.rpc.kjnodes.com:32659
```

**addrbook**
```bash
curl -Ls https://snapshots.kjnodes.com/ollo-testnet/addrbook.json > $HOME/.ollo/config/addrbook.json
```

**live-peers** (28)
```bash
peers="d5519e378247dfb61dfe90652d1fe3e2b3005a5b@65.109.68.190:32656,742d7dccc98ccc2b30abb6ea172fc2175782db50@148.251.91.185:26656,e2d59891f1aed38fe8884c63e0bb00f8ddc41b6f@5.78.46.66:26656,2a8f0fada8b8b71b8154cf30ce44aebea1b5fe3d@162.19.238.122:26656,dba5e8b41c4e369418f83a449966e4eb7ca05cd4@65.109.23.114:18156,da8d3ca8e1c147f0037b1c43ad3de7174f5ec1b7@209.145.59.224:26656,5c2a752c9b1952dbed075c56c600c3a79b58c395@195.3.220.135:27006,4b73754c2c10d523ffd43ca95d9cb6e0ad8204a4@5.189.148.147:26656,29b78da822388df177f4111e6589958d9f796f06@65.109.122.105:60856,cba0eacc21eaddadc8903d503b1db12dd002fd0f@65.108.226.183:18156,69d2c02f413bea1376f5398646f0c2ce0f82d62e@141.94.73.93:26656,ab89596768849d679ed11a9e1848224760a278cc@83.171.248.175:32656,d6c5ff021b091a1fd93b9f811cf7fca0d31e8510@65.108.238.61:46656,9865c6e15faced6643adc228e3a59744e1b4e277@116.203.29.162:46656,e53eedfc4c5c4487e1fba7f3b97de6aadfca8cea@5.161.179.64:26656,70ba32724461c7ed4ec8d6ddc8b5e0b1cfb9e237@54.219.57.63:26656,cadc2b601a188aedbe4156a6eb5a81e00770bcfc@65.108.219.110:26656,3ea40f63890f10272201edf96d2a49e197e52091@65.108.105.48:18156,032845b1a798108bfc1fd91ebe5bdbbccd4a34d8@135.181.221.186:32656,0f99f7481a1b49701866ddbdfe71dc3b2fd792d8@109.123.244.56:26626,0bee9e500e51465917506b47691a8fb032100da9@94.130.200.168:32656,80b1ad27820f58b49e7a5a68881f0248a6269e9b@65.108.132.239:15656,15bcdea616c717eb4356e125d4f631aaa596dfd5@65.108.77.106:26929,a487497f2c80b53fa0908ce072a94a99be698b6b@142.132.162.28:46656,90ad9622ac54023fe4ee9824d77b5d3e3c25c245@162.55.234.70:54956,47655c33bdecae7f449301197d8b951a97e1b680@89.58.59.75:26656,4ee088d9c65f7c7dd6e5d5fe771543c647650457@194.163.163.224:26656,42beefd08b5f8580177d1506220db3a548090262@65.108.195.29:26116"
sed -i -e "s|^persistent_peers *=.*|persistent_peers = \"$peers\"|" $HOME/.ollo/config/config.toml
```
