# How it works

Superposition works by taking a yield-generating asset (like an AMM LP token) and splitting its two economic components (principal and yield) into two separate tradable tokens: Principal Tokens and Yield Tokens. 

In practical terms, this is achieved by locking-up a yield-generating asset (e.g. a Saber or Raydium LP), into an escrow program and issuing a protocol-determined number of Principal and Yield tokens. At maturity, Principal Tokens can be redeemed 1-for-1 for the value of the underlying asset at time of minting, whereas Yield Tokens can be redeemed for the yield accrued by the underlying asset from the moment of minting through maturity.

#### Example

Let’s assume that a DeFi user wishes to provide $10,000 worth of liquidity on a Saber LP USDC-USDT pool over the course of 12 months. 

If he pursues that same strategy through a 12 month Superposition vault, he would receive 10,000 Principal Tokens redeemable for 10,000 USDC (or USDT) in a year, and 10,000 Yield Tokens redeemable for however much interest is generated on the relevant Saber pool over that year. If the average rate turned out to be 10%, then the Yield Tokens would have a terminal value of about 1,000 USDC (or 0.1 USDC per Interest Token).

![](<../.gitbook/assets/image (2).png>)

For a more detailed explanation of the functionality, you can visit the following pages:

{% content-ref url="minting.md" %}
[minting.md](minting.md)
{% endcontent-ref %}

{% content-ref url="swapping.md" %}
[swapping.md](swapping.md)
{% endcontent-ref %}

{% content-ref url="liquidity-provision.md" %}
[liquidity-provision.md](liquidity-provision.md)
{% endcontent-ref %}

{% content-ref url="burning.md" %}
[burning.md](burning.md)
{% endcontent-ref %}
