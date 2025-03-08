# Theft from Fantom Foundation C-Level

Amount Stolen:: $7,624,588

Date:: October 17, 2023

--


## Notes

- It's likely a single device or devices on a single network were compromised leading to the compromise of multiple wallets holding assets belonging to an employee of the Fantom Foundation and the Fantom Foundation wallets themselves.

- A total of approximately $7m was stolen in this single incident. The likely cause is, again, complete device pwnage due to DPRK malware. Most likely employee is Fantom CEO Michael Kong.

- DPRK attribution comes, in part, from observations on DPRK-controlled C2s as well as Onchain laundering and timing matching other thefts that occuring the same week.




## Details:

The Fantom Foundation, developer of the Fantom network, was hacked for over $550,000 in cryptocurrency, initially reported as $7 million by blockchain security researchers.

The foundation clarified that most of the stolen funds belonged to other users, and 99% of their own funds were secure. Some wallets mislabeled by block explorers were initially thought to belong to the foundation but were later reassigned to an employee and no longer held company funds.
The attack is under investigation to determine how the wallets were compromised.

The attack targeted the foundation and other Fantom wallet users, rather than the Fantom network itself.


### Page 550 of [The 2023 UN Report](https://documents.un.org/doc/undoc/gen/n24/032/68/pdf/n2403268.pdf?token=Lnb4xBoncpFwgtMIpl&fe=true)

Attack methodology:

- As part of a spearphishing campaign by the attacker(s) on Telegram, a Fantom Foundation employee received a message from an individual claiming to be the founder of an established blockchain and investment fund and purporting to be located in an Asian country, who was interested in investing in Fantom Foundation and requested a video call to discuss (see Figure 16). The attacker was not pushy or forceful in setting a date for the call.

The attacker sent a video link to join the call that resulted in an “access restricted” message (see Figure 17); the attacker sent a troubleshooting link which automatically downloaded an Applescript file without any warnings or prompts (see Figure 18). The file contained troubleshooting instructions to run a script, which did not result in any abnormal computer processes and was not identified as malicious by antivirus software.

After approximately 25 minutes of “troubleshooting”, the attacker agreed to meet on another, established platform, at a later date. However, the same day as the initial call attempt, the victim noticed messages disappearing from Telegram, and less than 24 hours later, wallets associated with the victim’s Metamask Chrome Browser extension were being drained (both personal and those of Fantom Foundation). The extension subsequently crashed and the victim was unable to use Chrome; after a compute restart, the Chrome application disappeared completely. By the time the victim re-downloaded Chrome and Metamask and restored access to wallets, they were almost completely drained.


Subsequent investigation determined that malicious IP address 104.168.137.21 had gained unauthorized access to the victim’s computer to effect the heist, and that the script had resulted in all of the victim’s Chrome data (including Metamask wallets) being stolen.

This attack is part of a broader Lazarus Group campaign of spearphishing on Telegram, targeting the cryptocurrency industry (see para 188).

The attacker(s) stole 47 cryptocurrencies from the Ethereum, Optimism, Fantom, Polygon, and Arb blockchains, from 11 cryptocurrency wallets (see Figure 19). 

The stolen cryptocurrency was converted into Ether (ETH) using services such as Squid Router and deposited into Tornado Cash.



## URLs

- https://twitter.com/CyversAlerts/status/1714308396453695518/photo/1
- https://twitter.com/BeosinAlert/status/1714326758894551477/photo/2
- https://twitter.com/FantomFDN/status/1714337765502992798
- Page 550 of [The 2023 UN Report](https://documents.un.org/doc/undoc/gen/n24/032/68/pdf/n2403268.pdf?token=Lnb4xBoncpFwgtMIpl&fe=true)



## Onchain

- 0x1bffb3a232e06e06a5d9e93c8df3321f768197c2 - Victim Foundation Wallet 1 
- 0x48f7572cfbc4f246600cf816c668271034d81f8f - Victim Foundation Wallet 16 
- 0x386aa44439e9c7181b1f0f1cac0efa478b623b27 - Victim Foundation Wallet 18 
- 0x596288a9090c9eedf87bb5f2da5d8e1bbc7bb935 - Victim Foundation Wallet 20 
- 0x4a6ff07acd81f8d0ec7dd51f325d86b833821b1d - Victim
- 0x124cb46cebd37ef9bf8b41c47f2f1bd5136656af - Victim
- 0xd2976a56cd84a91a2e83685a6dc5308315e29f15 - Victim
- 0xb86b137232c4e9b67f2b9bfd3d5641b77df70065 - Victim
- 0x3cba76e6a3298b19b77bd3b6a7bbc0b209e712b4 - Victim
- 0xdc3d7bca4c9db233ae10f4af3c1bd105a5818cce - Victim
- 0xb0e3baec3ba1990ebd2edf9eedc2f3213b381fb1 - Victim
- 0x8658bcf88c5d08f02ea5393ecd4a2b5e28c3e349 - Victim
- 0x00FBB426dd3b92384384ED870B74cf39eFC5b8F8 - Victim
- 0xb48677997e6e88c2cd1825017ccac3054b4080fc - Victim Safe Addy? 
- 0x50e0f818e870be4d5e5f012ff90d304db6e1e69b - Victim Safe Addy?
- 0x431e81e5dfb5a24541b5ff8762bdef3f32f96354 - Fantom Foundation (not compromised) 
- 0xa51b1bc907fe0a6bc6538c5c56472c1d9c60de23 - Fantom Controlled Wallet (not compromised?) 
- 0x2f4f1d2c5944dba74e107d1e8e90e7c1475f4001 - Theft 
- 0xdadc0421ee1b5426fca3db22f0a94a3bad5a329d - Theft  
- 0x1d93c73d575b81a59ff55958afc38a2344e4f878 - Theft 
- 0x0b1f29df74a19c44745862ab018d925501fe9596 - Theft TC 3x100 
- 0x5cdeffa84ee3c203fee7a3901d90ff464ebff801 - Theft TC 46x100
- 0x0c45060bc4c518b6942f19d7c279ed42e137d29d - Theft Jan 2024
- 0xdd92ff524b3b58adb55b9e4824749ba5b0993842 - Theft Jan 2024 FixedFloat
- 0x91decd1d92ff2cb5d83c9415bbb72d582599fb4c - Theft Jan 2024 ETH, FTM, OP
- 0x8d82d316fc421c44e3a7f3604ff965e7a19d438c - Theft Jan 2024 Intermediary
- 0xf857bb93eb57183ad42593496da46de83cf29d44 - Theft Jan 2024 Intermediary
- 0x0c45060bc4c518b6942f19d7c279ed42e137d29d - Theft Jan 2024 Intermediary
- 0xc0b635fb9dc28dea84db150b89d4578ff9859877 - Fantom/DPRK Dust Collector Jan 2024


## Tornado Cash

- 0x5cdeffa84ee3c203fee7a3901d90ff464ebff801
    - 46 Deposits
    - 4600 ETH
    - 2023-10-31 14:42
    - 2023-11-07 12:22

- 0x0b1f29df74a19c44745862ab018d925501fe9596
    - 3 Deposits
    - 300 ETH
    - 2023-10-25 2:59
    - 2023-10-25 3:02


## Related

- [March 2025 Hack](./march2025.md)



