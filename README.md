# Anchor Example: Escrow Program

#### Initialize

![image](https://github.com/user-attachments/assets/894a7821-28a6-4705-8ff2-3b1c46155f65)


`Initializer` can send a transaction to the escrow program to initialize the Vault. In this transaction, two new accounts: `Vault Authority's ATA` and `Escrow State`, will be created and tokens (Token A) to be exchanged will be transferred from `Initializer` to `Vault`(short for vault authority's ATA).

#### Cancel

![](https://hackmd.io/_uploads/ry0GNdKdo.png)

`Initializer` can also send a transaction to the escrow program to cancel the demand of escrow. The tokens will be transferred back to the `Initializer` and both `Vault` and `Escrow State` will be closed in this case.

#### Exchange

![](https://hackmd.io/_uploads/HkhNE_tdi.png)

`Taker` can send a transaction to the escrow to exchange Token B for Token A. First, tokens (Token B) will be transferred from `Taker` to `Initializer`. Afterward, the tokens (Token A) kept in the Vault will be transferred to `Taker`. Finally, both `Vault` and `Escrow State` will be closed.


