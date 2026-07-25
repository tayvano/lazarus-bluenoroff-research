# AFX

Date:: 2026-07-22

Amount Stolen:: $24,047,838

Tags:: 👛

G:: 561367

---

## Details

- https://x.com/AFX_XYZ/status/2080126901205770734

- https://x.com/blockaid_/status/2080080240265621680

- The malicious withdrawal was authorized by a quorum of hot-validator signatures and then finalized after the dispute period.

- Likely compromise or abuse of the bridge's hot-validator signing path. Five hot-validator signatures authorized a withdrawal of 24,150,000 USDC to the loot wallet, reaching 7,142 / 10,000 validator power (>2/3 quorum). The bridge contract then treated the withdrawal as valid and released funds after the 200-second dispute period.


## Onchain

### Victim / Compromised 

- 0xCb3B9A3E5668AFE84DC7A864B36b845dCE062e67 - Bridge contract
- 0x5553EA7Bda594aDE7AFe91D279779a42b2B84208 - Finalizer
- 0x32E3200D6E944cd9bD1C8C9865293B07206e7A01 - Withdrawal creation sender
- 0x00BB84aF06daC03BFe744Da13dF9D2D6fd8e77E5 - Validator
- 0x27259f90D6ae500262AcE6E8428434e0c1f308F5 - Validator
- 0x2e26dE22a92e41704B3eA00cc65a6CDA47b12c9e - Validator
- 0x52D4D9AD78a53a69bD089eE8f282CE0Cd0506Da7 - Validator
- 0xBB472BC3962Ad02Ac660429FdBB319B5BC66DA7b - Validator

### Attacker

- bc1q3ff9au48n4jzusxvj73tnuapgt9e6lredqwhkn - Funding
- 3GM3UZt1mUh7LetQzPDZZX7o3Q7g3TCYfv - Funding
- 0x32e3200d6e944cd9bd1c8c9865293b07206e7a01 - Funding
- 0x2f2974fAbc54dbA33442261211c06BD20E0FEefc - Attacker
- 0x627654b2782bfc57580ecd11d40869b350b6ebac - Holder
- Exploit tx: https://arbiscan.io/tx/0x50d0b3ec6c3f5fce0f10abf81540bbb508f421494aa2b3480c4a264b0436547b
- Withdrawal creation tx: https://arbiscan.io/tx/0x217c45c1272550e0439e53243f2987b7fb3f58b1d33c222597bbb71851b93f74
