# Background


- Lazarus Group is a threat group that has been attributed to the North Korean government and has been active since at least 2007.

- They are state-sponsored cyber actors—specifically hackers, cryptologists, and software developers—who conduct cyber espionage, politically-motivated operations, and cyber-enabled theft. 

- Their efforts are incredibly diverse but stereotypically they are known for targeting foreign media companies, financial institutions worldwide, and cryptocurrency exchanges. Specifically their disruptive DDoS and wiper attacks against South Korean and US (Sony and more), extortion campaigns via ransomware (WannaCry and more), hacks of banks via SWIFT (Bangledesh Bank Heist and so many more), hacks of CEX's (sooooo mannnnyyy CEX's).

- The US Army and other intelligence believe there are ~7000 hackers who make up the various cyber units generally referred to as "Lazarus". They are are extreme workaholics—working 15 hours, 6 days a week—probably the most hard-working APT-group among all known. They typically start at midnight o'clock sharp UTC with a break around 3pm. They consistently work Saturday. While it's more rare to see attacks initiated in the middle of the night Korean time or on a Sunday, it's not unheard of, especially for a big payday or if they know that is when a target is going to be offline (on a plane, on vacation, etc)

### They develop and deploy a wide range of malware tools

- ...and have resources that allow for development of custom malware tools for extensive, targeted, and coordinated attacks, including long periods of reconnaissance. 

### They are sophisticated as fuck. 

- This requires strict organization and control at all stages of operation. It's not usually found in the cybercriminal world. In most infiltrations of banks and cryptocurrency companies, they prefer to silently integrate into running processes without breaking them. Their invasions aim to be invisible and leave little or no trace. 

### They are financially motivated. 

- Some hackers are in it for the clout and, while larger paydays result in more clout, the money is not the end game. Nation-state actors' motivations are usually aligned with their broader military, political and intelligence operations and their cyber attacks are used as a means of information collection, sabotage, disruption. North Korea is different.

### They evolve faster than most startups. 

- They have grown increasingly sophisticated over time and move to target the most profitable sectors or further their larger political efforts at a rapid pace. Their initial efforts shifted from disruptive DDoS/Wiper attacks->Bank Heists around 2014 and then from Bank Heists->CEX Hacks around 2017, likely in reaction to the explosion of value in the cryptocurrency industry. In 2018 and 2019 they experimented with various forms of crypto malware and crypotojacking mining of Bitcoin and Monero, but also returned to their previous efforts targeting banks and financial institutions, possibly due to the decreased profits in crypto. By 2021, they show a deep knowledge of the Ethereum, DeFi, and NFT space, attacking individual via a malicious version of MetaMask, using Uniswap to swap stolen tokens for ETH, and mixing their funds via Tornado Cash.

### Thorough, persistent, patient. 

- They will often hang out in a system for months on end, gathering intel or slowly increasingly the scope of their access. They reliably do such thorough reconnaissance that initial investigations and reports mistake the attacks for an inside job. In the 2016 Vietnam Bank Heist the malware was only properly investigated after the Bangladesh Bank Heist occurred months later. At least 5 of the cryptocurrency exchange hacks in 2017 and 2018 and the more recent 2022 Ronin Bridge Hack were, at least by some, suspected to be an inside job.

### Insane depth of knowledge of their target. 

- Their reconnaissance ensures they have a full understanding of how both the human and technology systems operate: what software is supported, when it operates, who is responsible for what, who will be out of the office for a local holiday, everything. In the Vietnamese case, they knew the bank used Foxit and replaced it with a fake version. They also knew the names of the printers. 

### Really, really, really good at spearphishing. 

- They very rarely spend time trying to hack the actual systems and instead craft tools to levy attacks via individuals, employees, or usability flaws of the systems or infrastructure. One element that appears consistently since 2007 is their use of spearphishing to deploy custom malware and gain initial access. Their emails—or increasingly messages sent via LinkedIn, Telegram, etc.—are designed to appear legitimate and are tailored and personalized for the intended recipient. They use their recon time to craft harder-to-detect messages that appear like totally normal interactions. Investigations have revealed initial intrusions stemming from an email forwarded by one colleague to another and in an email related to a matter that was currently being discussed between the two parties.

### Notorious for constantly tuning their malware. 

- The malware in each attack is usually compiled just before the attack happened and custom built for the target. Once they have access, especially when attacking financial systems, they often manipulate the existing system and existing software to do their bidding for them. For example, in one incident, they knew a target used MetaMask to access his tokens on his hardware wallet. They replaced his MetaMask with a malicious version that hid the fact he was not sending a few tokens to a friend, but all his NXM tokens to the attackers address. Ultimately, the target was the one who clicked the buttons that resulted in the theft.



# Interesting Quotes



> Lazarus is not just another APT actor The scale of Lazarus operations is shocking. It has been on a growth spike since 2011 and activities didn't disappear after Novetta published the results of its Operation Blockbuster research.

> All those hundreds of samples that were collected give the impression that Lazarus is operating a factory of malware, which produces new samples via multiple independent conveyors.  We have seen it using various code obfuscation techniques, rewriting its own algorithms, applying commercial software protectors, and using its own and underground packers. Lazarus knows the value of quality code, which is why we normally see rudimentary backdoors being pushed during the first stage of infection. 

