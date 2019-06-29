![](readme-images/shrek-sorry.jpg)

![](readme-images/typing.gif)

# Lightning Subscription Dashboard

This project is inspired by: https://github.com/genesisdotre/Bitcoin-Games-nLightning-Mind-Chrome-Extension

![](readme-images/activity.gif)

I was trying to find if there is a way of streaming payment, literally satoshis per second.

Question on StackOverflow: https://bitcoin.stackexchange.com/questions/88117/does-lightning-network-has-concept-of-continuous-stream-of-value

> Streaming payments is not part of the lightning network protocol yet.
> However you can build a lightning app that simulates exactly this.

> **I'm stealing this idea. Not exactly stealing because I feel partially responsible for thinking about it, just not being fully aware if this is already a part of the protocol**

<!-- 
RANDOM UNRELATED

https://twitter.com/skddc/status/946008107800584192
Been to 34c3, had a brief chance to say "hi" to @starkness and @peterktodd and  appreciate their work (they are public figures, they don't remember)
-->
![](readme-images/billboard.jpg)
# [CantBeEvil.com](https://cantbeevil.com/)

> build and support technology that can’t abuse users

You are in control of all your subscriptions.

Pay for the stuff you are actually using.

### Revolutionary, paradigm shapeshifting ⚡️️️⚡️️️⚡️️️
### Building blocks are here, conecting the `. . .`

It’s not Netlix and other companies keeping your billing details, credit card data.

It’s not service providers holding on to your upfront payments.

It’s not banks overcharging you, stacking hidden fees.

It’s you pushing payment to them.

You are in full control, they cannot run away with your money, they can’t be evil.


#### Using decent defaults

| | insurance | mobile plan | bike rental |
|---| --- | --- | --- |
| **OLD 🏦** | pay annual | pay monthly  | pay daily |
| **NEW ⚡️**| pay daily |  pay hourly | pay every minute |
| Default increment|  1 day |  1 hour |  1 minute
| Default prepayment|  1 week |  1 day |  15 minutes


#### Grace period

There should be some buffer, reservoire, grace period.

I don’t want to lose my subscription just because my node went offline.

> I pay for my internet, my internet is down, cannot SSH to my node and fix it. Catch-22, just like this outage by Google:  https://www.wired.com/story/google-cloud-outage-catch-22/

As my longevity (reputation, loyalty) as a customer increases the service provider can tweak the values.

Initially, as we operate in a trustless (hostile) environment, it will be a customer who should prepay for the initial duration of the service.

<!-- 
I think it should be voluntary. If my node stay online 24/7/365 then I do not have to prepay, otherwise its my voluntary decision to prepay for a day (have a buffer) and then do micropayments every 1000 sat.
-->

#### Assuming both nodes are online

For simplicity we can assume for nodes are online, if one of the nodes is offline cannot do much.

* If my node is online and their node is online then I can request the new invoice via REST API, get the invoice and pay it.
* If my node is offline, then cannot pay anyway.
* If their node is offline, then cannot pay anyway.


<!-- IT ALREADY EXIXTS
#### Positive sideeffects
It is possible that companies compeete not only on price, but conditions of the payment.

It is possible that you build a relationship with a company to receive better terms. Your loyalty literally pays of.

-->


#### Minimal treshhold payment

Fees on lightning network: unfairly cheap.

BUT… I ran into a feature, when I couldn’t  send `1 sat` because the fee was too high.

It was not possible to send `1 sat` and spend `1 sat` to send it.

I suggest we set the default for `1000 sat` which is `$0.09` at the current prices.







<!--
NODE LAUNCHER UNRELATED
I’m in love with Node Launcher.
https://medium.com/lightning-power-users/windows-macos-lightning-network-284bd5034340

It’s unfairly easy to run the full node.

At the same time, it's too cumbersome for me to set up everything from scratch. I don't even know how much SSD, memory, CPU for a VPS 
-->

# ARCHITECTURE


### Wannabe integrations
### Real-life use cases
### Receiving end 
Let's assume this project is completed and we have ability to stream payments on Lightning Network. But who will be the receiver on the other end?

**Bitrefill** - `13 June 2019` - https://www.coindesk.com/bitcoin-startup-bitrefill-raises-2-million-seed-round-for-worldwide-expansion

**OpenNode** - `19 Decemeber 2018` - https://bitcoinmagazine.com/articles/bitcoin-payment-processor-opennode-gets-125m-investors

<!-- NOTES ABOUT DEMO, SHOW DON'T TELL
To make a great looking demo, we will probably have to create some fictional businesses that can accept streming payments:

* Echelon mobile
* Webflix (Netflix)
* Perpetual Insurance
* Digital Sea (Digital Ocean)
-->

### Webhook callbacks

* Similar to PayPal: https://developer.paypal.com/docs/integration/direct/webhooks/event-names/#billing-plans-and-agreements

* `BILLING_AGREEMENTS.AGREEMENT.CANCELLED`

* If the subscription is cancelled (either explicitly or via lack of payment) the receiving node should inform the service provider.

### Blockstack login

* This is their competition, they are sponsoring the prizes.
* Placeholder submission: https://devpost.com/software/lightning-subscription-can-t-be-evil-streaming-payment
* For reasons outlined above we will usee Blockstack login and submit the completed product to app mining

![](readme-images/honeybadger.png)


# BONUS

### Full control, can't be evil?

So let's assume I rented a VPS and it's spinning CPU cycles... Is it really my own machine, my own node, how do I assure it's not backdored right from the start?

* The  question: https://security.stackexchange.com/questions/211243/what-are-the-techniques-to-know-if-vps-cloud-hosting-provider-is-accessing-my-da

* This is cool: https://canarytokens.org/generate



### Related projects ecosystem

Since I started working on this project, I've discovered the following:

* Joule Allowances - `13 June 2019`: https://twitter.com/wbobeirne/status/1139229792128180224

> This is ideal for apps that have small, frequent payments to access content (For instance, a video streaming platform that charges you for every minute of viewing time.)

* Sablier - `1 June 2019`: https://twitter.com/PaulRBerg/status/1134773451888238592

> It's a decentralised app for continuous payments. Up to you to decide what to use it for, but works best for paying salaries by the minute 💸

* ERC: Money Streaming - https://github.com/ethereum/EIPs/issues/1620

### Spontaneus payments (WIP)

Currently there is no “force push” to a trigger payment, need to have invoice first. 

Check this out: https://github.com/lightningnetwork/lnd/pull/2455

### Team

* Mars, [@marsXrobertson](https://twitter.com/marsXrobertson) on Twitter
* Dave

![](readme-images/goaway.png)