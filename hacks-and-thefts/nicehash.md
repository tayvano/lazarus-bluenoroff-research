# NiceHash

Date:: December 6th, 2017

Amount Stolen:: $65,000,000 (4,736.42 BTC)

Tags: CEX Hack, Slovenia, BTC


---


## Details


Slovenian company Nicehash, a market place for trading computer hashing power to mine crypto-currency, lost $75,000,000 worth of crypto-currency. The hacker was able to infiltrate an internal system through VPN with one of the company engineer’s credentials. After the VPN login, the hacker transferred the funds to his or her own account. It is still unknown how the hacker could obtain the credential and how long the hacker maintained the connectivity to the internal network. 

However, the active attack timeline was only a couple of hours. Later, many Nicehash users have expressed a surprise to learn that the company’s Chief Technology. Officer recently served several years in prison for operating and reselling a massive botnet, and for creating and operating ‘Darkode,” one of the world’s most bustling English-language cybercrime forums.

Nicehash was a cryptocurrency mining service and marketplace, allowing users to buy and sell their own mining power. While not necessarily a mining pool of its own, it still maintained a wallet for customer funds. Nicehash appears to have shuttered their website with a notice saying “a security breach involving NiceHash website” and “our payment system was compromised and the contents of the NiceHash Bitcoin wallet have been stolen”. A [Facebook livestream](https://facebook.com/NiceHash/videos/2013146182237851/) has further notes on the issue. This is hard to archive so I will transcribe useful points. Overall, this was lateral movement from a remote IP address, gaining access to a VPN, possibly through an employee computer, and moving laterally into production systems. This appeared to all have happened within a couple of hours, when the attacker decided to work actively. 1. “We became a target and someone really wanted to bring us down.” 2. “We are cooperating with local and international law enforcement”. 3. ~4700 BTC stolen on early morning 12-06-2017 4. Can’t discuss everything due to investigation. 5. Hacker(s) were able to *infiltrate our internal systems through a compromised company computer*. 6. Unknown how company computer was compromised. 7. *VPN had visibility into abusive behavior*, IP address was outside of European Union. 8. “Made a crucial VPN login using *an engineer’s credentials*” 9. After VPN login, *learned and simulated the workings of our payment system*. 10. Managed to steal funds from accounts (indicates that the *active attack timeline was only a couple hours*)

It was determined that on December 4th, 2017, a conspirator sent a spear-phishing communication to an employee of the Slovenian Cryptocurrency Company, which included a hyperlink that redirected the employee to download a file containing malware.

> It is clear that the threat actor gained persistent access to the NiceHash internal network through a spear phishing email and was able to perform lateral movement within our data center via the stolen VPN credentials. The Indicators of the Compromise (IoCs), recovered in the digital forensic analysis of the breach, indicated similarities with techniques, tactics and procedures (TTPs) of a known nation-state threat actor. Based on the method and procedures of intrusion, this attack resembles TTPs used by the LAZARUS group, though the full threat actor attribution is still under investigation by the U.S. Law Enforcement Agencies.

> “The threat actor performed a technically flawless compromise of the NiceHash systems, and with military precision executed the transfer of bitcoins. This attack was targeted, and the threat actor was highly skilled, organized and acted with high speed”, commented Ondrej Krehel, CEO of LIFARS.

- [NiceHash security breach investigation update](https://web.archive.org/web/20181113075633/https://nicehash.com/news/niceHash-security-breach-investigation-update)



## Attribution

- "Slovenian Crypto Company" [US v 113](https://github.com/tayvano/lazarus-bluenoroff-research/blob/main/pdfs/2020-03-02_USA-v-113_yinyin_complaint-cv-606.pdf)

- Page 28 of [UN Security Council's North Korea 2019 Midterm Report](../pdfs/2019-08-30_UN-Security-Council_s-2019-691.pdf)

- This [comprehensive report on the incident](https://lazarus.day/media/post/files/2023/12/22/Lessons-Learned-from-64-Million-Dollar-Cryptocurrency-Hack-Case-Study.pdf)



## Onchain

- 1EnJHhq8Jq8vDuZA5ahVh6H4t6jh1mB4rq


## URLs

- https://archive.is/pWTbH
- https://archive.org/web/20181113211702/ 
- https://bitcointalk.org/index.php?topic=2535366.0
- https://coindesk.com/62-million-gone-cryptocurrency-mining-market-nicehash-hacked
- https://facebook.com/NiceHash/videos/2013146182237851/  
- https://krebsonsecurity.com/2017/12/former-botmaster-darkode-founder-is-cto-of-hacked-bitcoin-mining-firm-nicehash/
- https://lazarus.day/media/post/files/2023/12/22/Lessons-Learned-from-64-Million-Dollar-Cryptocurrency-Hack-Case-Study.pdf
- https://nicehash.com/news/niceHash-security-breach-investigation-update 
- https://web.archive.org/web/20181113075633/https://nicehash.com/news/niceHash-security-breach-investigation-update
- https://cnbc.com/2017/12/07/bitcoin-stolen-in-hack-on-nicehash-cryptocurrencymining-marketplace.html 
- https://coindesk.com/62-million-gone-cryptocurrencymining-market-nicehash-hacked/ 
- https://justice.gov/opa/pr/three-north-korean-military-hackers-indicted-wide-ranging-scheme-commit-cyberattacks-and
- https://quadrigainitiative.com/casestudy/nicehashexchangehack.php
- https://reddit.com/r/NiceHash/comments/7i0s6o/official_press_release_statement_by_nicehash/
- https://wikitribune.com/story/2017/12/11/technology/nicehash-ceo-speaks-outafter-60m-cryptocurrency-hack/27212/ 