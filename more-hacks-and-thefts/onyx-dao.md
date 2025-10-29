# Onyx Protocol / Onyx DAO    

Date:: 2024-09-26

Tags:: ❓DPRK IT Workers 

---


## Details

- Attributed in [MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities](./pdfs/2025-10-22_MSMT-Report.pdf)

It's a DeFi hack. It's not DPRK. I've documented both incidents for your enjoyment. 🤦‍♀️ ITW dump at the bottom


---

# Incident #1 

Date:: 2023-11-01

Amount Stolen:: $2,149,772


## Details


Onyx Protocol, a decentralized P2P lending platform, was exploited via Flash Loan resulting in a loss of 1,164.53 ETH, approximately $2.1 million.

The incident underscores concerns about vulnerabilities in decentralized finance (DeFi) platforms, especially in markets with low liquidity.

The attacker targeted a known bug related to a rounding issue in the CompoundV2 fork, a widely used framework in the DeFi sector.

This bug went unnoticed by Onyx Protocol until it was identified by blockchain investigator PeckShield.

The attacker exploited the oPEPE market, which lacked liquidity, by manipulating donations to borrow funds from more liquid markets and redeeming them through the rounding issue exploit.

A similar attack occurred on April 16 against the multichain lending protocol Hundred Finance, resulting in a $7 million loss.

In this case, the attacker manipulated the exchange rate between ERC-20 tokens and hTOKENS to withdraw more tokens than initially deposited.

These incidents highlight the need for better understanding and proficiency in tracking cryptocurrencies to mitigate risks in DeFi platforms, involving transaction tracing, address clustering, behavioral analysis, pattern recognition, regulatory vigilance, and collaboration for platform security and integrity.

The attacker manipulated the exchange rate with a flashloan and redeemed PEPE for profit by exploiting the redeemUnderlying


## On-Chain


- 0x085bdff2c522e8637d4154039db8746bb8642bff - Exploiter 1
- 0x526e8e98356194b64eae4c2d443cc8aad367336f - Exploiter 1 Contract
- 0x4c9c8661243e9e9a15a35b8873317eb881330c98 - Theft / Laundry (to Tornado Cash)
- 0x30e4d4e89369cf4d91cb675448db0b2f126c1caf - Funding (from Tornado Cash)
- 0x43083e943cd4d35f242f7850be2402126a57d6b5 - Funding (from Tornado Cash)
- 0xf7c21600452939a81b599017ee24ee0dfd92aaaccd0a55d02819a7658a6ef635 - Malicious Txn (Nov 2023)

- 0xaee294951f2b69b8c7720eed7ff05dbb4b184a86 - Messages the Exploiter and gets some free $$$
- 0x0afd3eb64466d046496aaf5f14bc9cab817fc489 - Messages the Exploiter and gets some free $$$
- 0x1b0e83d29787023c56f18e9001b3158f0eafae8b - Messages the Exploiter and gets some free $$$
- 0x351a71f64ad0294fca267696e9ba4c6f1f6ac419 - Messages the Exploiter and gets some free $$$

All to Tornado Cash 2023-11-01 10:42 


- 0x5083956303a145f70ba9f3d80c5e6cb5ac842706 - Exploiter 3
- 0x052ad2f779c1b557d9637227036ccaad623fceaa - Exploiter 3 Contract
- 0x27a3788d504af542681436bfdecf1823f7a8a691d04309ad33e6d3825e899746 - Malicious Txn (Nov 2023)
- 0xaee294951f2b69b8c7720eed7ff05dbb4b184a86 - Messages the Exploiter and gets some free $$$


## Further Reading

