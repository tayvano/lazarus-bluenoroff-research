# Wannacry

Date:: May 12th, 2017

Tags:: Ransomware, ShapeShift, Monero

Amount Stolen:: $200k (52+ BTC)

---

## Details

Organizations across the world reported ransomware infections affecting their computer systems. The infections, caused by a ransomware strain referred to as WannaCry, restrict users’ access to a computer until a ransom is paid to unlock it. Reportedly, 300,000 users in at least 150 countries were affected by the ransomware.20 The WannaCry worm was initially delivered through phishing attacks, but was able to spread more quickly than normal ransomware, as it exploited security vulnerabilities to move remotely between unpatched computers.

In April 2017, an anonymous online group known as the Shadow Brokers released what it alleged was a series of surveillance-enabling tools stolen from the National Security Agency (NSA) that, among other things, exploited a Microsoft Windows security vulnerability known as EternalBlue.

It was then reported that Microsoft had patched the vulnerabilities that these tools exploited the previous month, prompting speculation that NSA had alerted Microsoft to the theft.

Included in the March 2017 security update was a patch to protect against the propagation of WannaCry ransomware. Subsequently, only unpatched systems were susceptible to WannaCry, including outdated versions of Windows. Its proliferation was further inhibited after the implementation of a “kill switch” on May 12, 2017.23 

North Korea is suspected to be the architect of WannaCry, which experts say was written after the Shadow Brokers release.24 According to news reports, the NSA issued an internal assessment that linked the ransomware to North Korea’s RGB.

The assessment attributes WannaCry to North Korea with “moderate confidence,” and includes as evidence IP addresses in China that are known to have been used by the RBG. The WannaCry hackers are said to be part of the “Lazarus Group” that was also behind February 2016 SWIFT hacks (see below). In both cases, the cyberattacks may have been used as an attempt to raise revenue for the regime. However, some security researches believe that flaws in the WannaCry code and its demands for payment in digital currency suggest that the hackers may have used WannaCry to accumulate personal wealth.26 The hackers raised $140,000 in the digital currency bitcoin through WannaCry but have yet to convert it to hard cash, reportedly most likely due to an operational error that has made the transactions trackable by law enforcement entities.27

The largest ransomware attack in history, infecting more than 300,000 computers in more than 150 countries and causing more than $4 billion in damage. The attack crippled the United Kingdom’s National Health System, affecting one-third of hospitals providing intensive care and other emergency services and 8 percent of general medical practices.129


