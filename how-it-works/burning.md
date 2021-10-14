# Burning

After a vault has reached maturity, the relevant outstanding Principal and Yield Tokens may be burned to unlock the original yield-generating assets which are locked in the vault.

The ratio at which Principal and Yield Tokens may be exchanged for yield-generating asset tokens is determined at vault maturity, through the following vault-wide formulas:

First we calculate the Total Locked Originating Protocol Reserves held by the vault

$$
Op = Originating Protocol
$$

$$
LockedOpReserves = LockedOpTokensCount \cdot \frac{TotalReservesInOp}{TotalOpTokens}
$$

Secondly we calculate the Principal Tokens Redeem Ratio

$$
PrincipalTokensRR = \frac{LockedOpTokensCount}{LockedOpReserves}
$$

Finally, we calculate the Yield Tokens Redeem Ratio

$$
YieldTokensRR = PrincipalTokensRR \cdot \frac{LockedOpReserves - TotalPrincipalTokensMinted}{TotalYieldTokensMinted}
$$

Once these ratios are computed (automatically at vault expiration), users may interact with the program in order to unlock the underlying yield-generating asset tokens. This is accomplished on the Vault's page. 

![](<../.gitbook/assets/App -- Pool-1.png>)
