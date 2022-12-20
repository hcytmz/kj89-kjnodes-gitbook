---
description: Prepare for and the upcomming chain upgrade using Cosmovisor.
---

# Upgrade

<figure><img src="https://raw.githubusercontent.com/kj89/testnet_manuals/main/pingpub/logos/${PROJECT_NAME}.png" width="150" alt=""><figcaption></figcaption></figure>

**Chain ID**: ${CHAIN_ID} | **Latest Binary Version**: ${LATEST_BINARY_VERSION} | **Custom Port**: ${CHAIN_PORT}

{% hint style='info' %}
Since we are using Cosmovisor, it makes it very easy to prepare for upcomming upgrade.
You just have to build new binaries and move it into cosmovisor upgrades directory.
{% endhint %}

## Download and build upgrade binaries

```bash
# Download project binaries
mkdir -p $HOME/${CHAIN_DIR}/cosmovisor/upgrades/${LATEST_VERSION_NAME}/bin
wget -O $HOME/${CHAIN_DIR}/cosmovisor/upgrades/${LATEST_VERSION_NAME}/bin/gravityd https://github.com/Gravity-Bridge/Gravity-Bridge/releases/download/${LATEST_BINARY_VERSION}/gravity-linux-amd64
wget -O $HOME/${CHAIN_DIR}/cosmovisor/upgrades/${LATEST_VERSION_NAME}/bin/gbt https://github.com/Gravity-Bridge/Gravity-Bridge/releases/download/${LATEST_BINARY_VERSION}/gbt
chmod +x $HOME/${CHAIN_DIR}/cosmovisor/upgrades/${LATEST_VERSION_NAME}/bin/*
```

*Thats it! Now when upgrade block height is reached, Cosmovisor will handle it automatically!*