The [UN Security Council's 2019 Midterm Report](../pdfs/2019-08-30_UN-Security-Council_s-2019-691.pdf) included:

> With regard to laundering the proceeds of attacks through cryptocurrency, the worldwide WannaCry ransomware attacks in May 2017, which affected more than 200,000 computers in 150 countries, demanded ransom payments in the Bitcoin cryptocurrency. A Member State investigation found that the cryptocurrency obtained through WannaCry malware had been laundered through multiple virtual currencies and multiple jurisdictions to obfuscate transactions.

> Bitcoin ransom payments made by victims of WannaCry were transferred from a Bitcoin wallet through cryptocurrency exchanges and ultimately converted to Monero, another cryptocurrency, using a Swiss-based cryptocurrency exchange called ShapeShift.35 Monero is an anonymity-enhanced virtual currency and therefore more difficult to trace than standard cryptocurrencies such as Bitcoin, Litecoin or Ethereum, which prolongs attribution. The proceeds of the third attack on Bithumb in June 2018 were transferred through YoBit.36 By August 2018, less than two months after the attack, the funds were sent to YoBit in a complex series of hundreds of transactions with the aim of converting and cashing out the entirety of the stolen cryptocurrency (as opposed to spending the acquired cryptocurrency directly on goods and services). The above-mentioned cases show a clear evolution from the earlier Democratic People’s Republic of Korea cyberattack on the customers of a Republic of Korea online shopping mall, Interpark, which was designed to generate foreign currency.


## Onchain


- On August 3, 2017, the ransom payments from the victims of the WannaCry Version 2 ransomware were transferred from the original Bitcoin addresses to other cryptocurrency addresses in a series of transactions. 

- As with the laundering of the ransoms associated with Version 1, following the Version 2 ransoms being sent to currency exchanges, the funds were converted to Monero. 

- At least some of those transfers used IP addresses that have been identified as exit nodes for the TOR network, and used the same browser UserAgent string, “Mozilla/5.0 (Windows NT 6.1; rv:52.0) Gecko/20100101 Firefox/52.0.”

- The "Wannacry 2.0 peeling" wallet was emptied on August 4th at 12:50 UTC with its last transaction to Changelly.

Ransoms paid by victims of WannaCry Version 1 were paid into Bitcoin wallets. On July 20, 2017, a series of transactions occurred that moved all of the ransom payment proceeds from the Bitcoin wallets associated with WannaCry Version 1. After the funds were sent to a currency exchange, the funds were converted to Monero, another cryptocurrency. At least some of the transactions occurred from five IP addresses that have been identified as exit nodes for the TOR network,35 and used the same browser User-Agent string “Mozilla/5.0 (Windows NT 6.1.; rv:52.0.) Gecko/20100101 Firefox/52.0.”

As with Version 1, ransoms paid by victims of WannaCry Version 2 were also paid into Bitcoin wallets. Estimates as of early-August 2017 indicate that approximately 330 victims paid the ransom demanded by WannaCry Version 2 totaling over $140,000. On August 3, 2017, the ransom payments from the victims of the WannaCry Version 2 ransomware were transferred from the original Bitcoin addresses to other cryptocurrency addresses in a series of transactions. As with the laundering of the ransoms associated with Version 1, following the Version 2 ransoms being sent to currency exchanges, the funds were converted to Monero. At least some of those transfers used IP addresses that have been identified as exit nodes for the TOR network, and used the same browser User- Agent string, “Mozilla/5.0 (Windows NT 6.1; rv:52.0) Gecko/20100101 Firefox/52.0.”



## URLs

- https://medium.com/@nbax/tracing-the-wannacry-2-0-monero-transactions-d8c1e5129dc1
- https://money.cnn.com/2017/08/03/technology/wannacry-bitcoin-ransom-moved/index.html
- https://securelist.com/wannacry-and-lazarus-group-the-missing-link/78431/
- https://bloomberg.com/news/articles/2017-12-19/u-s-blames-north-korea-for-cowardly-wannacry-cyberattack
- https://cbsnews.com/news/wannacry-ransomware-attacks-wannacry-virus-losses/
- https://cnbc.com/2017/05/23/symantec-says-highly-likely-north-korea-group-behind-ransomware-attacks.html
- https://cnbc.com/2017/08/03/hackers-havecashed-out-on-143000-of-Bitcoin-from-the-massive-wannacry-ransomware-attack.html
- https://eyerys.com/articles/timeline/wannacry-infecting-more-230000-computers-99-countries#event-a-href-articles-timeline-namewreck-exposes-hundreds-millions-iot-devices-security-risks039-name-wreck039-exposes-hundreds-of-millions-of-iot-devices-to-security-risks-a
- https://fortinet.com/blog/threat-research/wannacry-evolving-history-from-beta-to-2-0
- https://justice.gov/opa/pr/north-korean-regime-backed-programmer-charged-conspiracy-conduct-multiple-cyber-attacks-and
- https://justice.gov/opa/pr/three-north-korean-military-hackers-indicted-wide-ranging-scheme-commit-cyberattacks-and
- https://justice.gov/opa/press-release/file/1367701/download
- https://malwaretech.com/2017/05/how-to-accidentally-stop-a-global-cyber-attacks.html
- https://nao.org.uk/report/investigation-wannacry-cyber-attack-and-the-nhs/
- https://securitycouncilreport.org/atf/cf/%7B65BFCF9B-6D27-4E9C-8CD3-CF6E4FF96FF9%7D/S_2019_691.pdf
- https://technologyreview.com/2020/01/24/276082/lazarus-group-dragonex-chainalysis/ 
- https://theatlantic.com/technology/archive/2017/05/shadow-brokers/527778/
- https://whitehouse.gov/briefings-statements/press-briefing-on-the-attribution-of-the-wannacry-malware-attack-to-north-korea-121917/
- https://wired.com/story/confessions-marcus-hutchins-hacker-who-saved-the-internet/
- https://wsj.com/articles/u-s-preparing-cases-linking-north-korea-to-theft-at-n-y-fed1490215094.
- Page 106 [US v PARK JIN HYOK (June 2018)](https://justice.gov/opa/press-release/file/1092091/download)
- Page 29 of [UN Security Council's North Korea 2019 Midterm Report](../pdfs/2019-08-30_UN-Security-Council_s-2019-691.pdf)
