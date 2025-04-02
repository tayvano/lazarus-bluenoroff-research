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


### Onchain

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

### Misc Theft (DPRK) Addresses

- 0xcf49bc040f204eed8c5620b5ba325ad0a0cc811c
- 0xfd152bc1a8d47eb8f87700637c89ad0e7db47182
- 0xff7493efe724557ad99b4986d74af75c4f24750d
- 0xc51d1237dc91f4d844d69b80e1ed52a2612f3e05


### Initial Theft to Tornado - $1.5m
- 0x3e8c9490687dfc26c5621dd63ce9c3d415b405ed
- 0xa6dbd83666c141ae7965a813f5774b3791e1c8fe
- 0x418e337774d26365efeaa4700e889a9746330c4e
- 0x30cfbb9fb7dd6e41d7f2e421b7b08da101cd996f
- 0x1ce2502d49380bb09ac36caa8caea991331fb880
- 0x4bcc3a43e7469fea3fa29a903ce6c82b89cabaf6
- 0x6fa4658a587fec9aee83635a866326e43f13e11a
- 0x639f61ca3e0e3fdcd654dc4a22579e7382debea3 - deposits to Tornado May 22 2024
- TSMQQM9NMumDfZryQCtsKT5d5kgt7Ck2rm - leftvoers via Symbiosis


### Initial Theft to Railgun - $1m
- 0xb5fb14c1daa5d821b3049e2257dad723339a0238 - Withdraws from Lbank, Binance, etc.
- 0xb8132c207d0e6756fc70b043f26810c1dcb84422 - Withdraws from Lbank, Binance, etc.
- 0x1caf2a094b822674c7fd7ee0c2658051715aefe8 - Withdraws from Lbank, Binance, etc.
- 0x3663d3c0c442901614c21da835ac5b1841f17320 - Withdraws from Lbank, Binance, etc.
- 0x47da8f829feb4175cdcab942e1a9265d655718cc
- 0x948d92ddc99af3fc18f4f71c6e9961ff440ed55a - Consolidation
- 0xa41a6b3996a6cbb75fe2d7c67220d7012bb1487e - To Railgun May 22 2024
- 0xb125e60890db32596094e874500bfb9913bb4d37 - To Railgun May 23 2024
- 0xe2ebb51705a45221547dcc10b782801f1b62a95a - To Railgun May 24 2024


### June 2024: Swaps non-EVM stolen funds for ETH via Kraken, OKX, Kucoin, OrangeX, Gate, Bitget

- 0xcde108f9b138f52a8861d98418449cf3b96f39ea - Withdraws from CEXs
- 0xf8ae02565222756d040625081c42e556fa3d096c - Withdraws from CEXs
- 0x3b5fbd4f076a3084c68fc7a431095e3e1adbf52f - Withdraws from CEXs
- 0xb2ed78d4ca77a1068823ffb454df637590e85486 - Withdraws from CEXs
- 0x3508c159f5a418be49fda20a5893ddc6f9c87a3c - Withdraws from CEXs
- 0xcb5d4c4a7d0e9839184fd078ddef8e52b07be9f8 - Withdraws from CEXs
- 0x9f4f736faed111800a81c1af0bfcf4061c34aaf2 - Withdraws from CEXs
- 0x17151b77029b997c0858a50fd65a87744b548863 - Withdraws from CEXs
- 0x61947ff2e18aed20c3b28406ddb5ef2e06dd30bf - Withdraws from CEXs
- 0x92855956c7d970dd406fb372f681e814d53c8e4f - Withdraws from CEXs
- 0x91220970ebc3b414eb7e12c547ae49277989bd4a - Withdraws from CEXs
- 0xa1a3c94341dced86d210f5543309bdd98bfd6bf3 - Withdraws from CEXs
- 0xa9dbfea4e5da6715b653c72f5314b90da69ebe5b - Withdraws from CEXs
- 0xe8609b65db32dbc5934b170c1d6454b1f084a093 - Withdraws from CEXs
- 0x8c9fb01b09cf1811e7bef72b4b0398088399530a - Withdraws from CEXs
- 0x851c73e3b37fdc153be3f1b22c136234118de7b3 - Withdraws from CEXs
- 0x5793f4c46d974c120afab66ad229d43b2d7d36fe - Withdraws from CEXs
- 0xed260caf9394c7e0fd5a9285512ee82b0ca7df94 - Withdraws from CEXs
- 0x3b7c7f075c597ad2aa763526b32fbc285432dd73 - Withdraws from CEXs
- 0x9a5c14518f3954ffbdd074798ab598c641f4f9ca - Withdraws from CEXs
- 0xedafe3add817bacda196eb3f7e7e5191f841e05e - Withdraws from CEXs
- 0x482943c55d958474248aa0f6cdb22f0b84842675 - Withdraws from CEXs

