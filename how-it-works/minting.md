# Minting

From a user’s perspective, the minting process is straightforward: they just deposit their _**yield-generating token **_into a **Superposition** [minting pool](https://app.superposition.finance/app). In exchange, they receive a set number of _**Principal and Yield tokens**_, which are redeemable at maturity for the value of the principal and accrued yield respectively

![](<../.gitbook/assets/App -- Mint.png>)

#### **Principal Tokens Minting Formula**

For both fungibility and ease of market pricing, the Principal Token is a proxy for the reserves inside the Originating Protocol:

$$
Op = OriginatingProtocol
$$

$$
PrincipalTokens = OpPoolReserves \cdot  \frac{UserOpTokens}{OpTotalPoolTokens}
$$

#### Yield Tokens Minting Formula

Given the compounded growth of yield through a term, the Yield Token formula  needs to calculate the portion of that yield that should be given to a minter based on his time of minting. 

Since the final rate of return is not know until the moment of expiration, we can only assume that it will be constant throughout the lock-up term. 

If we think of the total term return as a whole (the returns generated from term-start to term-end), the portion of that return that the minter should receive is not linear, that rate of decay can be expressed as the inverse of the compounded growth rate. Expressed by the following formula:

$$
YieldTokens = 2PrincipalTokens^{1-TimeLeftInTerm}
$$

_The 2 comes from the "100%" of the returns received at the end of the Term. _