- https://blog.solidityscan.com/onyx-protocol-hack-analysis-372facda4a55
- https://coinpaper.com/2567/new-v2-money-market-protocol-may-help-onyx-recover-from-hack
- https://community.onyx.org/t/the-onyxprotocol-experienced-an-exploit/1125
- https://cryptorank.io/news/feed/8cfde-onyx-protocol-exploited-peckshield-reports-2m-ethereum-theft
- https://github.com/SunWeb3Sec/DeFiHackLabs?tab=readme-ov-file#20231101-onyxprotocol---precission-loss-vulnerability
- https://hacken.io/discover/onyx-protocol-hack/
- https://medium.com/@invitedtea/analysis-for-onyx-exploit-2023-nov-1st-by-keybox-ai-c4d195bb65e9
- https://medium.com/@sharkteam/sharkteam-analysis-of-the-onyx-protocol-attack-incident-principles-0cabeb2bb9f2
- https://twitter.com/Phalcon_xyz/status/1719697319824851051
- https://twitter.com/SlowMist_Team/status/1719667931926413679
- https://twitter.com/DeDotFiSecurity/status/1719690524603425113
- https://www.coinlive.com/news/onyx-protocol-exploiter-drains-2-1m-from-tornado-cash
- https://www.dlnews.com/articles/defi/hacker-drains-funds-through-pepe-market-on-onyx-protocol/
- https://www.halborn.com/blog/post/explained-the-onyx-protocol-hack-october-2023
- https://www.oodaloop.com/briefs/2023/11/02/onyx-protocol-victim-of-2-million-exploit/
- https://www.web3rekt.com/hacksandscams/onyx-protocol-1789


---

# Inident #2

Date:: 2024-09-26

Amount Stolen:: $3,800,000


## Details


The Onyx protocol was hacked for a second time  resulting in a loss of over $3.8 million.

The attacker exploited a known precision issue in the Compound V2 code. 

Additionally, the NFTLiquidation contract failed to properly validate untrusted user input, allowing the attacker to inflate the self-liquidation reward amount, which further worsened the losses.

The attackers took advantage of a known precision loss vulnerability in the forked Compound V2 code that Onyx DAO implemented. 

By deploying a malicious contract, they manipulated the market’s exchange rates within the protocol, artificially inflating the value of small deposits. 

This allowed them to withdraw 4.1 million VUSD along with other cryptocurrencies, such as XCN, DAI, WBTC, and USDT. 

The attackers executed multiple transactions to miscalculate and inflate their token values, minting excessive amounts of VUSD, which they then converted to other cryptocurrencies. 

Onyx apparently didn't learn their lesson the first time around, when they were exploited for $2m in November 2023 an attacker taking advantage of a known vulnerability affecting empty markets on the protocol. 

This same bug seems to have contributed to this exploit, although Onyx has claimed the hack was due to a separate vulnerability in an NFT liquidation contract.

