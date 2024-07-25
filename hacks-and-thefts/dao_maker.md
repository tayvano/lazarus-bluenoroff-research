# DAO Maker

Amount Stolen:: $7,000,000

Date:: August 12th, 2021

Tags:: 💼 Admin Key Compromise 


---

CEO Christoph Zaknun said hackers were able to remove roughly $7 million in USD Coin USDC from 5,251 user accounts.

DAO Maker, an encryption incubator, issued an announcement stating that at around 1:00 UTC on August 12th, hackers maliciously used a DAO Maker wallet and obtained administrator rights. After initially testing this vulnerability and successfully stealing 10,000 USDC, the cybercriminal made another 15 transactions quietly. In this way, hackers embezzled approximately $7 million before the security team was able to track, control, and prevent the outflow of funds. A total of 5,251 users were affected, and each user lost an average of $1250. Fortunately, users who hold up to $900 in funds are not affected at all

> Regretfully, we must announce that in the early hours of August 12th (approx. 1 AM UTC) DAO Maker faced malicious use of one of our wallets with access to admin privileges.

> The admin's private key was used to grant the attacker's contract permission to withdraw funds from the exploited contract. The cybercriminal, after tentatively testing this exploit and managing to steal 10,000 USDC, then proceeded to quietly make 15 more transactions. In this manner, the hacker was able to siphon approximately $7M, until our security team was able to trace, contain and stop the drain of funds. A total of 5251 users were affected, losing $1250 USD on average per user




### On-chain

- 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c - the original deployer (legit)

- 0x0Eba461D9829C4e464A68D4857350476CFb6F559 - EOA wallet, admin (legit)

- 0x1C93290202424902a5e708b95f4ba23A3F2F3Cee - attacker malicious contract

- 0x41B856701BB8c24CEcE2Af10651BfAfEbb57cf49 - Exploiter

- 0x26aa86261c834e837f6be93b2d589724ed5ae644bc8f4b8af2207e6bd70828f9




### URLs

- https://blocksecteam.medium.com/the-analysis-of-the-daomaker-attack-32365c37e7fc
- https://cointelegraph.com/news/dao-maker-crowdfunding-platform-loses-7m-in-latest-defi-exploit
- https://drive.google.com/file/d/1tPRMktnros6ifJLfvQkrT6mAmEJvUufT/view - Whitepaper
- https://github.com/openblocksec/blocksec-incidents/blob/main/defi/2021.md
- https://medium.com/daomaker/5-steps-plan-removing-all-smart-contract-custody-risk-by-end-of-the-month-3f7bd22b92c8
- https://medium.com/daomaker/dao-maker-compensation-plan-b7a76a312c30
- https://medium.com/daomaker/dao-maker-statement-thursday-12th-of-august-2c3bb0d1bb69
- https://medium.com/daomaker/dear-users-and-supporters-of-dao-maker-e00a5f3a3883
- https://www.certik.com/projects/daomaker
- https://www.quadrigainitiative.com/casestudy/daomakerexploit.php
- https://www.web3rekt.com/hacksandscams/dao-maker-270
- https://twitter.com/peckshield/status/1425778230968135684
- https://twitter.com/PeckShieldAlert/status/1532936259877732358



### Ethsec Convo
- 4b4f892a -> getUserAvailableBalance(address,address)
- 50b158e4 -> withdrawFromUser(address,address,uint256)
- Looking at the last tx, it passes in 349 addresses and then does this loop
- 0xd8428836ed2a36bd67cd5b157b50813b30208f50
- Investigation revealed 9 connections to 8 clusters, where are 2 direct connections, and 7 indirect. 
- https://web.amlbot.com/aml/response/5EC6CA4DDB26177/26412520210812153733:E505D29ADCAA9AC 
- No clues still, lets wait 🤔
- an insider? looks it bypasses access control
- The DAO Maker sho controller should be controlled only by the Dao
- https://bloxy.info/tx/0x2fba930502d27f9c9a2f2b9337a0149534dda7527029645752b2a6507ca6b0d6
- There is more 'grantRole's before this transaction...
- 0x0eba461d9829c4e464a68d4857350476cfb6f559
- 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c
- https://gist.github.com/banteg/a2e4897ad73d7d6bedff525f89e88f2b
- here 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c grants admin role to 0x0Eba461D9829C4e464A68D4857350476CFb6F559
- https://bloxy.info/tx/0xa1b4fceb671bb70ce154a69c2f4bd6928c11d98cbcfbbff6e5cdab9961bf0e6d
- they also grant admin role to 0x1F8Db5982bE60b6543d4069268555564c498B3dA which looks like a gnosis safe

> safe = Safe('0x1F8Db5982bE60b6543d4069268555564c498B3dA', EthereumClient())

> safe.retrieve_owners() -> ["0x7B03314B2f51e3Bb845BF8ADd51A254a89b646B5", "0x45166749C271F0688F624f6C1e897Ad14B8bF6d7", "0xcF28556EE95Be8c52AD2f3480149128cCA51daC1", "0x3a8CE3451f3C5a040578D568c5A61090F97f2BF4"]

- the attacker needed a SC to withdraw the funds. 
- he deployed it here: 0x1c93290202424902a5e708b95f4ba23a3f2f3cee#code
- 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c grants -> 0x0Eba461D9829C4e464A68D4857350476CFb6F559 grants -> 0x1C93290202424902a5e708b95f4ba23A3F2F3Cee (Attacker's Contract)
- already know this, but what about the account 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c? Any useful information?
- Need to wait, anyways (if speaking about scoring). Made a quick cluster check, now checking for false positives
- legit... so Private Key Compromise?
- yes
- https://t.me/c/1372269197/38260