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

> “Lazarus is a rather unusual nation state sponsored group. On one hand, as many other similar groups do, it focuses on conducting cyberespionage or sabotage operations. Yet on the other hand, it has also been found to influence attacks that are clearly aimed at stealing money. The latter is quite unique for such a high profile threat actor because generally, other actors do not have financial motivations in their operations” - Konstantin Zykov security researcher, Kaspersky Global Research and Analysis Team.

> “The vast amount of samples we found demonstrate how Lazarus is one of the most active APT groups, constantly developing and evolving threats in a bid to affect large-scale industries. Their successful execution of these RATs proves that even when a threat seems to disappear, it can be resurrected in a different guise to attack new targets.

> We have discovered an asset-backed crypto scam called Marine Chain operated by North Korea enablers in Singapore & at least one other scam coin called HOLD/HUZU

> In December 2019, Lazarus Group had 470 separate cryptocurrency addresses at its top 20 exchanges that had received at least $1,000 worth of stolen cryptocurrency. By the end of December 2020, that number had risen to 2,078. This suggests that Lazarus Group is spreading its funds around more to mitigate the risk of any one address being identified and frozen. It also fits a pattern of adaptability on the part of Lazarus Group — each year, their money laundering strategy changes as services improve their security efforts.




# The Many Names of Lazarus

- The Lazarus Group naming and attribution originally stems from the February 2016 Operation Blockbuster report on the 2014 Sony Pictures Hack.

- As security researchers continued to analyze earlier and ongoing cyber attacks, it became clear that perpetrators shared code, infrastructure and malicious tools but also appeared to have different motivations or mandates.

- This is partially due to the fact that the group's malware and tactics change, making definitive attribution difficult. They obfuscate their trail and leave no trace behind. Often a known group will be called by a certain name for months or years, only later to be definitively linked to Lazarus.

- This is also partially due to the fact that there's not one room with 1000 North Korean hackers in it. There are actually different teams with different mandates and operating under different departments and levels of government. Different groups work on different hacks, have different methods, different motivations, etc.

- Generally, today, you should assume the moniker Lazarus refers very broadly to any cyber / threat activity attributed to North Korea unless explicitly specified otherwise.

- Increasingly, sec researchers and governments have been using "DPRK" instead of "Lazarus", possibly to avoid confusion around attribution to a specific group or imply a linkage to specific malware/iocs/ttps. Or perhaps bc its just shorter.


## Mandiant's Current Naming Conventions

Source: https://www.mandiant.com/resources/blog/north-korea-cyber-structure-alignment-2023

Mandiant maintains, tracks, and reports campaign history on North Korea’s offensive cyber operations. The following are the most prevalent groups Mandiant currently tracks, along with a brief summary of each threat group, and primary targeting priority/priorities. Note: The groups that follow are referred to with their Mandiant designations (UNC numbers) alongside the names that have been used publicly to identify activity we attribute to the underlying group. While we believe that these definitions are largely congruent, differences in visibility and analytic tradecraft mean that an exact match is unlikely. 




### [Andariel](https://global.ahnlab.com/global/upload/download/techreport/%5BAhnLab%5DAndariel_a_Subgroup_of_Lazarus%20\(3\).pdf) / UNC614

