# Overview

### Why Yield Matters

Yield is the life force of DeFI. Protocols distribute yield to their active participants as compensation for providing fundamental services to the network. For example:

* **AMMs** like Saber and Raydium reward liquidity providers with trading fees
* **Credit marketplaces** like Solend reward lenders with interest
* **Tokenized proof-of-stake** systems like Marinade and Lido reward stakers with protocol dividends

DeFi yield is channeled through particular _**yield-generating tokens**_, such as “LP tokens”, which can be redeemed in the future for the initial deposit, plus any yield generated since then. They embody a fractionalized, decentralized share of yield-generating activity and as such serve as fundamental DeFi building blocks.

### The Problem with DeFi Yields

For all their worth, however, _**yield-generating tokens**_ also embed two unfavorable properties:

* **Interest rate volatility:** yield rates are driven by the market, as such they are variable and prone to volatility. Their final value is uncertain until they are redeemed
* **Capital inefficiency:** yield-generating deposits are locked until redeemed, which means they cannot be employed productively elsewhere

It is important to note that these drawbacks are not an accident — they’re a feature, rather than a bug. They originate from mechanisms that allow DeFi protocols to remain competitive and solvent, by responding to changes in market forces through the adjustment of interest rates. However, they also adversely affect a large swathe of users who are susceptible to uncertainty, risk and volatility.

### Our Solution: The Superposition Protocol

We have built **Superposition** to unshackle the potential of unrealized yield by mitigating these two fundamental drawbacks present in all _**yield-generating tokens**_. **Superposition** is a decentralized fixed-income protocol which allows users to tokenize, trade and monetize their future yield. It works by taking a _**yield-generating token**_, like a _Saber or Raydium LP_, and splitting it into two separate tradable tokens:

* _**Principal Tokens**_
* _**Yield Tokens**_

At maturity, _**Principal Tokens**_ can be redeemed 1-for-1 for the value of the _**yield-generating token**_ at time of minting, whereas _**Yield Tokens **_can be redeemed for the yield generated since then.

_This value is expressed as a portion of the locked LP Tokens._

![](<.gitbook/assets/image (5).png>)

Through our supporting AMM Pools, users can trade their _**Principal and Yield Tokens**_ in the open market, enabling a variety of [use cases](use-cases.md).
