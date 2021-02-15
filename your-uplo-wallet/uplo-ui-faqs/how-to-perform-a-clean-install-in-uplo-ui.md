# How to perform a clean install in Uplo-UI

Uplo-UI is great for storing UploCoins, uploading data to the Uplo network, or lending hard drive space for others to use.

It’s possible that you might have to perform a **clean install** of Uplo-UI if you run into a problem that can’t be solved by other means.

During a clean install, two primary things are deleted:

* The Uplo data folders
* The Uplo-UI application, in certain circumstances

But don’t worry, restoring your balance of UploCoins is easy as long as you have your original wallet seed.

{% hint style="warning" %}
Performing a clean install will remove all your renting and hosting info as well. So if you've uploaded data to Uplo or are hosting other's files, this will eliminate those contracts and should be used as a last resort. If you're not comfortable doing this, [contact support](mailto:hello@uplo.tech) or [visit our Discord](https://discord.gg/uplo) and we might be able to guide you through a specific fix.
{% endhint %}

## Your Uplo wallet seed

When you first generated your wallet, you were given [a 29-word seed](../the-importance-of-your-seed.md). This seed is the master key for your Uplo wallet and your UploCoin balance. Your UploCoins are always safe as long as you, and only you, have your seed.

The seed is required for this process, so make sure you have it handy. We’ll use it towards the end of the document.

If you don’t have your seed, do not proceed with these steps.

## Deleting the Uplo data folders

Uplo stores its data in specific folders. This includes things like the entire blockchain and your wallet info. We need to delete these, but first we need to find them. There are two easy ways to locate the folders.

{% hint style="warning" %}
**Note:** Quit Uplo before deleting the data folders.
{% endhint %}

**Navigate directly to the location below, depending on your OS.**

Windows: `%UserProfile%\AppData\Roaming\Uplo-UI\uplo`

Linux: `~/.config/Uplo-UI/uplo/`

Mac: `~/Library/Application Support/Uplo-UI/uplo/`

**or…**

**Use Uplo-UI**

If you've updated to v1.3.1 or later, you can easily find these folders by clicking **Show Uplo Data** in the About tab.

If you're on 1.4.0 or later, use the Info button at the top of Uplo.

![](../../.gitbook/assets/coming-soon-01.png)

Then click **Show Uplo Data.**

Once you find the `/uplo` folder:

![](../../.gitbook/assets/coming-soon-01.png)

Delete it.

Reboot your computer after deleting this folder.

## Deleting and re-downloading Uplo-UI

{% hint style="warning" %}
While not required, deleting and re-downloading the application files will ensure you are on the latest version. If you're sure you're already [on the latest version](https://uplo.tech/get-started), you can skip this step.
{% endhint %}

### **Prior to 1.4.0**

Uplo-UI installed where it was downloaded, unless moved. For Windows and Linux, you’ll see a folder that is named something like:

`Uplo-UI-v1.3.2-win32-x64`

On macOS, you’ll simply see the Uplo-UI icon.

Drag the folder containing the Uplo-UI app into the trash if you wish to.

### **1.4.0 and later**

On macOS, Uplo-UI can be found in the Applications folder. Trash it.

On Windows and Linux, you can run the uninstaller found with the Program file - `user/AppData/Local/Programs/Uplo-UI/` on Windows.

[Learn how to download and install Uplo-UI**.**](how-to-download-and-install-uplo-ui.md)\*\*\*\*

## Setting Uplo-UI up again

At this point, you’ve deleted the Uplo data folders and made sure you’re updated to the latest version of Uplo-UI. Now you’ll need to restore your seed to make sure your UploCoin balance is restored.

When you open Uplo-UI, choose **Restore from seed**. [Learn how to do that here](how-to-restore-a-wallet-from-a-seed-in-uplo-ui.md) if you need help.

Uplo-UI will then scan the blockchain for any UploCoin associated with your seed. This may take a while, but once it’s done your Wallet will show your previous UploCoin balance.

## Questions?

If you have any issues with this process, let us know! Send an email to [hello@uplo.tech](mailto:hello@uplo.tech) and we’ll get back to you as soon as we can.

