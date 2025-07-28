# Thorswap Admin Theft

Tags:: 💼 DPRK IT?

---

The only really details come from this article, copy and pasted below: https://thorswap.medium.com/thorswap-disclosure-15aa228db147


# Important THORSwap Disclosure

In late Summer of 2022, the founder of THORSwap, known to most as THORSwap Admin (aka “TSA”), departed the project. At that time, control of THORSwap treasury assets and administrative functions were transitioned to a series of multi-sig wallets controlled by a group of THORSwap contributors.

After assets were transferred to the contributor-controlled multi-sig wallets, we undertook a full review of the activity around project assets, both current and historical. Our audit revealed a number of unexplained activities in the months preceding TSA’s departure.

Our analysis indicates that TSA transferred a total of roughly 6 million THOR tokens and 200 thousand RUNE tokens from THORSwap’s Treasury & Contributor wallets into what appear to be personal wallets controlled by himself. These activities, which we’ve detailed below, were not disclosed to other contributors.

At the time of TSA’s departure, he personally revoked his own vesting schedule and notified the remaining contributors as well as investors that he had done so. TSA’s vesting schedule was for a total of 25m THOR over 3 years. Of the 25m, 6m had been released at that point; TSA returned those 6M THOR, and the remaining 19M was never released. However, several other activities were uncovered including an additional undisclosed vesting schedule, this is detailed in section 4 below.

