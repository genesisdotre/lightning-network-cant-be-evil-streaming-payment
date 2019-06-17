<span style="font-size:2.5em;">**L**ightning **S**ubscription **D**ashboar<span style="color:red">d</span></span>

![](readme-images/billboard.jpg)

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

# [cantbeevil.com](https://cantbeevil.com/)

> build and support technology that can’t abuse users

You are in control of all your subscriptions.

Pay for the stuff you are actually using

**REVOLUTIONARY, PARADIGM SHAPESHIFTING**
### Building blocks are here, conecting the . . .

It’s not Netlix and other companies keeping your billing details, credit card data.

It’s not service providers holding on to your upfront payments.

It’s not banks overcharging you, stacking hidden fees.

It’s you pushing payment to them.

You are in full control, they cannot run away with your money, they can’t be evil.


#### Example insurance

Currently: paying monthly.

Now you can pay every day, having more liquidity.

Contract day: 1 year
Default resolution: 1 day
Default prepayment length: 1 week


#### Example a mobile plan.

Currently: 1 month rolling contract.

Now you can pay daily.

Contract day: 1 month
Default increment: 1 hour
Default prepayment: 1 day

#### Example bike rental.

As obvious as it gets. No preauthorisation, no nothing, just PAYG (pay as you go)

Contract length: 6 hours
Default increment: 1 minute
Default prepayment: 15 minutes


### Sensinble defaults
### Buffer reservoire grace period

I don’t want to lose my subscription just because my node went offline.

I pay for my internet, my internet is down, cannot SSH to my node and fix it. Catch-22, just like this outage by Google:  https://www.wired.com/story/google-cloud-outage-catch-22/

There should be some tolerance / reservouire / buffer.

As my longevity as a customer increases, as valued customer, the service provider can tweak their values.

Initially, as we operate in a trustless (hostile) environment, it will be a customer who can prepay for the service, if they wish to.

I think it should be voluntary. If my node stay online 24/7/365 then I do not have to prepay, otherwise its my voluntary decision to prepay for a day (have a buffer) and then do micropayments every 1000 sat.


<!-- IT ALREADY EXIXTS
#### Positive sideeffects
It is possible that companies compeete not only on price, but conditions of the payment.

It is possible that you build a relationship with a company to receive better terms. Your loyalty literally pays of.

-->



### Minimal treshhold payment

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


### Would be partnerhips integrations
### Real-life use cases
### Receiving end 
Let's assume the project is not completed and now you have an ability to stream payments on Lightning Network. But who will be the receiver on the other end?

Bitrefill - `13 June 2019` - https://www.coindesk.com/bitcoin-startup-bitrefill-raises-2-million-seed-round-for-worldwide-expansion

OpenNode - `19 Decemeber 2018` - https://bitcoinmagazine.com/articles/bitcoin-payment-processor-opennode-gets-125m-investors

<!-- NOTES ABOUT DEMO, SHOW DON'T TELL
To make a great looking demo, we will probably have to create some fictional businesses that can accept streming payments:

* Echelon mobile
* Webflix (Netflix)
* Perpetual Insurance
* Digital Sea (Digital Ocean)
-->



#### Assuming both nodes are online
If my node is online and their node is online then I can request the new invoice via REST API, get the invoice and pay it.
If my node is offline, then cannot pay anyway.
If their node is offline, then cannot pay anyway.
That’s why for simplicity we can assume for nodes are online.

#### Webhook callbacks

PayPal equivalent

https://developer.paypal.com/docs/integration/direct/webhooks/event-names/#billing-plans-and-agreements

`BILLING_AGREEMENTS.AGREEMENT.CANCELLED`


### Spontaneus payments (WIP)


https://github.com/lightningnetwork/lnd/pull/2455

Currently there is no “force push” to a force it.

Currently the invoice has to be generated first and only then sent.






# BONUS

### Full control, can't be evil?

Ignorance is a bliss. So let's assume I rented a VPS *(AWS, Azure, Digital Ocean)* and it's spinning CPU cycles... Is it really my own machine, my own node, how do I assure it's not backdored right from the start?

* My question: https://security.stackexchange.com/questions/211243/what-are-the-techniques-to-know-if-vps-cloud-hosting-provider-is-accessing-my-da

* This is cool: https://canarytokens.org/generate



### Related projects ecosystem

Since I started working on this project, something interesting happened, check this out:

Joule Allowances - `13 June 2019`: https://twitter.com/wbobeirne/status/1139229792128180224

> This is ideal for apps that have small, frequent payments to access content (For instance, a video streaming platform that charges you for every minute of viewing time.)

Sablier - `1 June 2019`: https://twitter.com/PaulRBerg/status/1134773451888238592

> It's a decentralised app for continuous payments. Up to you to decide what to use it for, but works best for paying salaries by the minute 💸

https://github.com/ethereum/EIPs/issues/1620


### Join the team

* Dave JarvisTrade       
* Mars, marsXrobertson@gmail.com, [@marsXrobertson](https://twitter.com/marsXrobertson) on Twitter


![](readme-images/goaway.png)