- 0xc597682e15b9576f4f57be6837a8eb7a135abd99 - Consolidation, $3.7m
- 0x1bd8e2a7293b22b9e82de3727af49a8236f93323 - Consolidation, $4.1m
- 0x9906b7e5df58ca2038cb0e3818137af8986b39ea - Consolidation, Dust
- 0x5b70ef457f1ffcd5b1c9566725f23c23cb8c4ced - Consolidation, Dust

### Railgun June 13-16
- 0xc0a0ec4dbf170611cc76f31a9df910ad79bc2266 - To Railgun June 13-16 - $3.68m
- 0x5d393799a3c58d828dad1924e1db1d109ab6cf86 - From Railgun June 13-16 - $2m
- 0x9fc1350f80734044b7189fe7b8f288396f76feb5 - From Railgun June 16 - $1.06m
- 0x21c926a1a328a4906feeb18664d00f3d85df1aed - From Railgun June 16 - $600k
- 0xf4d64095a802524536834caf18702a80fedf0a52
- 0x305423ac2c50500c199994eae4c96a36a71f97a6
- 0x43f27789e0ddd7ff313f7a4750787e45949c7c76
- 0xb554e2adf27a133c416dee2f680f7b07da0d60c6
- 0x20f3a5a048832b95ea76c820c4e3584aeeaafdf6
- 0x631f635c23ea0ae23a26a32a65c8fb70b168a2a5
- 0xf60e4ac344bf57956adfa1535fb737d264a0c33d
- 0xcc9ad065ec8738d4bf78c88571aa115fb2655875
- 0x484f7fbab4058419ba682686530736ac47d26cf8
- 0x60d76296282ab4e8d97e9d7862af699df074efdb
- 0xe52375e2a2f79cfc65aff90686fe75b21f36fc7c
- 0xef0ed4012b8346cf7fce7470e37e2dcfceff9ac6
- TUqXnzfh174gM5XPaRtZdj8kv6UfkwLFZu
- TNVDV3E5cHpESwcvHzNoL5zajhPzNXiAxk
- TFgBXLa4hPiDUSBSdroxmmvN8Gojji5Eao
- TXA6mWjNYHcYyifwLva5ZvCpD95WhwEUTA
- TTDY6iKfzDuXUP4dyyaEjgmndpT5DwCXak
- TAQQabMqRXgEoWegtoFMHt3bumsk7828Fw
- TV1WokJauzJRJ2JorkUusbKL18fkCrmV3w
- TDDq4RsYze9vbdAd4JGG1j8y37e5SYdG5H

### Railgun June 27-19
- 0x1871bb6257b1f622548ef64a12ae5149eb208bd8 - To Railgun June 27-29 - $2.54m

### Railgun June 30-July 1
- 0xe381680d05057e20ac54978ddb3a345acc7bb42a - To Railgun June 30-July 1 - $1.55m
- 0xa20d83d25bcaacd5f8174b54367b9958ac02ee44 - From RG


### More from STX Laundry - Dec 18-20 2024 - $2,500,000

