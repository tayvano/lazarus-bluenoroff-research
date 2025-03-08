# DAO Maker

Amount Stolen:: $7,000,000

Date:: August 12th, 2021

Tags:: 💼 Admin Key Compromise 


---

## Details

CEO Christoph Zaknun said hackers were able to remove roughly $7 million in USD Coin USDC from 5,251 user accounts.

DAO Maker, an encryption incubator, issued an announcement stating that at around 1:00 UTC on August 12th, hackers maliciously used a DAO Maker wallet and obtained administrator rights. After initially testing this vulnerability and successfully stealing 10,000 USDC, the cybercriminal made another 15 transactions quietly. In this way, hackers embezzled approximately $7 million before the security team was able to track, control, and prevent the outflow of funds. A total of 5,251 users were affected, and each user lost an average of $1250. Fortunately, users who hold up to $900 in funds are not affected at all

> Regretfully, we must announce that in the early hours of August 12th (approx. 1 AM UTC) DAO Maker faced malicious use of one of our wallets with access to admin privileges.

> The admin's private key was used to grant the attacker's contract permission to withdraw funds from the exploited contract. The cybercriminal, after tentatively testing this exploit and managing to steal 10,000 USDC, then proceeded to quietly make 15 more transactions. In this manner, the hacker was able to siphon approximately $7M, until our security team was able to trace, contain and stop the drain of funds. A total of 5251 users were affected, losing $1250 USD on average per user



### Onchain

- 0x054e71D5f096a0761dba7dBe5cEC5E2Bf898971c - the original deployer (legit)
- 0x0Eba461D9829C4e464A68D4857350476CFb6F559 - EOA wallet, admin (legit)
- 0x41B856701BB8c24CEcE2Af10651BfAfEbb57cf49 - DAO Maker
- 0x1C93290202424902a5e708b95f4ba23A3F2F3Cee - Exploiter Contract
- 0xd8428836ed2a36bd67cd5b157b50813b30208f50 - Exploiter, Direct Theft
- 0xef9427bf15783fb8e6885f9b5f5da1fba66ef931 - Laundry / TC
- 0x895d7ba5fb4043722214042e43d7fde4c3449307 - TC, donates just to Gitcoin:TC address
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
- https://certik.com/projects/daomaker
- https://quadrigainitiative.com/casestudy/daomakerexploit.php
- https://web3rekt.com/hacksandscams/dao-maker-270
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




---



# DAO Maker #2

Date:: September 3rd, 2021

Amount Stolen:: $4,000,000

Tags:: Unprotected init


DaoMaker was exploited for ~$4m. They left the `init` function unprotected. The attacker re-initialized the contract with malicious data and then called `emergencyExit` to get away with the funds.

On 3rd of September 2021, around 10:00 PM UTC, DAO Maker, a decentralized finance platform on the Ethereum blockchain that enables startups to raise funds, was hacked for almost $4 million (although the true realized cost to DAO Maker is far greater). A collection of altcoins were stolen; DeRace Token (DERC), Capsule Coin (CAPS) Showcase (SHO) and Coinspaid (CPD). Evidently, the hacker was preparing for the recent crypto market rout as the stolen tokens were swapped to the stablecoin Dai using DEX aggregators 1inch and Metamask. The attacker is still holding the Dai on the same Ethereum blockchain address the stolen tokens were initially sent to.Updated 6/5/22: 300 ERTH was sent to [[Tornado Cash]] by the exploiter via an intermediary address

They left the `init` function unprotected. The attacker re-initialized the contract with malicious data and then called `emergencyExit` to get away with the funds.

Attacker was able to reinitialize the token and empty funds

The source code is not public and some messaging by DaoMaker is questionable

They called the required functions one by one rather than creating a contract to do it in a single transaction. They also used [[1inch]] for a swap.

All of this points to the attacker being not very technical. 

However, the source code of the contract was not public. You need deep technical knowledge to find this vulnerability without the source code. This makes one wonder how the attacker knew about this vulnerability.


### Onchain

- 0x2708cace7b42302af26f1ab896111d87faeff92f - Primary Theft
- 0x0b7894e365a0f8a7e3e294ea6562071497da2f83
- 0xd08c13ee849d7e7936a57cc60cecab46c7e3b743
- 0xbe70cf6749d97df054f4edbe51a3c63634f77eba
- 0xa79e633bd0f735abe64657d4a6208efdc674dfb0


### URLs

- https://drive.google.com/file/d/1tPRMktnros6ifJLfvQkrT6mAmEJvUufT/view
- https://web3rekt.com/hacksandscams/dao-maker-251
- https://rekt.news/daomaker-rekt/
- https://slowmist.medium.com/intelligence-of-slowmist-zone-dao-makers-vesting-system-was-hacked-5825e4828969
- https://quadrigainitiative.com/casestudy/daomakerinsufficientauthentication.php
- https://twitter.com/Mudit__Gupta/status/1434059922774237185
- -https://twitter.com/Mudit__Gupta/status/1434059922774237185
