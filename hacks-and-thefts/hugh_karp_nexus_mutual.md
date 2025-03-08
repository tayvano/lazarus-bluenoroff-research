# Hugh Karp / Nexus Mutual

Date:: December 14th, 2020

Amount Stolen:: $8,000,000

Theft via custom MetaMask to steal funds off Ledger

Time:: 9:40am UTC

Tags:: 🔑 Keys Not Compromised, Ledger

--


## Details

Malicious MetaMask, compromised computer hardware wallet. malicious ext came from coinbene[.]team

This was a targeted, personal attack on Hugh. Hugh was using a hardware wallet. The attacker gained remote access to his computer & modified his MM tricking him into signing a diff txn than what MM / Ledger showed him even though he was using a hardware wallet.

December 14th, 2020 at 9:40am UTC, I was tricked into approving a single transaction that sent 370,000 NXM to a hacker instead of what I thought was claiming some mining rewards. The hacker has subsequently liquidated the majority of the NXM into ETH/BTC and has been dispersing it to many different addresses and exchanges.

I was using a Ledger connected via Metamask to interact with the Nexus Mutual application at the time. Computer was Windows OS.

December 11th, 2020 10:20 UTC I was writing an email and my computer screen went black for 2–3 seconds.

December 11th, 2020 My MetaMask extension was altered from disk and replaced with an infected version. See the background.js file and this diff for details.

December 14th, 2020 09:40 UTC I went to claim some shield mining rewards on the Nexus Mutual application. As usual, Metamask pops-up asking for confirmation, nothing appears odd at this point, as Metamask presents the information I expect. However, it is in fact hiding a spoof transaction that it will send to the Ledger. I hit confirm as all looks ok.

While most Metamask attacks phish your private keys by tricking you into downloading a malicious version, this was not the case here. My computer was compromised and Metamask was altered from disk. This means the browser extension warning would not flag.

On December 14, Hugh Karp, the CEO of DeFi insurer Nexus Mutual, lost the equivalent of $8 million in NXM tokens in a targeted attack by one of the project’s own members. The hacker executed the attack by completing Nexus Mutual KYC process to become a member; later, the attacker switched to a new address and gained remote access to Karp’s computer and modify Karp’s MetaMask wallet extension.

Fortunately, no other members have been attacked, and, according to a Nexus Mutual tweet, “The mutual is not impacted; the pool of funds and all systems are safe.” However, after the attack was exposed, the price of Nexus Mutual wrapped tokens dropped 14% on the cryptocurrency exchange Huobi. A portion of the stolen funds were located on 1inch.exchange, a decentralized exchange aggregator.




## On the KYC Details

> The official said that this is a targeted attack, only the official name, Karp used a hardware wallet, the attacker obtained remote access to his computer, and modified the wallet plug-in MetaMask, deceived him to sign the transaction, the attacker Completed KYC 11 days ago, and then changed to a new address on December 3

This ended up being another DPRK victim in Singapore who had multiple wallets emptied just prior to the Hugh Karp attack. This theft, along with Fetch.ai and other unknown / unreported thefts from the Fall 2020 all co-mingle on chain.



## Onchain

- https://etherscan.io/tx/0xfe2910c24e7bab5c96015fb1090aa52b4c0f80c5b5c685e4da1b85c5f648558a 
- 0x09923e35f19687a524bbca7d42b92b6748534f25 - Theft
- 0xad6a4ace6dcc21c93ca9dbc8a21c7d3a726c1fb1 - Theft
- 0x03e89f2e1ebcea5d94c1b530f638cea3950c2e2b - Theft
- 0x0784051d5136a5ccb47ddb3a15243890f5268482 - Theft
- 0x0adab45946372c2be1b94eead4b385210a8ebf0b - Theft
- 3DZTKLmxo56JXFEeDoKU8C4Xc37ZpNqEZN - Theft

- 0x78a9903af04c8e887df5290c91917f71ae028137 - Post ChipMixer Consolidation

- 0x0864b5ef4d8086cd0062306f39adea5da5bd2603 - Post March ChipMixer Consolidation with CoinMetro hack

- 0xb27d40fb4a7975e6f4e6bd7f9fbf6e8d53bf8298 - More consolidating on the ETH side

- 0x8e7f5d85c3587725b1188d3cc04ca814ab60cdce - Bixin deposit address

- 0x593dc5e1ad81667bbfc90739dd2c09c926920e3b - Paxful deposit address

- 0x2e1155cf5374cba058a04fd03ebd0ba19afe580d - Noones deposit address


### ChipMixer

- db0cd0f1cb5bd13b9b3249e6a560aaeddbd0134d0f678220e626b20a424473ce - CM Deposit 30 BTC
- 1586fec6363ba1d6bac3056e4aee0bc0b4fefdf37f6060850b2d9168c39e6683 - CM Deposit 50 BTC
- eb4854fb3ea8a3f5d87331b04bfc4daeac76343ebcbcaeff976551fadb5050cc - CM Deposit 41.99 BTC
- 0b6b1a990b6aab6edaef925c4af2a03f64c1a03ee98d3309f9557029af415f66 - CM Withdraw 15 BTC
- 9726abb675bff14f512018a583693e815857829dc2459556938a491900638e21 - CM Withdraw 60 BTC 
- ffeb3dd56d0bde492cd08c0975edad38524f5ef003f55c258e75638044324acf - CM Withdraw 42 BTC

### Tornado Cash

- 0x0784051d5136a5ccb47ddb3a15243890f5268482 - Deposit 
- 0x78a9903af04c8e887df5290c91917f71ae028137 - Withdrawals

## URLs

- https://certik.medium.com/nexus-mutual-attack-8-millions-lost-8d3592d14cfa
- https://medium.com/@hugh_karp/nxm-hack-update-72c5c017b48 
- https://twitter.com/HughKarp/status/1341063567408328705
- https://twitter.com/NexusMutual/status/1338441875326427137
- https://breadcrumbs.app/reports/0x09923e35f19687a524bbca7d42b92b6748534f25/1/10/10
- https://quadrigainitiative.com/casestudy/nexusmutualfounderhacked.php
- https://web3rekt.com/hacksandscams/nexus-mutual-425

## Malicious MetaMask

- payload diff https://gist.github.com/banteg/53a62b1f5eab56c8d4841786fc94d3ca