- $2,087,000 via Coinbase
- $168k via OKX
- $96k via Gate
- $81k via Kraken
- $42k via CoinW
- $21k via Whitebit

- SP3BYYEWFEAZX3A4HM0B9E0MAZFGHP62BVQ46MHMA From Initial Stolen Funds

- SPM0HTDM7G3JN3ETDH7W0F0STD4EHQ5268X4EF8C 1 Hop Tranches
- SP2Y56NCZT05CJX1GWFFYZ9KB0Z44GHE65461Z6NR 1 Hop Tranches
- SP2GZ3TPYCHYK7NH8JWKPG69X8ND9DFX9XNY4C3T2 1 Hop Tranches

- insert 4 more hops and hundreds of addresses here

- SP2EFY5Z69FH1WXSWDV1M8F6E4F1340TNTB5Z74NY Deposit Address (Coinbase)
- SP3M4AG92Q3FQWHYQPG98FVCRBT2X59JJFEGS1ED0 Deposit Address (Coinbase)
- SP276V832XBDG0Z9ECQ6RZ2TA25AB6WJY8GN12G7J Deposit Address (Coinbase)
- SP1A93SCBPWCTT9YQRRWV30H03309PD9NSY0NYSW2 Deposit Address (Coinbase)
- SP2N9DJA05H43CE946ZEKCM7CP6ME8MP9C49PYNMA Deposit Address (Coinbase)

- 0xae76ba497c211a7e1c33dadc8863c0b3e1210622 Withdrawal Addresses (Coinbase)
- 0xf5e80cedb44d2dcdf9ec76b4fa46daebeb1eb5ef Withdrawal Addresses (Coinbase)
- 0x1fe03a31338795d3249a8dc64b4faf944b1390db Withdrawal Addresses (Coinbase)
- 0x5e097095c8dbc1485f70e975d39ee3f84b5b99d8 Withdrawal Addresses (Coinbase)
- 0xec6ae1038a2f6822abd52b625508f44ed30948bd Withdrawal Addresses (Coinbase, Kraken, CoinW, OKX, FixedFloat)
- 0xaa92124c4805476f09b1445e72ee1d190f7eb34d Withdrawal Addresses (Coinbase)
- 0xec79fb56d8ca400e951778caa3d63babf2522109 Withdrawal Addresses (Coinbase)
- 0x54719ed916b80942660623c598ccf385143697bc Withdrawal Addresses (OKX)
- 0xdaf996a586eaf6d0fee5ce175683cb1d58c28fa2 Withdrawal Addresses (OKX, FixedFloat)
- 0x5b5b892b56e45c262bcb2f363cb173f0c8fc2e02 Withdrawal Addresses (Gate, FixedFloat)
- 0x12c4a5cc80624118170804b4c17c2d3f2968262a Withdrawal Addresses (Gate, FixedFloat)

- 0x48b886a7b6f5dcdaf1dd0f070126a946869f5334 Consolidation of the above

- TXxAihDJVezZ7s8tx8n9ysnMAvjCnrbq9K from Consolidation vs Allbridge
- TJcbNZZkzJgp6XcEbpEBx32TAuMkwuGZzL from Consolidation vs Allbridge
- TLsUeBvdy2NNJpxo83U7xtnYmSsFMFSVLz from Consolidation vs Allbridge

- Note: FixedFloats for gas from TLDEPVvBSjcQq2tc7HixdSkuE9F5kqW9hg, per usual







### Personal/Test Wallets