> Speaking of unnecessary hacks, Onyx Protocol was hacked again for $3.8M with the Compound bug that already cost them $2M about a year ago. The issue here is a lack of process and/or knowledge of your code base. A simple playbook on [how to safely deploy new cTokens](https://twitter.com/hexagate_/status/1650177767965700102) would have saved their day.

- Source: Blockthreat


## Onchain

- 0x680910cf5Fc9969A25Fd57e7896A14fF1E55F36B - Primary Exploiter (Sep 2024)
- 0xa57eDA20Be51Ae07Df3c8B92494C974a92cf8956 - Exploiter Contract (Sep 2024)
- 2024-09-26 12:01:59 [0x46567c731c4f4f7e27c4ce591f0aebdeb2d9ae1038237a0134de7b13e63d8729](https://etherscan.io/tx/0x46567c731c4f4f7e27c4ce591f0aebdeb2d9ae1038237a0134de7b13e63d8729)
- 0x7Af460547300e30290f63d21E0d1c5BE6e87ace8 - Theft/Laundry (2024-10-31)
- 0x29485afa514455e9d5b849d0a4771971016a896f - Theft/Laundry (2024-11-06)
- 0xf15ea0986d346b61edd377ab00ffd85752b4ce8f - Theft/Laundry (2024-11-07)
- 0x1fbe96d22696028f14c1278d1839059b07e762b5 - Theft/Laundry (2024-11-07)
- bc1qh6lnelsvksn6cf3gva5w6fndjrlxc5h8mdhl46 - Dormant as of 2025-10-22 (2024-11-07)
- bc1qlvcrkjc20xkc6paegh2ajtqcg8jp72keck4nxj - Dormant as of 2025-10-22 (2024-11-07)
- bc1q2hspzvnl226892dq224z3htexy3df828snx4e0 - Dormant as of 2025-10-22 (2024-11-07)


- 0x0000000000004f3d8aaf9175fd824cb00ad4bf80 - Bot, Also RoulettePotV2 Exploiter
- 0x000000000000bb1b11e5ac8099e92e366b64c133 - Bot, Also RoulettePotV2 Exploit Contract
- 2024-09-26 15:45:23 [0x7d89055543e57a9e12305c674b6f7c2091b5d8ea235b21473a3a5dcb83f36c87](https://app.blocksec.com/explorer/tx/eth/0x7d89055543e57a9e12305c674b6f7c2091b5d8ea235b21473a3a5dcb83f36c87


- 0x5995af29d3726b3a697fe91f41f92786802d8c45 - Another Bot
- 2024-09-26 15:45:47 [0x0ee347f153166a3b6b2518a67fffff09688ea0892ac3c4de9a560b7458428abc](https://etherscan.io/tx/0x0ee347f153166a3b6b2518a67fffff09688ea0892ac3c4de9a560b7458428abc)


### Further Reading

- https://cointelegraph.com/news/onyx-protocol-exploited-second-time-3-8m-via-known-bug
- https://www.bitget.com/news/detail/12560604235782
- https://www.theblock.co/post/318499/defi-protocol-onyx-hit-with-a-3-2-million-exploit-marking-second-attack-within-a-year
- https://x.com/CyversAlerts/status/1839284600461303958
- https://x.com/OnyxDAO/status/1839444120060023167
- https://x.com/OnyxDAO/status/1839444121938706847
- https://x.com/peckshield/status/1839296480357789902
- https://x.com/peckshield/status/1839298850605142413







# DPRK IT Workers Dump

Super fucking incomplete, what a fucking goddamn shitshow. First guy defo begs for money in Onyx github.

Second guy def associated with him

There are dozens more in this cluster.

### 0xopsdev / Nelo Labhart

- 0xopsdev
- its0xopsdev
- meta0xflip
- Nelo Labhart
- nelo.labhart
- the Swallow
- Zireael
- ZireaelGit
- t.me/its0xopsdev (id: 7692311172) (fka: t.me/Meta0xFlip)
- github.com/0xopsdev
- github.com/meta0xflip
- x.com/0xopsdev
- trycoco.me
- nelo.labhart@gmail.com
- @MediaSurgeGG dev (from x.com/0xopsdev bio)
- @MutantRolls co-founder (from x.com/0xopsdev bio)
- @OnyxDAO ex-dev(ai agent) (from x.com/0xopsdev bio)
- @BrainrotGamez ex-dev (from x.com/0xopsdev bio)
- Hey, I have rich experience in building AI Agents (from https://x.com/0xopsdev/status/1978501615586881729)
- 0x7a87c66718255c5be3c0607e134592d9a8bdb32c (from https://github.com/Onyx-Protocol/onyxcoin/issues/2)


### m4rcu5o / Apollum

- J.YATES
- m4rcu5o
- j_apollum
- idioRusty
- idioguru
- richrusty015
- apollum
- m4rcu5sol
- x.com/m4rcu5sol
- x.com/m4rcu5o/
- x.com/j_apollum/
- x.com/m4rcu5o/status/1924920118783447408
- x.com/x_fivefingers
- hudes0112@gmail.com
- matthiasli.com (via twitters, @idioRusty 8064597851 https://t.me/Solanavietnamdev/5127) • [Archive](https://archive.ph/2YHWo)
- @idioRusty @idioguru @richrusty015 (ID: 6715083084)
- @idioRusty @apollum  (ID: 8064597851)
- https://x.com/j_apollum/status/1957891599222075777 • [Archive](https://archive.ph/2sycY)
- https://x.com/x_fivefingers/status/1958332104171004031 • [Archive](https://archive.ph/6DcfK)
- https://x.com/x__rusty/status/1835936833026642250 (deleted, linked from @idioRusty 6715083084)
- https://t.me/Solanavietnamdev/5127 • [Archive](https://archive.ph/2YHWo)
- https://x.com/x_fivefingers/status/1973454463454290090 • [Archive](https://archive.ph/dqUpv)
- https://x.com/m4rcu5sol/status/1923422538253627566 • [Archive](https://archive.ph/wip/I1tOF)


### So Much More

- https://www.ketman.org/dprk-it-workers-github-organizations.html#:~:text=The%20Core%20Team%20of%20HyperbuildX

- ![](../dprk-it-workers/matthias-li-tovar-idiorusty.jpg)


Separately, this motherfucker Ryuhei AGAIN:

- https://github.com/r2moon

- ryuheimat3@gmail.com


















