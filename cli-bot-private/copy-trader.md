# 🤖 Copy Trader

The copy trading feature will monitor a specified wallet for buy and sell share transactions. When a share is bought by the target wallet the bot will attempt to purchase a share. Likewise, when a share is sold by the target wallet the bot will attempt to sell a share. Below is a demonstration of using the copy trading feature:

First you will be prompted to enter the wallet address you would like to copy trade:

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

Next you will be prompted to enter the amount of eth to send per transaction. Be sure to read [important.md](../important.md "mention")to understand how transactions are routed and the amount in ETH you should send:

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

Finally you will be prompted to enter the max amount of buys the copy trader will make:

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

After this the copy trader will start monitoring the wallet for all transactions:

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Note:&#x20;

The copy trader does not allow you to choose the number of shares to buy per transaction and will by default only purchase a singular share. Once the max buy is reached the copy trader will continue to monitor for transactions it will just stop buying and only monitor for sells. If you wish to sell manually based on your own intuition (which I recommend) you can close the copy trader after it buys and use the share seller to sell instead.&#x20;
