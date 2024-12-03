# ALEX Lab

Date:: May 15th, 2024

Amount Stolen:: $4,300,000

Tags:: 🔑 SquidSquad

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


### ALEX Lab Key Compromiser (DPRK)
- compromises the keys
- upgrades the contracts
- gets some money ($1.5m)
- from changenow
- stargate
- to tc eth (may 22)
- to railgun

### Theft (DPRK) Addresses

- 0xcf49bc040f204eed8c5620b5ba325ad0a0cc811c
- 0xfd152bc1a8d47eb8f87700637c89ad0e7db47182
- 0xe2ebb51705a45221547dcc10b782801f1b62a95a
- 0xb125e60890db32596094e874500bfb9913bb4d37
- 0xa41a6b3996a6cbb75fe2d7c67220d7012bb1487e
- 0xff7493efe724557ad99b4986d74af75c4f24750d
- 0x5b70ef457f1ffcd5b1c9566725f23c23cb8c4ced
- 0x9906b7e5df58ca2038cb0e3818137af8986b39ea
- 0xc597682e15b9576f4f57be6837a8eb7a135abd99
- 0xc0a0ec4dbf170611cc76f31a9df910ad79bc2266 - to railgun
- 0x3b5fbd4f076a3084c68fc7a431095e3e1adbf52f
- 0x3508c159f5a418be49fda20a5893ddc6f9c87a3c
- 0x61947ff2e18aed20c3b28406ddb5ef2e06dd30bf
- 0xf8ae02565222756d040625081c42e556fa3d096c
- 0xcb5d4c4a7d0e9839184fd078ddef8e52b07be9f8
- 0x1bd8e2a7293b22b9e82de3727af49a8236f93323
- 0x3e8c9490687dfc26c5621dd63ce9c3d415b405ed
- 0xc51d1237dc91f4d844d69b80e1ed52a2612f3e05
- 0x4bcc3a43e7469fea3fa29a903ce6c82b89cabaf6
- 0xa6dbd83666c141ae7965a813f5774b3791e1c8fe
- 0x418e337774d26365efeaa4700e889a9746330c4e
- 0x639f61ca3e0e3fdcd654dc4a22579e7382debea3
- 0x30cfbb9fb7dd6e41d7f2e421b7b08da101cd996f
- 0x6fa4658a587fec9aee83635a866326e43f13e11a
- 0x1ce2502d49380bb09ac36caa8caea991331fb880
- 0xe381680d05057e20ac54978ddb3a345acc7bb42a - to railgun
- 0x1871bb6257b1f622548ef64a12ae5149eb208bd8 - to railgun

### Withdraws from CEXs to Ehereum

- 0x3b7c7f075c597ad2aa763526b32fbc285432dd73
- 0xa1a3c94341dced86d210f5543309bdd98bfd6bf3
- 0xcde108f9b138f52a8861d98418449cf3b96f39ea
- 0xa9dbfea4e5da6715b653c72f5314b90da69ebe5b
- 0x92855956c7d970dd406fb372f681e814d53c8e4f
- 0xb2ed78d4ca77a1068823ffb454df637590e85486
- 0x17151b77029b997c0858a50fd65a87744b548863
- 0x9f4f736faed111800a81c1af0bfcf4061c34aaf2
- 0x91220970ebc3b414eb7e12c547ae49277989bd4a
- 0xedafe3add817bacda196eb3f7e7e5191f841e05e
- 0x482943c55d958474248aa0f6cdb22f0b84842675
- 0x8c9fb01b09cf1811e7bef72b4b0398088399530a
- 0xed260caf9394c7e0fd5a9285512ee82b0ca7df94
- 0x851c73e3b37fdc153be3f1b22c136234118de7b3
- 0x5793f4c46d974c120afab66ad229d43b2d7d36fe
- 0xe8609b65db32dbc5934b170c1d6454b1f084a093
- 0x9a5c14518f3954ffbdd074798ab598c641f4f9ca


## URLs

- https://twitter.com/ALEXLabBTC/status/1790611871986331855

- https://certik.com/resources/blog/alex

- https://twitter.com/ALEXLabBTC/status/1791020176332230988


## Connections

https://dailycoin.com/alex-lab-blames-north-koreas-lazarus-group-for-4m-exploit/

> Update on the ALEX Incident Investigation
> Dear ALEX Community,
> We wish to share an important update on the ALEX incident investigation from last month, which resulted in unauthorized access and the loss of funds. We understand the severity of this issue and are committed to full transparency in our ongoing response.
> **Potential Identification of the Attacker**
> After extensive forensic analysis and investigations facilitated by blockchain analyst [@Zachxbt](https://twitter.com/Zachxbt) who provided critical assistance on transaction tracing, there is substantial transaction evidence linking the attack to the Lazarus Group, a notorious hacker collective believed to be associated with the North Korean government.
> **Detailed Transaction Evidence**
> The following blockchain addresses and transactions were crucial in tracing the culprits and the flow of stolen assets:
> 1. Initial Exploit Link: Address 0x418e337774d26365efeaa4700e889a9746330c4e was directly linked to the
> XLink/ALEX Exploit. That address sent funds to 0x639F61cA3E0e3fDCd654DC4A22579e7382dEBeA3.
> 2. Connection to Lazarus Group: Address 0x639F61cA3E0e3fDCd654DC4A22579e7382dEBeA3 used a known Lazarus TRON address (TSMQQM9NMumDfZryQCtsKT5d5kgt7Ck2rm).