> Burning those doesn't cause too much impact on the group. However, if the first stage backdoor reports an interesting infection it starts deploying more advanced code, carefully protecting it from accidental detection on disk.  The code is wrapped into a DLL loader or stored in an encrypted container, or maybe hidden in a binary encrypted registry value.  It usually comes with an installer that only the attackers can use, because they password protect it.  It guarantees that automated systems - be it public sandbox or a researcher's environment - will never see the real payload.  Most of the tools are designed to be disposable material that will be replaced with a new generation as soon as they are burnt. And then there will be newer, and newer, and newer versions. 

> Lazarus avoids reusing the same tools, the same code, and the same algorithms. "Keep morphing!" seems to be its internal motto.  Those rare cases when it is caught with the same tools are operational mistakes, because the group seems to be so large that one part doesn't know what the other is doing. 

> All this level of sophistication is something that is not generally found in the cybercriminal world.  It's something that requires strict organization and control at all stages of the operation.  That's why we think that Lazarus is not just another APT actor. 

> It has reverse engineering skills and spends time tearing apart legitimate software, implementing patches for SWIFT Alliance software, and finding ways and schemes to steal big money.  Its malware is different and the attackers aren't exactly soldiers that hit and run. Instead they prefer to make an execution trace to be able to reconstruct and quickly debug the problem.  They are field engineers that come when the ground is already cleared after the conquest of new lands. 

> One of Bluenoroff's favorite strategies is to silently integrate into running processes without breaking them.  From the perspective of the code we've seen it looks as if it is not exactly looking for hit and run solutions when it comes to money theft.  Its solutions are aimed at invisible theft without leaving a trace. Of course, attempts to move around millions of USD can hardly remain unnoticed but we believe that its malware might now be secretly deployed in many other places - and it doesn't trigger any serious alarms because it's much more quiet.

> We would like to note, that in all the observed attacks against banks that we have analyzed, servers used to connect to SWIFT didn't demonstrate or expose any specific vulnerability.  The attacks were focused on the banks’ infrastructure and staff, exploiting vulnerabilities in commonly used software or websites, bruteforcing passwords, using keyloggers and elevating privileges.  However, the design of inter-banking transactions using a bank's own server running SWIFT connected software suggests that there are personnel responsible for the administration and operation of the SWIFT connected server.  Sooner or later the attackers find these users, gain their necessary privileges and access the server connected to the SWIFT messaging platform.

> With administrative access to the platform, they can manipulate the software running on the system as they wish. 

> There is not much that can stop them, because from a technical perspective it may not differ from what authorized and qualified engineers do: starting and stopping services, patching software, or modifying databases. 

> To date, the Lazarus/Bluenoroff group has been one of the most successful in large scale operations against financial industry.  We believe that it will remain one of the biggest threats to the banking sector, finance and trading companies as well as casinos, for years to come.

— [Lazarus Under The Hood, 2017](https://securelist.com/lazarus-under-the-hood/77908/)




> “Lazarus is a rather unusual nation state sponsored group. On one hand, as many other similar groups do, it focuses on conducting cyberespionage or sabotage operations. Yet on the other hand, it has also been found to influence attacks that are clearly aimed at stealing money. The latter is quite unique for such a high profile threat actor because generally, other actors do not have financial motivations in their operations”

> “The vast amount of samples we found demonstrate how Lazarus is one of the most active APT groups, constantly developing and evolving threats in a bid to affect large-scale industries. Their successful execution of these RATs proves that even when a threat seems to disappear, it can be resurrected in a different guise to attack new targets.

- [Konstantin Zykov security researcher, Kaspersky Global Research and Analysis Team](https://usa.kaspersky.com/about/press-releases/dtrack-previously-unknown-spy-tool-hits-financial-institutions-and-research-centers)



> We have discovered an asset-backed crypto scam called Marine Chain operated by North Korea enablers in Singapore & at least one other scam coin called HOLD/HUZU

—[Shifting Patterns in Internet Use Reveal Adaptable and Innovative North Korean Ruling Elite, Recorded Future, 2018](https://www.recordedfuture.com/north-korea-internet-usage/)





> In December 2019, Lazarus Group had 470 separate cryptocurrency addresses at its top 20 exchanges that had received at least $1,000 worth of stolen cryptocurrency. By the end of December 2020, that number had risen to 2,078. This suggests that Lazarus Group is spreading its funds around more to mitigate the risk of any one address being identified and frozen. It also fits a pattern of adaptability on the part of Lazarus Group — each year, their money laundering strategy changes as services improve their security efforts.

—[The 2021 Crypto Crime Report, Chainalysis, 2021](https://safewayconsultoria.com/wp-content/uploads/2021/09/Chainalysis-Crypto-Crime-2021.pdf)

Note:

- Lazrus used over 3,248 distinct EVM addresses to launder Atomic Wallet between June 3, 2023—August 3, 2023

- They used over 1,000 addresses just for the Tornado Cash laundering of Poloniex on Ethereum in Spring 2024

