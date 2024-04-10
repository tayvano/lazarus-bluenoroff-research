# 3CX 

Date:: April 20, 2023

DPRK Malware Breach Was a Double Supply Chain Compromise

## Details

from https://riskybiznews.substack.com/p/risky-biz-news-north-korean-hackers

In March, hackers compromised 3CX’s desktop applications for Windows and macOS and bundled them with malware. As a result, customers of 3CX inadvertentl  downloaded malicious versions of the company’s voice- and video-calling software. Using the malicious versions of the software, the attackers were able to download and run arbitrary code on victim machines. This supply chain attack114 was the result of a previous supply chain attack on Trading Technologies, a financial software firm – a rare example of how a single perpetrator used one software supply chain attack to carry out another downstream. Targets included critical infrastructure in the energy sector. Cybersecurity companies have attributed this attack to the Lazarus Group.

A threat actor has compromised VoIP software development company 3CX and has trojanized its macOS and Windows desktop clients with malware.

The incident was discovered by cybersecurity firm [CrowdStrike](https://www.crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaign-targeting-3cxdesktopapp-customers/), and the company believes this may be the work of a North Korean state actor tracked as [Labyrinth Chollima](https://www.crowdstrike.com/adversaries/labyrinth-chollima/), also known as the Lazarus Group or Hidden Cobra.

Current evidence suggests the group infiltrated the company months before and hid malware in the company's macOS and Windows desktop clients around the start of the month. Customers who downloaded the apps were infected. The malware was also installed on some systems via the app's built-in updating feature—if this was enabled.

The incident is as bad as it gets, primarily because of the popularity of 3CX solutions.

The company's products include hosted and on-premise telephony VoIP IPBX servers. Employees in companies with 3CX VoIP IPBX servers can either use a VoIP phone or install the 3CX softphone on their devices to make and receive calls or host video conferences via a desktop or mobile app. It's these macOS and Windows desktop apps that were trojanized.

It's unclear how many users downloaded the trojanized desktop clients or how many received the malicious update for existing clients, but 3CX's customer base is huge. The company claims on its website to serve more than 600,000 companies and more than 12 million daily users. Per its [website](https://www.3cx.com/company/customers/), 3CX serves some of today's largest corporations.

A [Shodan search](https://www.shodan.io/search?query=http.favicon.hash%3A970132176) returns more than 245,000 3CX VoIP IPBX servers, just to give you an idea of how popular the 3CX system is.

As for 3CX, well, it's not good. At all. First, they didn't detect the intrusion for months. Second, when several antivirus products started detecting their clients as malicious, they repeatedly claimed it was just false positives, over and over again, without investigating further. When 4-5 different vendors see the same thing, it's probably a indicator you should look at your app. Third, some customers said that when they went to 3CX's customer support with CrowdStrike's findings, they were asked to "[open a support ticket at £75 per incident](https://archive.ph/DkWSh#selection-2579.99-2579.140)." That's just... not what people wanted to hear.



## Links

- https://www.crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaigntargeting-3cxdesktopapp-customers
- https://www.welivesecurity.com/2023/04/20/linux-malwarestrengthens-links-lazarus-3cx-supply-chain-attack
- https://www.mandiant.com/resources/blog/3cx-softwaresupply-chain-compromise
- https://symantec-enterprise-blogs.security.com/blogs/threatintelligence/xtrader-3cx-supply-chain
- https://riskybiznews.substack.com/p/risky-biz-news-north-korean-hackers
- https://www.sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/
- https://objective-see.org/blog/blog_0x73.html
- https://www.volexity.com/blog/2023/03/30/3cx-supply-chain-compromise-leads-to-iconic-incident/
- https://news.sophos.com/en-us/2023/03/29/3cx-dll-sideloading-attack/
- https://www.trendmicro.com/de_de/research/23/c/information-on-attacks-involving-3cx-desktop-app.html
- https://www.huntress.com/blog/3cx-voip-software-compromise-supply-chain-threats