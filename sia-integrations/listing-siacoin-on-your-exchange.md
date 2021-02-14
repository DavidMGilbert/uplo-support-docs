# Listing UploCoin on your exchange

Uplo is one of the best projects in the blockchain space. Uplo is open source, and we believe completely in the spirit of decentralization. As such, exchanges should strive to implement the best projects that will enhance their platforms with little involvement from the development team for that project.

## Some background on UploCoin

UploCoins are used for buying and selling storage space on the Uplo network. We believe that UploCoin is a pure utility token. UploCoins are generated only through Proof of Work mining, and there is no limit on the number of UploCoins that will be issued

## Download Uplo

UploCoins are stored in a Uplo wallet. Our two official apps are Uplo-UI or uploc \(for command-line interfaces\). Only one instance of Uplo can run at a time, so you’ll need to install it on multiple machines or virtual environments if you’d like to run more than a single wallet.

You can download the latest release [directly from Gitlab,](https://github.com/uplo-tech/uplo/tags) or [from our website](https://uplo.tech/get-started).

Learn how to download and install Uplo-UI.

## Technical Specifications for Uplo

* **CPU:** Uplo does not require special CPU considerations
* **RAM:** 8 GB recommended
* **SSD:** 40 GB recommended \(keep an eye on your consensus size!\)

As of January 2021, the blockchain is 24.25 GB, and you’ll need to download an entire copy to properly run your wallet. The blockchain grows by about 1 GB every two months.

No special libraries are required for installation.

## Review our API documentation

[Uplo API docs](https://uplo.tech/docs/)

## Setting up Uplo

This is where you come in. Every platform is different, and your team can determine how best to integrate the UploCoin wallet. While we don’t provide dedicated technical support, our developers can provide assistance with your issues. See the "[Point of contact](listing-uplocoin-on-your-exchange.md#point-of-contact)" section at the bottom of the article.

In the meantime, here are some answers to questions we’ve received regarding wallet setup for exchanges.

**IP Access Restriction.** IP access is restricted to localhost with user-agent "Uplo- Agent" required. We highly recommended keeping this as the default.

**User Access Restriction.** Our API documentation has information on how to set up password authentication to access the API.

**Transactions per block.** We recommend at most three multi-output transactions per block, and about 250 outputs per multi-output transaction.

**TLS/SSL Availability.** TLS/SSL is not currently available.

**Transaction Fee.** The transaction fee is automatically set, but you can always get an estimated range via the API [https://github.com/NebulousLabs/Uplo/blob/master/](https://github.com/NebulousLabs/Uplo/blob/master/) doc/API.md\#tpoolfee-get

**If the explorer returns incorrect info.** Instead of using the explorer, use the /consensus endpoints listed in the API documentation. These should get you the same info easily. We'll be working on the explorer soon.

## Common API Requests

**Generating wallet addresses**

[https://github.com/uplo-tech/uplo/blob/master/doc/API.md\#walletaddress-get](https://github.com/uplo-tech/uplo/blob/master/doc/API.md#walletaddress-get)

**Getting transactions for an address**

[https://github.com/uplo-tech/uplo/blob/master/doc/](https://github.com/uplo-tech/uplo/blob/master/doc/) API.md\#wallettransactionsaddr-get

**Sending to an address or set of addresses**

[https://github.com/uplo-tech/uplo/blob/master/doc/API.md\#walletuplocoins-post](https://github.com/uplo-tech/uplo/blob/master/doc/API.md#walletuplocoins-post)

**Unlocking the wallet**

[https://github.com/uplo-tech/uplo/blob/master/doc/API.md\#walletunlock-post](https://github.com/uplo-tech/uplo/blob/master/doc/API.md#walletunlock-post)

**Verifying an address**

[https://github.com/uplo-tech/uplo/blob/master/doc/](https://github.com/uplo-tech/uplo/blob/master/doc/) API.md\#walletverifyaddressaddr-get

**Changing the wallet password**

[https://github.com/uplo-tech/uplo/blob/master/doc/](https://github.com/uplo-tech/uplo/blob/master/doc/) API.md\#walletchangepassword—post

## A note about fees

We believe in the quality of our project, and the spirit of fair play. The long-term value proposition of listing any token comes, of course, from the transaction fees that an exchange earns. And these fees can add up to substantial amounts.

If your exchange requires any fee to list a coin, you can go ahead and skip us. We do not pay fees of any sort – whether they are called listing fees, marketing fees, sales budgets, etc.

## Community Votes

We don't participate in any type of community voting. Community votes typically come in two forms – those that are free and easy to manipulate or those that require paid votes and are still possible to manipulate. We'll never ask our community to participate in either in the future and urge all exchanges to add projects and tokens that they feel will benefit their users and the blockchain space.

## A legal opinion

If your exchange requires an opinion regarding UploCoin's status as it relates to US securities law, you can [download our team's self-written opinion.](https://files.helpdocs.io/YzA4Zq3JuM/articles/4ubdozs16r/1531331962488/uplo-legal-opinion-self-written.pdf) If your team requires an opinion from a US-based law firm, send an email to the point of contact listed below.

## Point of contact

If you have any questions, [send an email to Steve](mailto:steve@uplo.tech). He runs our support channels and will get you in contact with our dev team.

