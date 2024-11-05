---
description: >-
  Please carefully read this entire page to understand how transactions are
  sent. (This only applies to the CLI bot the Discord bot automatically routes
  shares through the official FT contract.)
---

# 🚨 Important

Before using the bot it is important to understand how shares are routed. The bot does not use the original friend.tech contract to send its buy and sell share transactions, instead it uses this friend.tech wrapper contract:&#x20;

[https://basescan.org/address/0xb1675320847917f6918c461e942e4be61388d8dd](https://basescan.org/address/0xb1675320847917f6918c461e942e4be61388d8dd)

What this allows us to do is send any amount of eth we want with our buy shares transactions and the wrapper will only use however much is necessary to purchase the specified number of shares and send back the rest to our wallet. \


<figure><img src=".gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

In this transaction for example the user sent .11 eth however only 0.0396 ETH was needed to purchase the share and the remaining 0.0704 ETH was sent back to the wallet. What this essentially means is that the more you send the more likely you are to successfully purchase the specified number of shares. While this makes it very easy to purchase shares without failing it is also a double edged sword as it could result in you paying more than you want. For that reason I recommend when you are telling the bot how much eth to send you treat it as the max amount of ETH you are willing to pay for a single share in the case of the copy trader, and per share in the case of the share buyer.&#x20;

Note:&#x20;

Because the bot uses a wrapper contract to send transactions buy and sells will not show up on the friend.tech feed essentially allowing you to anonymously copy trade without users knowing as well as buy and sell shares without users knowing.&#x20;

It is also important to note that any shares purchased through the bot AKA any shares bought through the wrapper contract must also be sold through the wrapper contract as they do not show up in your account. After every buy and sell the bot will send you the friend.tech link to the share address you have purchased and the transaction hash. If you lose the share address you can find it by going to the buy or sell transaction on Basescan, scrolling down to "Input Data", and pressing "Decode Input Data":

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>
