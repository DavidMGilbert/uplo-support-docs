---
description: ...and now you have to resync your Uplo wallet.
---

# So, you didn't update in time for the fork

![](../.gitbook/assets/cap.jpg)

On February 3rd, 2021 at block 298,000, [the Uplo network hardforked](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/forks/navigating-the-2021-uplo-hardfork.md) to implement the Uplo Foundation: a new non-profit entity that builds and supports distributed cloud storage infrastructure, with a specific focus on the Uplo storage platform.

It's a great thing! But here you are, and you didn't update in time. Maybe you never even updated from the 2018 fork! You can't rent storage space, host, or send SC to friends or exchanges. For most people who updated ahead of time, it was a simple matter of [downloading the latest version and installing it](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/your-uplo-wallet/uplo-ui-faqs/how-to-download-and-install-uplo-ui.md).

Not you though, something went \(or is going\) wrong. It might be that:

* Uplo is not syncing
* Uplo is not forming contracts
* Your transactions are not broadcasting
* Your transactions are broadcasting, but are not being received at your destination
* Uplo says you are not up to date
* Uplo says you are up to date, but you know you're not \(sometimes happens with very old versions when checking via the uploc `update` command\)

Many of these issues can manifest when you're [on the wrong chain](using-the-wrong-chain-after-a-fork.md).

## How to resync

You're on the wrong Uplo chain if you're not on 1.5.4. Type `./uploc version` in your CLI, or use the ⓘ in the top nav bar of Uplo-UI to check.

The most effective way to resync is to perform a clean install. The process requires:

* your Uplo seed
* deleting the Uplo data folders
* deleting and re-downloading Uplo
* setting Uplo up again

It's a bit of a long process, mostly because Uplo will re-download the consensus blockchain file. But resyncing is something you'll need to do anyway, and a clean install works 100% of the time. Use [this guide](https://github.com/DavidMGilbert/uplo-support-docs/tree/7d49a88dcb3b035d374d7df410f395a22d2df2d1/your-uplo-wallet/uplo-ui-faqs/how-to-perform-a-clean-install-in-uplo-ui.md) for a detailed walkthrough of these steps.