Several attempts were made by THORSwap contributors to contact TSA directly but we did not receive a reply. However, through an intermediary, we were able to recover [2 million THOR](https://etherscan.io/tx/0x36f78bdcc0988447f2386eb4384638f3d08aaee943cbd2da3f9a5817d6381d1c) originating from his undisclosed vesting contract.

After discussing the situation among a group of contributors and some trusted advisors, we proceeded to engage legal counsel to help review and disclose this situation to the community for transparency. We also engaged a third party security auditor to ensure all remaining assets and contracts are secured.

There has been no loss of user funds nor any compromise to the THORSwap platform or its operation. All of the activity we are disclosing occurred months in the past, and all remaining assets were secured when TSA transitioned out. That said, we feel it is important to inform the community about what we found and explain the actions taken in response.

Unwinding this all has taken significant time and effort. We wanted to complete a thorough investigation and fix potential points of failure prior to presenting our findings to the community.

Below is a summary of each of the activities we have uncovered.

## Transfers of $THOR during staking contract creation

- Timeline: March 2022
- Total impact: 600K THOR

When setting up and testing the v1 THOR staking contract, 999,600 THOR was [withdrawn](https://etherscan.io/tx/0xf6b178a09056d968625f9d45a9763efa34e3ceb252f90a28eb447e4458863721) to a wallet used for THORSwap Treasury and known to be controlled by TSA. 

This address was used to operate both THORSwap SushiSwap POL as well as Hammerwallet.eth/forgewallet.eth ENS (THORSwap projects)  

This wallet was labeled “Personal 2” in TSA’s spreadsheet. 

[500k](https://etherscan.io/tx/0x0357fd92865dae25940ea083e0b2fe2f1308d244adf08888c5d1296461d3f58c) THOR was transferred to the “ [Personal 2](https://etherscan.io/address/0x7508abb804b7afba91e9d6cc1be4e918b3068d51) ” wallet and [100k](https://etherscan.io/tx/0xc42a4a8c50e90cc9ad4a3d19a94851bcc8136ecfeee2e6ebacecd6e89c0e5124) to the “ [Dev](https://etherscan.io/address/0x2197b9b22071f77b121a947cbd991aed63959a22) ” Wallet. This 600k THOR was swapped for various other assets in a series of transactions. The remaining 339,600 THOR were returned to the project multi-sig at a later date.

![](https://miro.medium.com/v2/resize:fit:1400/0*qTD9on2PuZ_1D5Ke)

A visualization of transfers through “Personal 2” wallet

## THOR / RUNE Protocol Owned Liquidity

- Timeline: March 2022

- Total impact: 600K THOR


4.1M THOR was [transferred](https://etherscan.io/tx/0x818dd1fa4aa55d7c8235774d17e2c3f5e0666b28dba7311adda636d8644cab6d) from the THORSwap Protocol Owned Liquidity wallet, used for the THORChain THOR/RUNE pool. 

3.5M was then [returned](https://etherscan.io/tx/0xa039d7a16ad21e32cc855e1434ad9d3e0de546539891d5925853e6baec35e2d7). 

The remaining 600,00 THOR were [transferred](https://etherscan.io/tx/0xd299ef65eb5173deb62b9ed7aad2054b6c9195fae88fefafcc9d7b623f4aadfe) to [degenoppa.eth](https://etherscan.io/address/0xb4ad833d6f3b3c4426fea59ded207a952087f47c) (likely TSA’s ENS wallet). This 600k THOR was then sold/swapped.

1. Evidence connecting TSA to the degenoppa.eth wallet:

A wallet labeled [Owner](https://etherscan.io/address/0x4e9f1be1712ca82515da3b661b99c77ec8acb2fc) that had been staking THOR since the token generation event transferred 319,343 THOR (covered in activity #5) to the [Personal 2](https://etherscan.io/address/0x7508abb804b7afba91e9d6cc1be4e918b3068d51) wallet. 

The degenoppa.eth wallet also [sent 389,234 THOR](https://etherscan.io/tx/0x451900b0c7b9208bea7c4336205b1752620afd573bebd2372289b7907c590c58) to the same Personal 2 wallet.

![](https://miro.medium.com/v2/resize:fit:1400/0*BeEpfejg41ylpgL-)

Flow of Funds Through dengenoppa.eth Wallet

## Direct transfers from treasury to personal wallets

- Timeline: April — September 2022
- Total impact: 500K THOR

The [THORSwap deployer](https://etherscan.io/address/0xdd20057b8a4f9565cb871a244f04447be5b03e08), a THORSwap treasury wallet, was used to send [100k](https://etherscan.io/tx/0x10ed99671fa73fb8dc12d94b1dc7e70311dfadf5448d01973474d57d0b8d92f8) THOR directly to the same “ [Personal 2](https://etherscan.io/address/0x7508abb804b7afba91e9d6cc1be4e918b3068d51) ” wallet mentioned above and eventually sold.

Another [treasury wallet](https://etherscan.io/address/0x03061edf0c77b33309d9de0f6f156a2661659bd9) (labeled “Treasury 2” by TSA) used for contributor payouts transferred 400k THOR in 2 transactions ([1](https://etherscan.io/tx/0x7516165002a60db84f391af6f003c189a1993dd20b47c1f65659380223472386), [2](https://etherscan.io/tx/0x45e8fd765df712a238c17023d27b150cc712a1b0b10e41a729f30af7c689e7fd)) to this unknown fresh [wallet](https://etherscan.io/address/0xba2e5a6435793cdf4c54f85b63b8fa27574a68b6). The 400k THOR balance still remains in this wallet and it is the only transaction to this wallet.

## Undisclosed vesting contract

- Timeline: May 2022 — September 2022
- Total impact: ~3M THOR

On May 10th 2022, TSA initiated his founder’s vesting schedule for a total of 25M THOR over 3 years. 

This vesting schedule was known to other contributors and documented, but was later [revoked](https://etherscan.io/tx/0xffe96c67bf2f691a9469223c2a7e863f7100a10a1ccc1c23042f8bc6c77cf588) and the THOR was [returned](https://etherscan.io/tx/0x5dc32528b2d84b68c53cfe8efc8d27ef10929790a502ef6d104b2eee4a7f3992) when he departed the project. 

He detailed this revocation and return of funds in a departure letter written to investors.

However, in the same May 10th [transaction](https://etherscan.io/tx/0x6c16c653afc6ee70d9063561fb71bb9949990d00d02d83aee825db9e394403ea), he also granted an additional unapproved vesting schedule to this [Undocumented Address 0x454](https://etherscan.io/address/0x454857F869882FA426329423389cB5c5Af435B84).

[Undocumented Address 0x454](https://etherscan.io/address/0x454857F869882FA426329423389cB5c5Af435B84) claimed [4.68M THOR](https://etherscan.io/tx/0xd2635855b98e5463e81d52ca32a4122ec39565514cf278ef7b8ac27da47fad33) and [119,500 THOR](https://etherscan.io/tx/0x4fe4f71ce92206bd88e2decb97429f1966c6bfe81826c3d36b820ed228f0f1ce) for a total of ~4.8M THOR before it was revoked by TSA himself, prior to anyone discovering it. 

This THOR was then transferred to another [wallet (145e)](https://etherscan.io/address/0x49e39d91110c736d862dfdc5463e66ff69e8145e) in a series of transactions and staked into the vTHOR vesting contract and slowly sold ~3m THOR to BUSD and BTC over the course of several months. This 145e wallet was also used as intermediary between other known TSA addresses on other chains

THORSwap contributors discovered this undocumented 145e address while it was actively selling THOR tokens, and after tracing the origin back to the vesting contract, we alerted alerted an ecosystem contributor who we understood had several channels of communication with TSA. After this third party contacted TSA, the 145e wallet stopped selling, and [returned 2M THOR](https://etherscan.io/tx/0x36f78bdcc0988447f2386eb4384638f3d08aaee943cbd2da3f9a5817d6381d1c) from 145e to THORSwap’s Contributor & Investor Vesting Contract.

Additional context: TSA had sole control of the Contributor & Investor Vesting [Contract](https://etherscan.io/address/0x0c3c9e5d9b08131dbd82a8648a23592b4dda2223) which was owned by the [THORSwap Deployer](https://etherscan.io/address/0xdd20057b8a4f9565cb871a244f04447be5b03e08), also under his control, until contract ownership was [transferred](https://etherscan.io/tx/0x6ebb43815dddbbbe428e40e880bdf1729819efe99a20cf86a08215dc0e55efb9) to the Multisig Operator wallet in August 2022.

![](https://miro.medium.com/v2/resize:fit:1400/0*lCYQpydfGHtc4LMU)

145e (Interactions with Contributor & Investor Vesting Contract)

## Withdrawing THOR LP Position Funds

- Timeline: November 2021 — June 2022

- Total impact: 920K THOR & 200K RUNE

During the creation of the THOR-RUNE pool on THORChain, TSA used his unique access to the $THOR faucet (which he created) combined with THORSwap Treasury funds, in order to create an extremely advantageous and profitable [LP position](https://viewblock.io/thorchain/tx/09B9AF23639E488F20635ADF8DDC8E320744E1132C66636C6ADD6CA2C6870E94).

Only TSA had control of when the faucet would become activated, since it had to be activated by a transaction originating from “THORSwap: Deployer.” He then used his other address to enter the LP pool just 5 Ethereum blocks after faucet activation.

### TSA deposited 200k RUNE and paired it with 1 THOR. 

We have confirmed that the 200k RUNE was provided to him by the THORChain treasury via these transactions: 

1. https://explorer.bnbchain.org/tx/74BFA2E06D5587398BFB67EA3D78772393F6DB757A3CC8B47CA97155E2038381

2. https://explorer.bnbchain.org/tx/15B50A6735B8CDD18996F023C05D1CD624F9E06BA06B264D2F76FE01F795627F

This RUNE was intended for use by THORSwap Treasury, not for TSA’s personal use.

### LP position withdrawn

The LP position was then withdrawn in three transactions:

1. https://viewblock.io/thorchain/tx/DC49366ED2391B9E78F35B1742567CCC3523EB7BC54111EDCD9B355550900D51

2. https://viewblock.io/thorchain/tx/0F9B2A7FCE47C5ACD8A21A4616A9110B39D5BBB22F189468D3600DEA92389F24

3. https://viewblock.io/thorchain/tx/218FACFFBB870DFFF3F981F69FA0387F4AF6C87D2A00F3651C43BEBC47565404

for 177k RUNE and 920k THOR. 

#### 30k RUNE

30K RUNE was [transferred](https://viewblock.io/thorchain/tx/02AD79A2BFCDA195671278DE6BC2BF2A1FCA5DC3EF0A8862C2A0DAD5ADE174FE) to [Personal 2](https://viewblock.io/thorchain/address/thor17pl9lqca8kamgejxucg5k8fqfgef0xq3k599z3) — used for various trading activities.

Then it was eventually off-ramped to [Binance](https://explorer.bnbchain.org/address/bnb1s679lwerqw63lg3mwkq4d996hfmx90kqunpmv4). 

#### 147K RUNE

The remaining 147K RUNE was [transferred](https://viewblock.io/thorchain/tx/006D5DB5A6C9E38BC534754F57067E29C7AF8FCADF61B44EF123D47538377EFB) to this [wallet f205](https://viewblock.io/thorchain/address/thor1gdty4yq4sfjm08tn3y4atjm9vzgn4n4hfqf205) — sold for stablecoins in many transactions netting ~$1.35M USD.

Then it was eventually off ramped through Binance at this [address](https://explorer.bnbchain.org/txs?address=bnb17xjgzxlhm6ntmlvgfrlnjpnag3v8ynn673a8wy). 

#### 920K THOR

920K THOR was [staked](https://etherscan.io/tx/0x614f4139eae5548a6e3612a41b9fe4b35ee45dce8fc0871cdbd3151bcc120779) into the v1 THOR staking contract and earned 319K THOR in rewards. 

The net 1.24M THOR was then [sold via several transactions](https://etherscan.io/address/0x7508abb804b7afba91e9d6cc1be4e918b3068d51#tokentxns).

## Summary

All told, approximately 6M THOR and 200K RUNE were improperly transferred without any disclosure or notification. Nearly all of the assets have been sold or swapped for various digital assets including BTC, NFTs, stable-coins, etc. The only outstanding THOR we believe TSA still has access to is the 400k THOR sitting [here](https://etherscan.io/address/0xba2e5a6435793cdf4c54f85b63b8fa27574a68b6). Over $1.5M USD appears to have been [off-ramped](https://explorer.bnbchain.org/txs?address=bnb17xjgzxlhm6ntmlvgfrlnjpnag3v8ynn673a8wy) via Binance.

It is interesting to note that if TSA had continued to contribute to the project, the25M THORthat was officially vested to him would have far outweighed the amount he transferred without disclosure. Indeed, at the time of his exit, he returned 6M THOR from his official vesting contract, almost exactly the amount he had taken over the previous 12 months.

Additionally, all contributors involved in the investigation agreed not to sell any vested tokens until the investigation was completed and our analysis disclosed to the community. Two contributors with knowledge of the investigation proceeded to sell some of their vested tokens prior to this disclosure. This has resulted in their remaining vesting being revoked, and they are no longer contributors.

O ur Response: The root cause of these undisclosed, unapproved, and unexplained transactions were due to a single person having total control over THORSwap Treasury assets.

This single point of failure was rectified upon TSA’s departure 6 months ago. Many steps have been taken to remove all single points of failure to prevent a situation like this from reoccurring in the future:

- all Treasury assets and THORSwap controlled contracts were moved to a series of multi-sig wallets
- a third party security team [reviewed](https://static.thorswap.net/Disclosure/Upshield-THORSwap-Review.pdf) all treasury vaults, smart contracts, and infrastructure to ensure that all remaining funds and infrastructure are properly secured
- multiple initiatives to progressively decentralize all aspects of the THORSwap project

In the spirit of transparency, along with this public disclosure, we are [publishing a report](https://static.thorswap.net/Disclosure/THOR-Emissions-to-date.pdf) detailing token emissions to-date.

## Progressive Decentralization:

We have been steadily working toward progressively decentralizing additional aspects of the THORSwap project and will continue to do so:
- Migrating away from reliance on cloud providers
- Soon releasing and open sourcing our libraries and SDK
- Improving deployment resilience and supporting decentralized deployment via IPFS
- Shifting governance decisions to the larger THORSwap community

## Moving Forward

It is important to reassure the community that these undisclosed and unapproved transactions were taken by a single actor, TSA, who has not been involved with the project for the past 6 months.

Despite the significant time and effort this investigation and disclosure required, THORSwap contributors have continued to deliver industry leading cross-chain products and services: more chain support, DEX aggregation, Savers vaults, new partner integrations and much more.

The future of THORSwap remains bright. We are blessed by a vibrant community and a diverse group of contributors around the globe who remain committed to building the best cross-chain De-Fi experience for users and developers alike.

Thank you for your continued support,

THORSwap Contributors




## Onchain

- 0xa82b8d05514d4218a213a7f85d081bf632b46b75 - Thorswap Staking Contract
- 0x0c3c9e5d9b08131dbd82a8648a23592b4dda2223 - Contributor Vesting Contract 
- 0x6755630c583f12ffbd10568eb633c0319db34922 - Thorswap SingleStaking Contract
- 0x03061edf0c77b33309d9de0f6f156a2661659bd9 - Treasury 2 
- 0xdd20057b8a4f9565cb871a244f04447be5b03e08 - Thorswap Deployer 
- 0xb4ad833d6f3b3c4426fea59ded207a952087f47c - TSA degenoppa.eth 
- 0xc23dce883008f9e0146e50bfa8d311a17b00ea4e - TSA hammerwallet.eth - controlled by TSA
- 0x4e9f1be1712ca82515da3b661b99c77ec8acb2fc - Theft - "Owner"
- 0xba2e5a6435793cdf4c54f85b63b8fa27574a68b6 - TSA "Personal"
- 0x7508abb804b7afba91e9d6cc1be4e918b3068d51 - Theft - "Personal 2"
- 0x2197b9b22071f77b121a947cbd991aed63959a22 - Theft - "Dev"
- 0x454857F869882FA426329423389cB5c5Af435B84 - Theft - Undocumented Address 454 (unapproved vesting schedule)
- 0x49e39d91110c736d862dfdc5463e66ff69e8145e - Theft - Receives from Undocumented Address 454
- thor1gdty4yq4sfjm08tn3y4atjm9vzgn4n4hfqf205 - Theft - 147K RUNE
- thor17pl9lqca8kamgejxucg5k8fqfgef0xq3k599z3 - Theft - Personal 2
- bnb17xjgzxlhm6ntmlvgfrlnjpnag3v8ynn673a8wy - Theft - Binance Depo
- bnb1s679lwerqw63lg3mwkq4d996hfmx90kqunpmv4 - Theft - Binance Depo, From Personal 2

- 0x36f78bdcc0988447f2386eb4384638f3d08aaee943cbd2da3f9a5817d6381d1c
- 0xf6b178a09056d968625f9d45a9763efa34e3ceb252f90a28eb447e4458863721
- 0x0357fd92865dae25940ea083e0b2fe2f1308d244adf08888c5d1296461d3f58c
- 0xc42a4a8c50e90cc9ad4a3d19a94851bcc8136ecfeee2e6ebacecd6e89c0e5124
- 0x818dd1fa4aa55d7c8235774d17e2c3f5e0666b28dba7311adda636d8644cab6d
- 0xa039d7a16ad21e32cc855e1434ad9d3e0de546539891d5925853e6baec35e2d7
- 0xd299ef65eb5173deb62b9ed7aad2054b6c9195fae88fefafcc9d7b623f4aadfe
- 0x451900b0c7b9208bea7c4336205b1752620afd573bebd2372289b7907c590c58
- 0x10ed99671fa73fb8dc12d94b1dc7e70311dfadf5448d01973474d57d0b8d92f8
- 0x7516165002a60db84f391af6f003c189a1993dd20b47c1f65659380223472386
- 0x45e8fd765df712a238c17023d27b150cc712a1b0b10e41a729f30af7c689e7fd
- 0xffe96c67bf2f691a9469223c2a7e863f7100a10a1ccc1c23042f8bc6c77cf588
- 0x5dc32528b2d84b68c53cfe8efc8d27ef10929790a502ef6d104b2eee4a7f3992
- 0x6c16c653afc6ee70d9063561fb71bb9949990d00d02d83aee825db9e394403ea
- 0xd2635855b98e5463e81d52ca32a4122ec39565514cf278ef7b8ac27da47fad33
- 0x4fe4f71ce92206bd88e2decb97429f1966c6bfe81826c3d36b820ed228f0f1ce
- 0x6ebb43815dddbbbe428e40e880bdf1729819efe99a20cf86a08215dc0e55efb9
- 0x614f4139eae5548a6e3612a41b9fe4b35ee45dce8fc0871cdbd3151bcc120779
- 09B9AF23639E488F20635ADF8DDC8E320744E1132C66636C6ADD6CA2C6870E94
- 74BFA2E06D5587398BFB67EA3D78772393F6DB757A3CC8B47CA97155E2038381
- 15B50A6735B8CDD18996F023C05D1CD624F9E06BA06B264D2F76FE01F795627F
- DC49366ED2391B9E78F35B1742567CCC3523EB7BC54111EDCD9B355550900D51
- 0F9B2A7FCE47C5ACD8A21A4616A9110B39D5BBB22F189468D3600DEA92389F24
- 218FACFFBB870DFFF3F981F69FA0387F4AF6C87D2A00F3651C43BEBC47565404
- 02AD79A2BFCDA195671278DE6BC2BF2A1FCA5DC3EF0A8862C2A0DAD5ADE174FE
- 006D5DB5A6C9E38BC534754F57067E29C7AF8FCADF61B44EF123D47538377EFB
