# Using Uplo on multiple computers

Using Uplo on multiple computers can be an effective way to manage your Uplo life. You can have one instance of Uplo be your long-term UploCoin storage. While some users hold UploCoins, rent, and host under a single seed/single install, it's truly safest to have a separate seed and instance of Uplo for each use case.

## Using the same seed on multiple computers

In short, don't. Using the same Uplo seed on multiple computers can cause issues for your renter, host, and wallet balance.

In part, it comes down to address generation and syncing that data between the clients. It can cause your client to either not see or not catch in a timely manner the transactions that the other client is getting. Your wallet, renter, or host are not rescanning the blockchain before every transaction they make to ensure that the funding source wasn't already used.

Two wallets can become out of sync and show different balances, and new transactions could be denied by the blockchain.

When using multiple computers with Uplo, your best and safest bet is to have a different seed for each Uplo.

