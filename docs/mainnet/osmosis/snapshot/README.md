# Snapshot

<figure><img src="https://raw.githubusercontent.com/kj89/testnet_manuals/main/pingpub/logos/osmosis.png" width="150" alt=""><figcaption></figcaption></figure>

{% hint style='info' %}
Snapshots allows a new node to join the network by recovering application state from a backup file. 
Snapshot contains compressed copy of chain data directory. To keep backup files as small as plausible, 
snapshot server is periodically beeing state-synced.
{% endhint %}

**pruning**: 100/0/19 | **indexer**: null | **version tag**: v12.2.0

| BLOCK             | AGE             | DOWNLOAD                                                                                            |
| ----------------- | --------------- | --------------------------------------------------------------------------------------------------- |
| 6826388 | 5 hours ago | [snapshot (26.34 GB)](https://snapshots.kjnodes.com/osmosis/snapshot\_latest.tar.lz4) |

## Instructions

### Stop the service and reset the data

```bash
sudo systemctl stop osmosisd
cp $HOME/.osmosisd/data/priv_validator_state.json $HOME/.osmosisd/priv_validator_state.json.backup
rm -rf $HOME/.osmosisd/data
```

### Download the latest snapshot

```bash
curl -L https://snapshots.kjnodes.com/osmosis/snapshot_latest.tar.lz4 | lz4 -dc - | tar -xf - -C $HOME/.osmosisd
mv $HOME/.osmosisd/priv_validator_state.json.backup $HOME/.osmosisd/data/priv_validator_state.json
```

### Restart the service and check the log

```bash
sudo systemctl start osmosisd && journalctl -u osmosisd -f --no-hostname -o cat
```