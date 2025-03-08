# Nexera

Date:: August 7th, 2024

Amount Stolen:: $1,900,000

Tags:: 🎙️ Contagious Interview

---


## Details

On August 7, 2024, Nexera Fundrs experienced an exploit that led to the unauthorized transfer of 47.24 million NXRA tokens from its smart contracts, with approximately 14.75 million tokens sold, valued at around $449,000.

The incident occurred when an external actor gained unauthorized access to the credentials for managing Nexera Fundrs’ smart contracts. Utilizing this access, the attacker transferred NXRA tokens from the Fundrs staking contracts on Ethereum and accessed the vesting contract on Avalanche. Despite the breach, the attackers were unable to access NXRA tokens stored in users' wallets. Upon detecting the incident, the Nexera team promptly paused the NXRA token contract, halting all Onchain transactions. They also removed the remaining 32.5 million NXRA tokens from the attacker’s wallet, mitigating further potential losses. The attackers exploited BeaverTail malware, a method consistent with state-backed threat actors, to deploy the attack.

~47.2 million NXRA tokens or approximately $1.9m

Token price crashed 40%

Nexera's proxy contract at root of exploit

~448k USDT to BSC via the StarGate


## Persona

Request for Assistance via Linkedin 

> it seems like that you are very technical in the field of smart contract.

> we are going to integrate solidity smart contract functions into chat room page of this project.

> if you can, please help us to analysis current project status and give us technical estimate.

> then we can go with your document and get more funds.

> we will pay $100 for 1 hour project checking & document work

> and we can work hourly from next week.

> https://github.com/newbee96422/MetaWar_ver_4

> This is the project

> Check this please

> If you are interested, please get back to me soon

> https://linkedin.com/in/aline-santoro-2a2029215



### Onchain

- Burns tokens after: https://etherscan.io/tx/0xbb89f990344d0d0bd7dea0676ddd58089c2d4ebd398bde1965f14057eb3b5154
- 0xe697949817a45446776376db203c04d31b580a10 - Direct Theft
- 0x6bd33c8256f7a37336b2b8fe967321e25540337b - Direct Theft
- 0x8856eb9b59d7e68ca7fcb2c76ff67e9a70fe9141 - Theft/Laundry
- 0xadb7482d62d771e696ffbba07259fd0abd5d9190 - Theft/Laundry
- 0xd138ae2013bd501ba42f1b5d914e3a0afd3fcf92 - Theft/Laundry
- 0x1e6cb086100b264e5fcb02dfccd5f4aff6385efc - Theft/Laundry
- 0xf8d02d8bc8cfb3b50ee8fd21a1e21e0154fcee0b - Theft/Laundry
- 0xa736a6cf4239f3919740d9a434be358593f03fbc - Theft/Laundry
- 0x75fd76edc59a68c4de14ce248fa499b333d577f5 - Theft/Laundry
- 0xcfefd927aaa992c931809401dc36b6ca9a1d5cf4 - Dust
- TCVgK96xZbZFu1sNPvX2RAThZ4gzkAcC4c - Theft/Laundry
- TFTiEEaV4Kc8nb5TJKmXM238EQBLZMGE89 - Theft/Laundry
- TS33JwYCvEMiioh2hYuqPZCiyYdb416KBj - Theft/Laundry


### URLs

- https://github.com/newbee96422/MetaWar_ver_4
- https://linkedin.com/in/aline-santoro-2a2029215
- https://twitter.com/nexera_official/status/1821079381831512315
- https://archive.ph/SFeBd
- https://t.me/investigations/148



## Connections

> Attacker is connected Onchain to recent private key compromise incidents such as SpaceCatch, Concentric Finance, OKX DEX, Serenity Shield, Reach, and many more.

> https://zapper.xyz/bundle/0xe697949817a45446776376db203c04d31b580a10,0x6bd33c8256f7a37336b2b8fe967321e25540337b?id=0xab5640e604766596c91d77c26b52bdd0e0181b81&label=nexera&icon=%F0%9F%92%B0

—[zachxbt](https://t.me/investigations/148)



### Other victim - August 28, 2024

0x1046726f5311e721e1d532c9a59d654b339433a2

https://chainabuse.com/address/0x1046726f5311e721e1d532c9a59d654b339433a2?chain=ETH

> I've got contacted by Vlad Martsenyuk on Likendin, that he is a recruiter for Peru-based crypto-exchange TOTExchange and they're looking for senior blockchain developers. We stayed in contact and discussed details. He sent me a google form where was the job description and application process, so I applied for it. They wanted from me my CV, my Github and some basic contact information. After some hours, they have invited me to a Github repo under user TOTExchange-dev, where they told me is the MVP version of their new website and that I should give them feedback. The website was written in Typescript and in the evening hours I was lazy to open the source codes, so just cloned the repo, installed all dependencies through sudo yarn install. After that I just changed the install term for "start" so I put in terminal sudo yarn start. The website started but Terminal asked for a permission to my hard drive (I clicked allow) and the website was shown, however it was with some error and also the website stated Happy365Global, so obvious fake web, in that moment, I just closed everything, deleted repo and went to bed disappointed (I was really tired). In the morning I found out, that all my crypto wallets in any browser got dumped out to one address and I have nearly zero balance everywhere. That was the moment, when I realized I got robbed :( I just quickly opened the source codes (I still haev them, so can provide the whole code for investigation) and after some time found out, that there are IP addresses, API calls and also some wss call to ngrok app (of course already down). And that's the place I think where hackers have hidden some malicious code which got to my computer through websockets and download my Metamask seed phrases from browser storage, maybe also my passwords from Keychain.