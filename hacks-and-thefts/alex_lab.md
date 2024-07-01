# ALEX Lab

Date:: May 15th, 2024

Amount Stolen:: $4,300,000

Tags:: 🔑

---


## Details

Bitcoin DeFi application ALEX Lab was drained of over $4.3 million in various tokens after a suspected private key compromise attacked its bridging service. 

Hackers transferred over $300,000 USD worth of BTC, $3.3 million USD worth of stablecoins, and $75,000 USD worth of Sugar Kingdom (SKO) tokens.

An attacker tried to pull off what could have been a ~$12 million heist from ALEX Lab's XLink bridge after a private key was compromised. However, the sloppy work by the attacker enabled an apparent whitehat hacker to step in.
The attacker was successfully able to transfer around 13.8 million STX (~$2 million) on the Stack BTC layer-2 chain. However, their attempts to steal assets notionally worth around $4.3 million from the project's BNB Chain implementation failed when they upgraded the project contract to a malicious version, but failed to prevent other people from calling the withdraw function. The attacker's first transactions to withdraw the funds themself failed, and an apparent whitehat hacker was able to step in and complete the withdrawal ahead of the exploiter. They later negotiated a deal for the funds' return, after offering a 10% "bounty".

The exploiter had also tried, and failed, to steal assets notionally worth around $5 million on the Ethereum blockchain, but failed to do so. ALEX Lab later announced they were able to recover or secure around $4.5 million of those assets.

On 14th May, CertiK’s internal alerting system detected a suspicious transfer of $4.3 million worth of assets to a wallet on the Binance Smart Chain, with an additional 13.7 million STX worth $2 million that was transferred to a malicious address. The incident was due to a private key compromise of the project’s deployer which has been confirmed by the project since the attack. The funds that were affected on BSC were front run by a wallet who has begun negotiations to return the assets to the project. At the time of writing, the funds affected total $6.3 million.


### On-chain
- 0xb3955302E58FFFdf2da247E999Cd9755f652b13b Victim Proxy Contract
- 0x3e8C9490687dFC26c5621dd63CE9C3d415b405ed Attacker
- SP2AS4QCQ81PJQ5HE3TJ6AJ554QX2YK14MFHT2VRS Attacker
- 0x27055aE433E9DCb30f6EbCC1A374Cf5CC03C484E Whitehat / Frontrunner


### ALEX Lab Safe Addresses
- 0x321f7d116f980fac4415262e50f674effd5ff58d
- 0xffda60ed91039dd4de20492934bc163e0f61e7f5 (msig)
- 0x457aafb91f9f3866b481a54eaab53056f788593e (binance depo)

### ALEX Lab Frontrunner
- actually gets the money (~$4.4m)
- keeps some money ($448k)
- sends rest back
- celer
- from tc bnb
- to tc eth (june 7)
- 0x27055ae433e9dcb30f6ebcc1a374cf5cc03c484e
- 0xbd86bf693d591004085121daab16e7192fcd3b01


### ALEX Lab Key Compromiser
- compromises the keys
- upgrades the contracts
- gets some money ($1.5m)
- from changenow
- stargate
- to tc eth (may 22)
- 0x3e8c9490687dfc26c5621dd63ce9c3d415b405ed
- 0x30cfbb9fb7dd6e41d7f2e421b7b08da101cd996f
- 0x418e337774d26365efeaa4700e889a9746330c4e
- 0x639f61ca3e0e3fdcd654dc4a22579e7382debea3


## URLs

- https://x.com/ALEXLabBTC/status/1790611871986331855

- https://www.certik.com/resources/blog/alex

- https://x.com/ALEXLabBTC/status/1791020176332230988


## Connections

https://dailycoin.com/alex-lab-blames-north-koreas-lazarus-group-for-4m-exploit/

> Update on the ALEX Incident Investigation
> Dear ALEX Community,
> We wish to share an important update on the ALEX incident investigation from last month, which resulted in unauthorized access and the loss of funds. We understand the severity of this issue and are committed to full transparency in our ongoing response.
> **Potential Identification of the Attacker**
> After extensive forensic analysis and investigations facilitated by blockchain analyst [@Zachxbt](https://x.com/Zachxbt) who provided critical assistance on transaction tracing, there is substantial transaction evidence linking the attack to the Lazarus Group, a notorious hacker collective believed to be associated with the North Korean government.
> **Detailed Transaction Evidence**
> The following blockchain addresses and transactions were crucial in tracing the culprits and the flow of stolen assets:
> 1. Initial Exploit Link: Address 0x418e337774d26365efeaa4700e889a9746330c4e was directly linked to the
> XLink/ALEX Exploit. That address sent funds to 0x639F61cA3E0e3fDCd654DC4A22579e7382dEBeA3.
> 2. Connection to Lazarus Group: Address 0x639F61cA3E0e3fDCd654DC4A22579e7382dEBeA3 used a known Lazarus TRON address (TSMQQM9NMumDfZryQCtsKT5d5kgt7Ck2rm).
