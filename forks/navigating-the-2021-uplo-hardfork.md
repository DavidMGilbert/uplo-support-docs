# Navigating the 2021 Uplo hardfork

The Uplo network has implemented a hardfork to implement the Uplo Foundation: a new non-profit entity that builds and supports distributed cloud storage infrastructure, with a specific focus on the Uplo storage platform.

The hardfork occured around 4 pm ET on February 3rd. Track the fork with this [great tool](https://uplostats.info/fork) from SiaStats!

{% hint style="warning" %}
The hardfork requires v1.5.4 of Uplo. It is necessary to spend coins, receive coins, rent, or host after the fork. Every user, exchange, mining pool, wallet, and integration should upgrade as soon as possible.
{% endhint %}

This guide is strictly practical. If you'd like to learn more about the Foundation's proposal and the discussion that led to its acceptance, check these links.

[The Uplo Foundation proposal](https://www.reddit.com/r/uplocoin/comments/iox6ly/proposal_the_uplo_foundation/)

[Launching the Uplo Foundation](https://blog.uplo.tech/launching-the-uplo-foundation-ee47dfab4d2c)

[The Uplo forums](https://forum.uplo.tech)

You can reference our [Uplo API docs](https://uplo.tech/docs/) for technical documentation on Uplo and updating via CLI.

## Timeline

Uplo v1.5.4 has been released. The fork will be implemented at a block height of 298,000, which occurred on February 3rd at around 4 pm ET, 1 pm PT.

[Download 1.5.4 from our site](https://uplo.tech/get-started) \(best for most users\)

[Download 1.5.4 from Gitlab](https://github.com/uplo-tech/uplo/-/releases) \(if you prefer to build it yourself\)

## For renters and hosts

Renters and hosts need to [upgrade to v1.5.4](https://uplo.tech/get-started) by February 3rd.

Doing so ensures that renters will continue to upload data to hosts also on the new fork. Hosts who fail to upgrade in time will no longer form contracts with renters who upgrade. Long story short, you need to be on the same version as everyone else or you aren't part of the same network.

## For miners

Nothing will change. You can check in with your mining pool to make sure they've updated, but we've received confirmation from the following major pools that they will update: Luxor, SiaMining, f2pool, Dxpool.

## For exchanges

Exchanges should [upgrade to v1.5.4](https://uplo.tech/get-started) by February 1st at the latest. Due to the volume of users you serve, you should leave time for a proper upgrade. Once you do, your exchange will be able to support the fork once it takes effect.

{% hint style="warning" %}
Transactions created before the fork block but not confirmed yet will not be valid anymore after the fork block. We recommend that you pause withdrawals and don't send any transactions for the 6 hours leading up to the fork, and the 2 hours following the fork. This will prevent you from having your transactions become invalid.
{% endhint %}

Reference our [Uplo API docs](https://uplo.tech/docs/) if necessary. Updating your Uplo wallet can be as simple as running `uploc update`, or using the following API command, but only you know your Uplo wallet setup.

```text
curl -A "Uplo-Agent" -u "":<apipassword> "localhost:9980/daemon/update"
```

## For UploCoin holders

First, one important thing. You'll have the exact same amount of UploCoins after the fork.

### For users that store in our official wallet

UploCoin holders should [upgrade to v1.5.4](https://uplo.tech/get-started) by February 3rd. There are two versions of Uplo: Uplo-UI for most users, and uploc for advanced users. When the hardfork hits at block 298,000, your updated 1.5.4 version of Uplo will instantly give you access to the new chain, and all of your UploCoins will be available to you.

{% hint style="warning" %}
If you don't upgrade in time, you will brick your `consensus.db` file. This is the file that syncs the blockchain to your computer, and you will have to completely re-sync it. **You never lose your coins. Once you update to the new chain, your coins will be available to you again.**
{% endhint %}

[Learn how to download and install Uplo-UI](../your-uplo-wallet/uplo-ui-faqs/how-to-download-and-install-uplo-ui.md)

[Learn how to create a new wallet in Uplo-UI](../your-uplo-wallet/uplo-ui-faqs/how-to-make-a-new-wallet-in-uplo-ui.md)

[Download uploc from our site \(for advanced users\)](http://uplo.tech/get-started)

### For users that store UploCoins on an exchange

You don't have to do anything. When an exchange updates their wallet, you'll now have the same amount of coins on the new Uplo chain. These coins are usable to trade with exchanges once they have upgraded and to buy storage from hosts who also use the new chain.

## Exchange Support

Here's a list of all the exchanges that have had UploCoin volume over the past couple of months, according to CoinMarketCap. Please keep in mind that while we've confirmed with these exchanges that they are supporting the 1.5.4 Uplo fork, final implementation is up to their teams. You should reach out to your exchanges to confirm.

The second column will have three values:

* Informed, meaning we have passed the fork information along to the exchange
* Confirmed, meaning the exchange has agreed to update
* Complete, meaning the exchange has already updated

| Exchange | Updating to 1.5.4 |
| :--- | :--- |
| Binance | **Update Complete** |
| BiOne | Informed |
| Bittrex | **Update Complete** |
| CoinEx | **Update Complete** |
| Digifinex | Informed |
| HitBTC | Confirmed |
| Huobi Global | **Update Complete** |
| Kraken | **Update Complete** |
| Lbank | Confirmed |
| OKex | **Update Complete** |
| Poloniex | **Update Complete** |
| Upbit | **Update Complete** |
| VCC | Confirmed |

## For Ledger Nano S users

You'll need to update your app, but you should do it after the hardfork activates. Updating before the fork will your signatures won't be valid. Use [Ledger Live](https://github.com/DavidMGilbert/uplo-support-docs/tree/431ec4c4cb7b7fe1321203b069ebf4981995d762/uplo-integrations/using-the-uplo-ledger-nano-s-app.md#install_the_uplo_ledger_nano_s_app) in Developer mode to find and update the UploCoin app.

## For SiaStream users

SiaStream has been updated to support 1.5.4. If you run SiaStream, simply update to the [latest version](https://uplostream.tech) and you're all set once the fork hits.

## More questions?

Let us know! [Send us an email](mailto:hello@uplo.tech), or [reach out to the community on Discord](https://discord.gg/uplo).
