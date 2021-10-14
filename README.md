# Overview

### Why Yield Matters

Yield is the life force of DeFI. Protocols distribute yield to their active participants as compensation for providing fundamental services to the network. For example:

* **AMMs** like Saber and Raydium reward liquidity providers with trading fees
* **Credit marketplaces** like Solend reward lenders with interest
* **Tokenized proof-of-stake** systems like Marinade and Lido reward stakers with protocol dividends

DeFi yield is channeled through particular yield-generating assets, such as “LP tokens”, which can be redeemed in the future for the initial deposit, plus any yield generated since then. They embody a fractionalized, decentralized share of yield-generating activity and as such serve as fundamental DeFi building blocks.

### The Problem with DeFi Yields

For all their worth, however, yield-generating assets also embed two unfavorable properties:

* **Interest rate volatility:** yield rates are driven by the market, as such they are variable and prone to volatility. Their final value is uncertain until they are redeemed
* **Capital inefficiency:** yield-generating deposits are locked until redeemed, which means they cannot be employed productively elsewhere

It is important to note that these drawbacks are not an accident — they’re a feature, rather than a bug. They originate from mechanisms that allow DeFi protocols to remain competitive and solvent, by responding to changes in market forces through the adjustment of interest rates. However, they also adversely affect a large swathe of users who are susceptible to uncertainty, risk and volatility.

### Our Solution: The Superposition Protocol

We have built Superposition to unshackle the potential of unrealized yield by mitigating these two fundamental drawbacks present in all yield-generating assets. Superposition is a decentralized fixed-income protocol which allows users to tokenize, trade and monetize their future yield. It works by taking a yield-generating token, like a Saber or Raydium LP, and splitting it into two separate tradable tokens:

* Principal Tokens
* Yield Tokens

At maturity, Principal Tokens can be redeemed 1-for-1 for the value of the yield-generating asset at time of minting, whereas Yield Tokens can be redeemed for the yield generated since then.

_This value is expressed as a portion of the locked LP Tokens._

![](<.gitbook/assets/image (5).png>)

Through our supporting AMM Pools, users can trade their Principal and Yield Tokens in the open market, enabling a variety of [use cases](use-cases.md).
