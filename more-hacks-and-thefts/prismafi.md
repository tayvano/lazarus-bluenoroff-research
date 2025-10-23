# PrismaFi    

Date:: 2024-03-26

Amount Stolen:: $11,100,000

Tags:: ❌ Not DPRK

---

## Notes

Attributed in [MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities](./pdfs/2025-10-22_MSMT-Report.pdf)

I don't see any universe where this is DPRK

It's a solid DeFi Hack and the attribution Zach did to the idiot asshole in Vietnam/AU is also strong.

Connections to Arcade (Mar 2023) and Pine (Feb 2024) hacks are also strong.

Not everthing is DPRK. Especially not DeFi exploits.



## Details

- A vulnerability in both versions of the MigrateTroveZap (mkUSD and ULTRA) contract of Prisma Finance led to a loss of 3,479.24 ETH, or approximately $12 million USD.

- In response, the Prisma Finance emergency multi-sig has paused the protocol's operations.

- The vulnerable contract is a special-purpose contract designed to migrate user positions from one trove manager to another.

- The vulnerability affects Prisma Trove owners who approved this contract to manage their Trove's position via setDelegateApproval(MigrateTroveZap, True) on the BorrowerOperations contract.

- The issue occurred when an exploiter made a transaction that, with a lack of input validation in the onFlashloan function, allowed the exploiter to manipulate the contract's behavior and take a portion of a Trove owner's collateral.

- As a result, the exploiter was able to close a Trove owners Trove, withdraw the collateral (wstETH), and reopen the Trove with the same debt (mkUSD) but less collateral, taking the difference.

- A thorough investigation is conducted to identify the root cause and implement necessary fixes.

- There was a primary exploiter (Exploiter 1) followed by copycat exploiters.

- Trove owners should verify they have revoked any active approvals for the MigrateTroveZap.

- He was a talkative little fucker:

> Your team need to do an online press conference, in which all of your team must show their faces with ids (it s like KYC), and send apologies and thanks to all of your users, your investors, and me. During that session, you must specifically present the mistake you made, which party audited the smart contract, and your plan to improve security in the future (what you would do before deploying a new contract, how you react when an something you don t expect comes, etc.). Also, you need to admit that I have no responsibilities in this, and I m purely helping you guys to fix your mistakes. Out of that, you also need to change all the terms that are accusatory in the post-mortem within 12 hrs.


### Timeline

- 2024-03-28 11:15 UTC: Exploiter 1 wallet is funded via FixedFloat exchange

- 2024-03-28 11:22 UTC: Exploiter 1 Exploit contract is deployed

- 2024-03-28 11:25 UTC: Exploiter 1 calls function 0x82be0b96, initiating the transaction.

- 2024-03-28 11:29 UTC: The Prisma Team is alerted by a community member on Discord.

- 2024-03-28 11:51 UTC Prisma announces a potential incident on Twitter.

- 2024-03-28 12:11 UTC: Prisma advises users to revoke delegate approval on both LST and LRT BorrowerOperations

- 2024-03-28 12:41 UTC: Exploiter 2 executes its first transaction.

- 2024-03-28 12:49 UTC: Exploiter 3 executes its first transaction.

- 2024-03-28 12:51 UTC: Emergency multi-sig calls Paused()


### Zach Thread on Attribution

> An investigation into the alleged $11.1M @PrismaFi exploiter 0x77 (Trung) and the multiple other exploits they are connected to.
> On March 28, 2024 the Prisma team observed a series of transactions on the MigrateTroveZap contract which resulted in a loss of 3257 ETH ($11.1M)
> Exploiter address
> 0x7e39e3b3ff7adef2613d5cc49558eab74b9a4202
> A comprehensive post-morten of the incident can be found: https://x.com/PrismaFi/status/1773726224952480049
> At first the attacker communicated with the Prisma deployer the attack was whitehat.
> Later that day all of the funds were deposited to Tornado Cash contradicting that statement. 
> The exploiter began making outrageous demands and asked for a $3.8M (34%) whitehat bounty 
> This amount is significantly higher than the industry standard 10% essentially extorting the team as the treasury does not have sufficient assets to reimburse users.
> On-chain the exploiters address was funded via FixedFloat. 
> Using timing analysis the source address was then located on Arbitrum. 
> 0xd71f1590ad9008056d5d079835bdf5044c0b81fa
> 2000 USDT source transaction at 11:13 am UTC
> 0x93b047e530249592e50bde889c31f5346096ad2ae59073dec15abd39d05e3b20
> 0.553 ETH ($1.95K) received by Prisma exploiter at 11:15 am UTC
> 0xe55bd15d2bd17c0a97356f612480887df91bc483f6affae8edd06a6d08b60f53
> A timing analysis of Bybit withdrawals received by the exploiter revealed activity connected to them on Tron
> TGviNZQUpZ9ywameoCXCrJYctF463y556m
> TGdTGkY7oqW9PKeZ5HGomfqY73zogoAMCf
> I found TGviNZ funded by the Arcade_xyz exploit from March 2023 where the exploiter requested additional funds from the protocol. 
> Arcade exploiter
> 0x807350917efa87fb15ed7eb0952635cdf1c13366
> Further investigation revealed the team had been in contact with the exploiter who was using the alias ‘0x77’ on Telegram with the account still active.
> I then found the exploiter connected to another exploit on Pine Protocol from February 2024.
> Pine exploiter
> 0x05324c970713450ba0bc12efd840034fcb0a4baa
> For this one the team did not agree to a bounty as they asked for 50% and made additional unreasonable requests over email.
> I then discovered the exploiter’s address connected to the deployer of @modulusprotocol
> 0x77 was one of the few followers of the project strengthening the connection between each incident. 
> Deployer address
> 0x29300e694a77d913248d1761d7e4f2d81c350159
> Further analysis was conducted with the phone number, emails, and other details of the alleged exploiter. 
> From their posts on X it is clear they have a strong technical background. 
> As of now all personal details have been compiled and the Prisma team is pursuing every possible legal avenue in Vietnam and Australia. 
> I urge the exploiter to return the funds and save everyone time before this gets much worse for them.

