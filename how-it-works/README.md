# How it works

At **Superposition** our goal has been to simplify principal/yield separation and provide an environment for exchanging of these new assets 

{% page-ref page="minting.md" %}

{% page-ref page="swapping.md" %}

{% page-ref page="liquidity-provision.md" %}

{% page-ref page="burning.md" %}









to be build on top of so the process is very straight forward, simply head over to one of our currently supported [minting pools](https://app.superposition.finance/app) and deposit your **LP Tokens**, in return you will receive a set of **Principal Tokens** and **Yield Tokens** that are redeemable for the value of your principal and yield accrued at the end of the term respectively.

{% hint style="info" %}
IMAGE HERE
{% endhint %}

In the backend, our protocol works alot like a decentralized escrow that unlocks at the minting pool's maturity. The \[word I cant recall here\] lies in our minting formula which adjust's the amount of **PTs** and **YTs** minted based on the time of minting and our burning formula which set the final _LP redeem ratios_ for **PTs** and **YTs**

#### **Principal Tokens Minting Formula**

The Principal Token is a proxy for the reserves inside the _Originating Protocol,_  for both fungibility and ease of market pricing.

$$
PT = OriginatingProtocolPoolReserves \cdot  \frac{UserLPT}{OriginatingProtocolTotalPoolLPT}
$$

#### Yield Tokens Minting Formula

Given the compounded growth of yield through a term, the YT formula  needs to calculate the portion of that yield that should be given to a minter based on his time of minting. 

Since the final rate of return is not know until the moment of expiration, we can only assume that it will be constant throughtout the lock-up term. _\(assumptions aren't always good, but this specific assumption should help participants determine the correct market value of YTs\)_

If we think of the total term return as a whole _\(the returns generated from term-start to term-end\)_ , the portion of that return that the minter should receive is not linear, that rate of decay can be expressed as the inverse of the compounded growth rate.   
The formula looks like this:

$$
YT = 2PT^{1-TimeLeftInTerm}
$$

_The **2** comes from the "100%" of the returns received at the end of the Term. The portion of that 100% of the returns received is based on the time left in the term at the time of minting._

## Burning