- 0x2bd8a5310f2b62aee6c1fde782a1bb02e23ef9c1 A
- 0x474ae2bedc010e746f26723c508a83ca09d18029 A
- 0x7ab0fad50169e05d6d688c832c9c9103216a94b4 A
- 0x76b30d808e98ab6f896c449d1a8f677231d40f0c A
- 0x5b70ef457f1ffcd5b1c9566725f23c23cb8c4ced A
- 0xc51d1237dc91f4d844d69b80e1ed52a2612f3e05 A
- 0x55adc85fb2ba51d045d09d0695b1ab88e5502334 A
- 0x736b2a990033b3138c484a86a333cf96131f2b0a A
- 0x47e12e7bc11abedd1e1cfe2bf8725ad6e2014974 A
- 0x5d90955cd3b04bdc48eb68ce3a9aac04132571f4 A - Receives from Oct 31, 2023  Swingby Skybridge user that goes to peelchain
- 0x4927f5848a85738210f08262fd04e568e0a34fab A
- 0x55adc85fb2ba51d045d09d0695b1ab88e5502334 A + W + Frax
- 0xc4562666d8e5c38cd46788e8b13e6edbcfadd10b W
- 0xe3d830249711b3f6f59297719f17e4b8d5bdc9a4 Zoth
- 0xc771d698673fb72e6e5e0599323b45c445d99eaa Zoth
- 0x54a34ac0cef536f791197cc7209dbba0bee916a8 Zoth
- 0x16b936e9be1d840198c57d9a3a4d70639bec474e Zoth

**0x47e12e7bc11abedd1e1cfe2bf8725ad6e2014974** is the personal wallet of one of the guys, clearly.


Nov 26 2023 withdraws 10x100 from TC:
- 0x1ac089a4135feed394a2985dadaed14994498f85
- 0x4509e930fd366bacd9e6cc64be4e706765046248

Dec 1 2023 sends $635k / Dec 3 2023 sends $1.48m and is immediately laundered:
- 0xd110a4f0a80b774eca0a6eac1552fff20dadd0a3
- 0x81a4869e941ca22d1a0ecff934abf87976d4578a

Dec 20 2023 + June 7 2024
- Key Compromiser 0x3e8c9490687dfc26c5621dd63ce9c3d415b405ed sends to 0xc51d1237dc91f4d844d69b80e1ed52a2612f3e05

Dec 15 2023 0x81a4869e941ca22d1a0ecff934abf87976d4578a sends leftover $1.7k to:
- 0x47e12e7bc11abedd1e1cfe2bf8725ad6e2014974


May 10, 2024 7:57:35 AM: ALEX Stuff

June 05 2024 + June 13 2024: Frax Transfer Froms
- 0x2b42614380a51e5e2bd9dbb8fd4724be53f063228fcb7d0300b195a6cb3b83cb
- 0x1b9f5ce14aea9752bcdd887e07b52bc1941e892d7bfdcf4b54a9b6274ec7cbbd
- From: 0x55ADc85fb2bA51D045d09D0695B1AB88E5502334
- TransferFrom: 0x736b2A990033B3138c484a86a333CF96131F2b0A
- To: 0x5d90955cD3B04bdc48EB68cE3a9AAC04132571f4

July 2024: Paying for something via Bybit, WazirX, Coingate, Cryptomus

June 3, 2024: sends to 0x5b70ef457f1ffcd5b1c9566725f23c23cb8c4ced
- 0x5b70ef457f1ffcd5b1c9566725f23c23cb8c4ced receives dust from 0x3b7c7f075c597ad2aa763526b32fbc285432dd73 on June 27 2024
- 0x3b7c7f075c597ad2aa763526b32fbc285432dd73 received launderd STX from Bitget on June 17 2024
- 0x3b7c7f075c597ad2aa763526b32fbc285432dd73 also sends to 0x4927f5848a85738210f08262fd04e568e0a34fab, which is another peronsal wallet 
- 0xc51d1237dc91f4d844d69b80e1ed52a2612f3e05 sends to 0x4927f5848a85738210f08262fd04e568e0a34fab
- 0x76b30d808e98ab6f896c449d1a8f677231d40f0c sends to 0x4927f5848a85738210f08262fd04e568e0a34fab

July 18 2024: Deploys Gnosis Safe
- 0x82715798af6f2194c615e2ad235ad5f6dced5315 





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
