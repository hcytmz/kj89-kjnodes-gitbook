---
description: Catch the latest block faster by using our daily snapshots.
---

# Snapshot

<figure><img src="https://raw.githubusercontent.com/kj89/testnet_manuals/main/pingpub/logos/quicksilver.png" width="150" alt=""><figcaption></figcaption></figure>

{% hint style='info' %}
Snapshots allows a new node to join the network by recovering application state from a backup file. 
Snapshot contains compressed copy of chain data directory. To keep backup files as small as plausible, 
snapshot server is periodically beeing state-synced.
{% endhint %}

Snapshots are taken automatically each day at **05:00 UTC**

**pruning**: 100/0/19 | **indexer**: null | **version tag**: v1.0.0

| BLOCK             | AGE             | DOWNLOAD                                                                                            |
| ----------------- | --------------- | --------------------------------------------------------------------------------------------------- |
| 39644 | 6 hours ago | [snapshot (1.18 GB)](https://snapshots.kjnodes.com/quicksilver/snapshot\_latest.tar.lz4) |

## Instructions

### Stop the service and reset the data

```bash
sudo systemctl stop quicksilverd
cp $HOME/.quicksilverd/data/priv_validator_state.json $HOME/.quicksilverd/priv_validator_state.json.backup
rm -rf $HOME/.quicksilverd/data
```

### Download latest snapshot

```bash
curl -L https://snapshots.kjnodes.com/quicksilver/snapshot_latest.tar.lz4 | lz4 -dc - | tar -xf - -C $HOME/.quicksilverd
mv $HOME/.quicksilverd/priv_validator_state.json.backup $HOME/.quicksilverd/data/priv_validator_state.json
```

### Restart the service and check the log

```bash
sudo systemctl start quicksilverd && journalctl -u quicksilverd -f --no-hostname -o cat
```