# 3CX 

Date:: April 20, 2023

DPRK Malware Breach Was a Double Supply Chain Compromise

## Details

from https://riskybiznews.substack.com/p/risky-biz-news-north-korean-hackers

In March, hackers compromised 3CX’s desktop applications for Windows and macOS and bundled them with malware. As a result, customers of 3CX inadvertentl  downloaded malicious versions of the company’s voice- and video-calling software. Using the malicious versions of the software, the attackers were able to download and run arbitrary code on victim machines. This supply chain attack114 was the result of a previous supply chain attack on Trading Technologies, a financial software firm – a rare example of how a single perpetrator used one software supply chain attack to carry out another downstream. Targets included critical infrastructure in the energy sector. Cybersecurity companies have attributed this attack to the Lazarus Group.

A threat actor has compromised VoIP software development company 3CX and has trojanized its macOS and Windows desktop clients with malware.

The incident was discovered by cybersecurity firm [CrowdStrike](https://crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaign-targeting-3cxdesktopapp-customers/), and the company believes this may be the work of a North Korean state actor tracked as Labyrinth Chollima, also known as the Lazarus Group or Hidden Cobra.

Current evidence suggests the group infiltrated the company months before and hid malware in the company's macOS and Windows desktop clients around the start of the month. Customers who downloaded the apps were infected. The malware was also installed on some systems via the app's built-in updating feature—if this was enabled.

The incident is as bad as it gets, primarily because of the popularity of 3CX solutions.

The company's products include hosted and on-premise telephony VoIP IPBX servers. Employees in companies with 3CX VoIP IPBX servers can either use a VoIP phone or install the 3CX softphone on their devices to make and receive calls or host video conferences via a desktop or mobile app. It's these macOS and Windows desktop apps that were trojanized.

It's unclear how many users downloaded the trojanized desktop clients or how many received the malicious update for existing clients, but 3CX's customer base is huge. The company claims on its website to serve more than 600,000 companies and more than 12 million daily users. Per its [website](https://3ctwitter.com/company/customers/), 3CX serves some of today's largest corporations.

A [Shodan search](https://shodan.io/search?query=http.favicon.hash%3A970132176) returns more than 245,000 3CX VoIP IPBX servers, just to give you an idea of how popular the 3CX system is.

As for 3CX, well, it's not good. At all. First, they didn't detect the intrusion for months. Second, when several antivirus products started detecting their clients as malicious, they repeatedly claimed it was just false positives, over and over again, without investigating further. When 4-5 different vendors see the same thing, it's probably a indicator you should look at your app. Third, some customers said that when they went to 3CX's customer support with CrowdStrike's findings, they were asked to "[open a support ticket at £75 per incident](https://archive.ph/DkWSh#selection-2579.99-2579.140)." That's just... not what people wanted to hear.

In late March 2023, 3CX disclosed that its desktop applications for both Windows and macOS were compromised with malicious code that gave attackers the ability to download and run code on all machines where the app was installed. 3CX says it has more than 600,000 customers and 12 million users in a broad range of industries, including aerospace, healthcare and hospitality.

3CX hired incident response firm Mandiant, which released a report on Wednesday that said the compromise began in 2022 when a 3CX employee installed a malware-laced software package distributed via an earlier software supply chain compromise that began with a tampered installer for X_TRADER, a software package provided by Trading Technologies.
This is the first time Mandiant has seen a software supply chain attack lead to another software supply chain attack


## Links
- https://crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaign-targeting-3cxdesktopapp-customers
- https://welivesecurity.com/2023/04/20/linux-malwarestrengthens-links-lazarus-3cx-supply-chain-attack
- https://mandiant.com/resources/blog/3cx-softwaresupply-chain-compromise
- https://symantec-enterprise-blogs.security.com/blogs/threatintelligence/xtrader-3cx-supply-chain
- https://riskybiznews.substack.com/p/risky-biz-news-north-korean-hackers
- https://sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack
- https://objective-see.org/blog/blog_0x73.html
- https://volexity.com/blog/2023/03/30/3cx-supply-chain-compromise-leads-to-iconic-incident
- https://news.sophos.com/en-us/2023/03/29/3cx-dll-sideloading-attack
- https://trendmicro.com/de_de/research/23/c/information-on-attacks-involving-3cx-desktop-app.html
- https://huntress.com/blog/3cx-voip-software-compromise-supply-chain-threats
- https://welivesecurity.com/2023/04/20/linux-malware-strengthens-links-lazarus-3cx-supply-chain-attack
- https://reddit.com/r/crowdstrike/comments/125r3uu/20230329_situational_awareness_crowdstrike
- https://crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaign-targeting-3cxdesktopapp-customers
- https://blog.checkpoint.com/2023/03/29/3cxdesktop-app-trojanizes-in-a-supply-chain-attack-check-point-customers-remain-protected
- https://symantec-enterprise-blogs.security.com/blogs/threat-intelligence/3cx-supply-chain-attack
- https://trendmicro.com/fr_fr/research/23/c/information-on-attacks-involving-3cx-desktop-app.html
- https://twitter.com/patrickwardle/status/1641294247877021696
- https://elastic.co/kr/security-labs/elastic-users-protected-from-suddenicon-supply-chain-attack
- https://twitter.com/dez_/status/1641459372478935040
- https://cisa.gov/news-events/cybersecurity-advisories/aa21-048a
- https://cybersecuritydive.com/news/3cx-mandiant-investigate-supply-chain-attack/646543
- https://crn.com/news/security/3cx-supply-chain-attack-big-questions-remain
- https://securelist.com/gopuram-backdoor-deployed-through-3cx-supply-chain-attack/109344
- https://securelist.com/operation-applejeus-sequel/95596
- https://3ctwitter.com/blog/news/mandiant-initial-results
- https://krebsonsecurity.com/2023/04/3cx-breach-was-a-double-supply-chain-compromise
- https://explore.avertium.com/resource/lazarus-and-the-3cx-double-supply-chain-attack
- https://sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/