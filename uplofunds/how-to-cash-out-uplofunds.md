# How to cash out UploFunds

As Uplo network usage increases, UploFunds will accrue UploCoins over time. [Learn more about UploFunds.](what-are-uplofunds.md)

If you're an UploFund owner, you have the option of cashing out these accrued UploCoins at any point by sending your UploFunds to an Uplo address you own. This can be the same wallet the UploFunds are currently in, or a different wallet you control.

{% hint style="info" %}
You **do not** lose the UploFunds in this process. You'll always retain control over them unless you send them to someone else or a bad address.
{% endhint %}

## How many UploCoins has my UploFund earned?

Uplo automatically keeps track of how many UploCoins your UploFunds have accrued, and we have an easy way to check that balance.

In any tab of Uplo-UI, click on the Terminal button at the top. It's the third button, and looks like a right-facing arrow in a box: `>`

![](../.gitbook/assets/coming-soon-01.png)

Type a single word command into the interface that pops up: `wallet`

![](../.gitbook/assets/coming-soon-01.png)

You'll be presented with a recap of your wallet: how many UploCoins you have, how many UploFunds you have, and how many UploCoins your UploFunds have earned, listed as `UploFund Claims`.

## Generate a Uplo address

Go to the Wallet tab of Uplo, and click **Receive.**

Click **Generate New Address** to create a new Uplo address.

![](../.gitbook/assets/coming-soon-01.png)

Copy and paste this manually, or use the `Copy` button to the right to make sure you get the full address without any extra spaces.

## Send your UploFunds to this address

Now switch over to the Send section of your wallet.

Enter the wallet address and the amount of UploFunds you want to send. Make sure that you've entered a Uplo wallet address you control, and that you've entered it correctly.

![](../.gitbook/assets/coming-soon-01.png)

{% hint style="danger" %}
UploFunds sent to mistyped addresses cannot be retrieved.
{% endhint %}

Click **Generate Transaction.**

## Verify your info

Next, you need to verify everything. You'll have a chance to double-check the currency, amount, and recipient address. Uplo-UI will also show you estimated network fees.

Click **Back** to change something. If it's all good, click **Broadcast.**

![](../.gitbook/assets/coming-soon-01.png)

## Check the status

You'll immediately get a confirmation.

![](../.gitbook/assets/coming-soon-01.png)

And you'll see a small tag appear under your balance to let you know the transaction is on its way but hasn't yet appeared in a block.

## For advanced users

If you're using uploc, the process is the same. Just initiate a transaction and send your UploFunds to a wallet address you control. You can use this command:

`uploc wallet send uplofunds <amount> <destination address (must be your own)>`

to take the accrued UploCoins and put them in your wallet. The UploFunds will still be on your wallet because you sent them to your own address.

