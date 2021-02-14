# Using the wrong chain after a fork

## How a fork works

When a blockchain hardforks, a new version of the blockchain is created while the old is left behind. This typically happens at a certain block height.

For example, [Uplo is forking](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/forks/navigating-the-2021-uplo-hardfork.md) around February 3rd, 2021. When Uplo forks, it will occur at block 298,000 and means that we now have a new chain that the Uplo team will be supporting. There's also the non-fork chain that can be maintained by a separate group if they want. Here's a visual representation of the upcoming Uplo fork.

![](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/.gitbook/assets/uplo-fork-path-2021.png)

## What this means for users

Frequently, after a fork, users of a blockchain don't update right away. This means that while the main network is operating on `version Y`, some users are still operating on `version X`. If you're on `version X` and try to send coins to an address that's using `version Y`, they won't go through.

The same is true for Uplo. If you have not updated to 1.5.4 or later, but send coins to someone who has updated, the transaction won't be received on the other end. It will look like those coins have disappeared.

Since all exchanges that trade UploCoin will update to 1.5.4 or later, sending coins to an exchange from a pre-1.5.4 wallet will result in the apparent loss of those coins.

## Your coins are safe

**You have not lost your coins.** At least, not your main network UploCoins. Since you were on the old chain when you sent them to a 1.5.4 wallet, you sent and lost your old chain coins – the coins that would have been spendable on forks of Uplo.

**Once you update to 1.5.4 or later, your coins will reappear.** Any coins held in your official Uplo wallet as of block 297,999, just before the hardfork, will be accessible in your wallet once you update Uplo and sync the new version of the blockchain.

[Download the latest version of Uplo now.](http://uplo.tech/get-started)

Now that you're updated, to sync the new version of the Uplo blockchain you first need to delete the old one. Quit Uplo.

If you're on 1.3.7 or earlier, you can easily find these folders by clicking **Show Uplo Data** in the About tab.

If you're on 1.4.0 or later, use the Info button at the top of Uplo.

![](../.gitbook/assets/fork-2%20%281%29%20%283%29.png)

Then click **Open Data Folder.**

Once you find the /uplo folder:

![](../.gitbook/assets/fork-3%20%281%29%20%282%29%20%281%29.png)

delete the `consensus` and `transactionpool` folders. Reopen Uplo to let it sync the correct version of the blockchain.

## Special considerations for miners

Some forks come with no changes to the mining algorithm for their network. In this case, like with the[ 2021 Uplo network hardfork](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/forks/navigating-the-2021-uplo-hardfork.md), you just need to make sure your mining pool upgrades in time \(they did\).

Miners might be affected in other ways by a fork. If you've set up your miner to mine a certain coin, a fork might change the algorithm associated with mining that coin. An example of this was the 2018 Uplo network hardfork, which invalidated all ASIC Uplo miners except those produced by Obelisk. If you were using a Bitmain A3, Innosilicon S11, or any other non-Obelisk ASIC miner, you were no longer mining the primary dev-supported Uplo chain after the fork.

What this meant for you was that your miner was still working, but it was mining the pre-fork version of UploCoin, usable only on pre-fork versions of the Uplo network. These coins that are mined were not visible in your wallet until you upgraded your node.