- This actor targets foreign businesses, government agencies, financial services infrastructure, private corporations, and the defense industry. UNC614 also engages in cyber crime as an extra source of income to fund their operations, including the [ransoming of hospitals](https://advantage.mandiant.com/reports/22-00021780), using their own ransomware malware dubbed [MAUI](https://advantage.mandiant.com/reports/22-00019069). However, their primary focus is on targeting military and government personnel. 
- This cyber group stands apart from the other DPRK aligned groups and typically does not fall into the blending and targeting that the others may do. Some groups have espionage and financial focuses, but Andariel is tasked to acquire information to “build” the weapons of mass destruction or research and development programs in other targeted fields, like pharmaceuticals. 
- The targeting trends, such as nuclear, aerospace, high heat molds, etc. and overall successful compromises of this actor make it quite possibly the scariest of all the DPRK affiliated groups.
- Primary targeting: Defense, Aerospace, Healthcare (when self-funding operations), Nuclear




### [TEMP.Hermit](https://thehackernews.com/2023/03/north-korean-unc2970-hackers-expands.html)

- TEMP.Hermit, is an actor that has been active since at least 2013. Their operations since that time are representative of Pyongyang's efforts to collect strategic intelligence to benefit North Korean interests. This actor targets government, defense, telecommunications, and financial institutions worldwide and the term “Lazarus Group” refers most often to this cluster of activities. AppleJeus maintains overlap with this organization, but TEMP.Hermit’s targeting continues to focus on espionage related activities and not cryptocurrency as its primary focus.
- Primary targeting: Government, Defense, Telecommunications




### [AppleJeus](https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-048a) / UNC1720

- A threat group that has been active since at least 2018. It is assessed to primarily target the cryptocurrency industry with the goal of stealing digital assets to fund the regime’s priorities. The group uses a variety of tactics, including spear-phishing emails and fake cryptocurrency trading software, to infiltrate target systems and steal cryptocurrency. Like TraderTraitor, this crypto-focused group appeared to emerge after the notoriety that came with the Bangladesh heist and issues with stealing and laundering traditional currency. This group’s tools overlap with TEMP.Hermit, but is not focused on the same targeting profiles, potentially indicating shared resources.
- Primary targeting: Cryptocurrency




### [CryptoCore](https://www.clearskysec.com/cryptocore-lazarus-attribution/) / UNC1069

- A threat actor that has been active since at least 2018. UNC1069 is a cryptocurrency focused group that may include individuals or units previously tracked as APT38, and while it has minor overlaps with APT43, we belive it is distinct. UNC1069 has targeted a variety of financial services firms and cryptocurrency exchanges, commonly employing spear-phishing techniques that result in LONEJOGGER malware infections. This organization appears to maintain a revenue generation priority, like its overarching APT38 subunits, however on a much smaller financial scale.
- Primary Targeting: Financials, Cryptocurrency 




### [TraderTraitor](https://www.cisa.gov/news-events/cybersecurity-advisories/aa22-108a) / UNC4899

- TraderTraitor targets blockchain companies through spear-phishing messages. The group sends these messages to employees, particularly those in system administration or software development roles, on various communication platforms, intended to gain access to these start-up and high-tech companies. TraderTraitor may be the work of operators previously responsible for APT38 activity.
- Primary targeting: Cryptocurrency




### [IT Workers](https://ofac.treasury.gov/media/923126/download?inline)

- DPRK’s IT Workers, which according the the US Treasury department, primarily fall under the KWP’s Munitions Industry Department, are made up of thousands of highly skilled IT workers from North Korea. They are reportedly deployed both domestically and abroad to generate revenue and finance the country's weapons of mass destruction and ballistic missile programs. These workers acquire freelance contracts from clients around the world and sometimes pretend to be based in the US or other countries to secure employment. Although they mainly engage in legitimate IT work, they have misused their access to enable malicious cyber intrusions*carried out by North Korea.




### [APT37](https://www.mandiant.com/resources/blog/apt37-overlooked-north-korean-actor)

- APT37's assessed primary mission is covert intelligence gathering in support of DPRK's strategic military, political, and economic interests. The group has been observed targeting a wide range of industries, primarily in South Korea. This organization is most closely aligned with the efforts of the MSS and its overarching cyber activities highlight the monitoring of defectors abroad and foreign elements interacting with DPRK.
- Primary targeting: Defectors, Governments




### [APT38](https://www.mandiant.com/resources/blog/apt38-details-on-new-north-korean-regime-backed-threat-group)

- APT38 is a financially motivated group, known for significant financial compromises and its use of destructive malware against financial institutions. The group has been attributed to sophisticated compromises targeting [Interbank Fund Transfer Systems](https://www.mandiant.com/resources/blog/apt38-details-on-new-north-korean-regime-backed-threat-group) to steal millions of dollars at a time across multiple countries worldwide. 
- Current activity from this group is conducted by associated subgroups. Mandiant identified a long hiatus of activity attributed to APT38, which may be indicative of modifications and regrouping of APT38 operators to other units aligned with new priorities and needs.
- Primary targeting: Financials




### [APT43](https://www.mandiant.com/resources/blog/apt43-north-korea-cybercrime-espionage)

- APT43 is a prolific cyber operator that directly supports intelligence gathering interests of the North Korean regime. The group combines moderately sophisticated technical capabilities with aggressive social engineering tactics, especially against South Korean and US-based government organizations, academics, and think tanks focused on Korean peninsula geopolitical issues. 
This organization acts as an intelligence arm and seeming embassy replacement for the RGB and DPRK leadership writ large.
- Primary targeting: Governments, Nuclear, Foreign Relations




### Hybrid Operations & UNC2226

- Mandiant has observed operations that include tactics and tools from multiple groups, which suggests that in certain cases, operations may be undertaken by multiple groups that fluidly perform ad hoc tasks in support of another group, or due to temporary tasking. This is consistent with public reporting that identified a [group](https://www.dailynk.com/english/kim-jong-un-directly-handling-results-new-covid-19-hacking-organization-work/) that aligns with an alleged RGB Bureau, designated ‘325’, which was publicly announced in January 2021, when the structure of the RGB likely shifted in response to the COVID-19 pandemic.
- Mandiant assesses that UNC2226 is one of the collections of activity supporting the aforementioned mission. UNC2226, like other seemingly ad hoc created efforts, appears to have changed or even expanded targeting to fulfill intelligence gathering efforts. Other clusters, such as UNC3782, have a similar composition and are focused on cryptocurrency theft among other seemingly ad hoc tasks.
- The operations initially appeared to focus almost exclusively on intelligence gathering operations against COVID-19 research and vaccine development/manufacturing organizations. Over time, Mandiant perceived these operations shift from strictly COVID-19 efforts to the targeting of defectors, defense and governments, bloggers, media, cryptocurrency services, and financial institutions. 


