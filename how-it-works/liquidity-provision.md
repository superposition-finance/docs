# Liquidity Provision

Holders of Principal and/or Yield tokens can generate additional yield from these assets by staking them into the relevant vault AMM pool to provide liquidity.

To do so, users may visit the Vault's page, through which they will be able to deposit a set of Principal and/or Yield Tokens, along with a proportional amount of Underlying Asset tokens.

![](<../.gitbook/assets/App -- Pool.png>)

Our current (MVP-level) AMM design is based on the constant product market maker formula x \* y = k. We are developing, however, an improved market maker function which is enhanced to support the unique characteristics of tokens with time-decay (such as the Superposition Principal tokens).
