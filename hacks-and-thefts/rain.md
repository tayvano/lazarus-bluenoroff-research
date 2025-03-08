# Rain 

Date:: April 29, 2024

Amount Stolen: $16,130,000

Tags:: 🔐

---

## Details

> It appears the crypto exchange Rain was likely exploited for $14.8M on April 29, 2024 after their BTC, ETH, SOL, and XRP wallets saw suspicious outflows. Funds were quickly transferred to instant exchanges and swapped for BTC and ETH.

> Stolen funds currently sit:

- bc1q53aawrkpt5lvk2e30z36unvmhqqdru7q4rprp2 - 137.9 BTC 

- 0x197bc094f990261fd6841342901c451858756c28 - 1881 ETH

–[zachxbt](https://t.me/investigations/122)


Losses on BTC, LTC, DOGE, XRP, SOL, ETH

Directly following initial thefts, all assets swapped for BTC and ETH via ChangeNOW, Whitebit, and using Exodus's in-app swaps.

AWS, VPN interface, VULTR, Bitgo, Exodus in-app swaps

## Onchain

On May 14-16, 2024 funds were moved and depositted to a mixer:

- bc1qd3hs38w4m42p395v0czfy57tw4ppcpuxt058lt (35 btc)

- bc1q89za2yjlgzngndvqwpwemkzj7gzkxq82nvzfjv (50 btc)


On June 24, 2024, Ethereum was moved to:

- 0x3751aA0D047173d6dAc0a6bA3363c53EC5097f99

- 0x6B0470c7257537674D75b185CDFC358F2Cee9d87



On August 7, 2024, 0x6B0470c7257537674D75b185CDFC358F2Cee9d87 depositted into Tornado Cash.

- 11x100 ETH
- 5x10 ETH
- 5x1 ETH
- Total: 1155 ETH in 21 Deposits



On August 9, 2024, 0x3751aA0D047173d6dAc0a6bA3363c53EC5097f99 depositted into Tornado Cash.

- 7x100 ETH
- 2x10 ETH
- 6x1 ETH
- Total: 726 ETH in 15 Deposits



## IoCs


- Asia/Yakutsk timezone

- Mullvad VPN

- ko language setting


## Forfeiture

https://storage.courtlistener.com/recap/gov.uscourts.dcd.275374/gov.uscourts.dcd.275374.1.0.pdf

Rain Management W.L.L., also known as Rain.com, is licensed by the Central Bank of Bahrain as a Category 3 Crypto-Asset Services Provider.2 As a Crypto-Asset Service Provider, Rain.com offers its customers the ability to swap between different currencies, purchase or sell virtual currency, manage customer’s portfolios and assist with investment decisions. Rain Management is headquartered in the Kingdom of Bahrain.

29. On or about April 29, 2024, Rain.com was targeted by TraderTraitor malware, which the FBI knows to be associated with APT38. That targeting resulted in a financial loss to Rain.com of approximately $16.13 million, including approximately $760,997.68 in SOL.
As described in more detail below, of the $16.13 million stolen, the FBI was able to successfully freeze 2210.8222 SOL at WhiteBIT, a virtual currency exchange headquartered in Vilnius, Vlinias Apskritis, Lithuania.

### Rain.com’s Response to the Theft

30. In sum, Rain.com conducted an internal investigation. That investigation revealed that actors gained unauthorized access to Rain.com’s virtual currency using one of North Korea’s signature malware strains, TraderTraitor. According to Rain.com, the infiltration only enabled the exploitation of the Rain.com “send” wallets. A “send” wallet likely refers to Rain.com’s “hot wallet” used to send money to customers. A hot wallet is a key storage method for any private key that is connected either directly to the internet or through another device.
31. After the theft, Rain.com hired Mandiant Inc.4 (“Mandiant”) to investigate the cybersecurity breach. When conducting their investigation, Mandiant learned that a Rain.com employee (“Employee 1”) was compromised. Specifically, based on the investigation to date, law enforcement assesses that North Korean cyber actors contacted Employee 1 on LinkedIn and asked if Employee 1 was interested in a new job. Employee 1 indicated that Employee 1 was interested, so the North Korean cyber actors sent Employee 1 a malicious link disguised as a coding challenge. When Employee 1 downloaded the coding challenge, Employee 1’s device was compromised with malware. This malware allowed the North Korean actors to steal private keys and credentials that ultimately gave the actors access to Rain.com’s infrastructure managed by BitGo. That was important because Rain.com used BitGo to interact with and manage Rain.com’s virtual currency assets and infrastructure. After the foothold was established via Employee 1, the North Korean actors stole virtual currency from Rain.com and deleted the malware from Employee 1’s device.
32. The funds that are the subject of this warrant were traced from Rain.com’s wallets to WhiteBIT, where they were frozen pending seizure.
33. Below is a graph, created by the FBI, of the transactions involved in the theft through the deposit of stolen funds at the WhiteBIT exchange:

### Details Regarding Tracing the Stolen Funds to WhiteBIT
34. FBI investigators traced a total of eight transactions involving funds stolen from Rain.com’s hot wallet to an address controlled by the North Korean cyber actors and/or their money laundering co-conspirators, “DrkSpv…RQom.” Beginning on or about April 29, 2024, at 01:54 GMT, and continuing through 03:42 GMT, through these eight transactions, the actors stole 5,505.904159384 SOL, which was valued at approximately $760,997.68 as of the date of the theft.
35. Of the 5,505.904159384 SOL sent to address “DrkSpv…RQom,” approximately 4,890 SOL was sent in seven transactions to seven different addresses at WhiteBIT, as described below. Of the 4,890 SOL, approximately 2,211 SOL was sent in two transactions of approximately 1,500 SOL and approximately 710.753138909 SOL from “DrkSpv…RQom” to WhiteBIT. Approximately 1,500 SOL was sent to WhiteBIT deposit address “JDZvMk…SB1K7,” and approximately 710.753138909 SOL was sent to WhiteBIT deposit address “EJe7Ca…Pb6nf.” 
36. On or about May 7, 2024, WhiteBIT’s Anti-Money Laundering and Financial Monitoring Departments suspended 2,204.8222 SOL6 associated with the 1,500 SOL and 710.753138909 SOL deposits and thereafter consolidated that SOL into WhiteBIT address 8mowmVCEewZ9W2cEaQyQeQEeSxhGr1hvRviLwozwNtBt (the Defendant Property).
37. North Korean cyber actors typically launder stolen funds through several exchanges, swapping currencies or value to different blockchains, to make following those assets more difficult and to prevent stolen funds from being frozen by law enforcement. What happened here is no different; the Lazarus Group, APT38, transferred the virtual currency to WhiteBIT to launder the virtual currency and obfuscate the nature, source, location, ownership, or control of stolen funds.