[Source: ZachXBT](https://x.com/zachxbt/status/1780244613808160958)




## Further Reading

- https://hackmd.io/@PrismaRisk/PostMortem0328

- https://x.com/PrismaFi/status/1773316945430852058

- https://quadrigainitiative.com/casestudy/prismafinancetrovemanagerexploit.php

- https://etherscan.io/idm?addresses=0x2d413803a6ec3cb1ed1a93bf90608f63b157507a,0xd8531a94100f15af7521a7b6e724ac4959e0a025&type=1

- https://www.theblock.co/post/285776/prisma-finance-hacker-defends-exploit-demands-public-apology






## Onchain

- 0x7e39e3b3ff7adef2613d5cc49558eab74b9a4202 - Exploiter 1
- 0x2d413803a6eC3Cb1ed1a93BF90608f63b157507a - Exploiter 1
- 0x57f7033F84894770F876bf64772E7EBA48990D65 - Exploiter 1
- 0x5d0064f3B54C8899Ab797445551058Be460C03C6 - Exploiter 1
- 0xce63dd78232b218cd0c13c1eaceb1e2c7518f098 - Exploiter 1

- 0x7Fe83f45e0f53651b3ED9650d2a2C67D8855e385 - Exploiter 2

- 0x7C9FC6E2B908e858F30c5c71a20273315Efd5cf8 - Exploiter 3





### Victims of Exploiter 1

- 0x56A201b872B50bBdEe0021ed4D1bb36359D291ED  1745.08 wstETH  463.18 wstETH   11:25:11 AM +UTC
- 0x774bb9306df1cd921eb842b1388c78f75e6ef79f  172.18 wstETH   149.36 wstETH   11:28:11 AM +UTC
- 0xcbfdffd7a2819a47fcd07dfa8bcb8a5deacc9ea8  824.6 wstETH    192.12 wstETH   11:29:11 AM +UTC
- 0xc47fae56f3702737b69ed615950c01217ec5c7c8  40 wstETH   11.69 wstETH    11:36:47 AM +UTC
- 0x3b15cec2d922ab0ef74688bcc1056461049f89cb  107.18 wstETH   18.89 wstETH    11:43:23 AM +UTC
- 0x1b72bac3772050fdcaf468cce7e20deb3cb02d89  166.41 wstETH   47.49 wstETH    11:45:47 AM +UTC
- 0x3b15cec2d922ab0ef74688bcc1056461049f89cb  18.89 wstETH    18.97 wstETH    11:48:11 AM +UTC
- 0x16f570e93fdbc3a4865b7740deb052ee94d87e15  113.6 wstETH    32.4 wstETH 11:53:47 AM +UTC
- 0xf9ca66ef84c773fab422562ab41b1ee8d4397418  47.3 wstETH 15.48 wstETH    11:54:47 AM +UTC
- 0xc487370895f6e8f5b62d99bf1472c95a94073379  377.2 wstETH    95.6 wstETH 12:07:47 PM +UTC
- 0x9fceded3a0c838d1e73e88dde466f197df379f70  356.28 wstETH   102.12 wstETH   12:12:47 PM +UTC

### Victims of Exploiter 2 

- 0x14b30b46ec4fa1a993806bd5dda4195c5a82353e  4.22 wstETH 1.21 wstETH 12:42:11 PM +UTC
- 0x19562df3e7fd2ae7af4e6bd288b04c2c90405212  31.22 wstETH    9.15 wstETH 12:46:35 PM +UTC
- 0x1b004189e64d5b2f71d5be554470e6c49e10123b  21.74 wstETH    5.98 wstETH 12:46:59 PM +UTC
- 0x3b82ee6c15b212ed69d5795bcd957e136eaa4bff  13.02 wstETH    3.45 wstETH 12:47:11 PM +UTC
- 0x409c6c5ec5c479673f4c09fb80d0f182fcff643e  3.8 wstETH  0.93 wstETH 12:47:23 PM +UTC
- 0xc47fae56f3702737b69ed615950c01217ec5c7c8  11.69 wstETH    11.78 wstETH    12:49:11 PM +UTC
- 0xf8d1c9ab49219f7acf7b1d84705e5aea3b8ce0aa  17.85 wstETH    17.93 wstETH    12:49:35 PM +UTC
- 0x19562df3e7fd2ae7af4e6bd288b04c2c90405212  9.15 wstETH 9.23 wstETH 12:50:23 PM +UTC
- 0x409c6c5ec5c479673f4c09fb80d0f182fcff643e  .99 wstETH  1.06 wstETH 12:50:35 PM +UTC
- 0x4a3fced7c536e39ca5292a024ee66c9b45b257ec  87.93 wstETH    19.85 wstETH    12:50:47 PM +UTC
- 0x19562df3e7fd2ae7af4e6bd288b04c2c90405212  9.23 wstETH 9.3 wstETH  12:51:47 PM +UTC

### Victims of Exploiter 3

- 0xf8d1c9ab49219f7acf7b1d84705e5aea3b8ce0aa  70.3 wstETH 17.85 wstETH    12:49:35 PM +UTC
- 0x3b82ee6c15b212ed69d5795bcd957e136eaa4bff  3.45 wstETH 3.52 wstETH 12:50:23 PM +UTC
- 0x409c6c5ec5c479673f4c09fb80d0f182fcff643e  0.93 wstETH .99 wstETH  12:50:35 PM +UTC









