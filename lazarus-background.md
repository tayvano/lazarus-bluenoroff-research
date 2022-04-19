> “If the Internet is like a gun, cyberattacks are like atomic bombs.” – Kim Jon Il

> “Cyberwarfare is an all-purpose sword that guarantees the North Korean People’s Armed Forces ruthless striking capability, along with nuclear weapons and missiles.” – Kim Jong-un

# Really Good Links
    - The Incredible Rise of North Korea's Hacking Elite
        - https://www.newyorker.com/magazine/2021/04/26/the-incredible-rise-of-north-koreas-hacking-army
    - Tracking Internet Use Out of North Korea Reveal The Adaptable and Innovative Ruling Elite
        - https://www.recordedfuture.com/north-korea-internet-usage/
    - Organizational Map of DPRK
        - https://www.mandiant.com/resources/mapping-dprk-groups-to-government
    - Kim Jong Un is directly handling results of new COVID-19 hacking organization's work
        - https://www.dailynk.com/english/kim-jong-un-directly-handling-results-new-covid-19-hacking-organization-work/
    - Lazarus Group Deep Dive 1
        - https://blog.bushidotoken.net/2020/02/deep-dive-lazarus-group.html?m=1
    - Lazarus Group Deep Dive 2
        - https://blog.bushidotoken.net/2021/08/the-lazarus-heist-where-are-they-now.html?m=1
    - Lazarus: Under The Hood
        - https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07180244/Lazarus_Under_The_Hood_PDF_final.pdf
    - Spotlight On Lazarus
        - https://www.cybersecurity-help.cz/blog/2511.html
    - The All-Purpose Sword: North Korea’s Cyber Operations and Strategies (2019)
        - https://ccdcoe.org/uploads/2019/06/Art_08_The-All-Purpose-Sword.pdf
    - US Army's Report on North Korean Tactics (2020)
        - https://irp.fas.org/doddir/army/atp7-100-2.pdf
        - cmd f for cyber, Bureau 121, computer warfare
    - CISA's Guidance on the North Korean Cyber Threat (2020)
        - https://www.cisa.gov/uscert/ncas/alerts/aa20-106a
    - North Korea's Military Power
        - https://www.dia.mil/Portals/110/Documents/News/North_Korea_Military_Power.pdf


# Background / General Analysis
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
    > We would like to note, that in all the observed attacks against banks that we have analyzed, servers used to connect to SWIFT didn't demonstrate or expose any specific vulnerability.  The attacks were focused on the banks’ infrastructure and staff, exploiting vulnerabilities in commonly used software or websites, bruteforcing passwords, using keyloggers and elevating privileges.  However, the design of inter-banking transactions using a bank's own server running SWIFT connected software suggests that there are personnel responsible for the administration and operation of the SWIFT connected server.  **Sooner or later the attackers find these users, gain their necessary privileges and access the server connected to the SWIFT messaging platform.**
    > With administrative access to the platform, they can manipulate the software running on the system as they wish. 
    > There is not much that can stop them, because from a technical perspective it may not differ from what authorized and qualified engineers do: starting and stopping services, patching software, or modifying databases. 
    > To date, the Lazarus/Bluenoroff group has been one of the most successful in large scale operations against financial industry.  We believe that it will remain one of the biggest threats to the banking sector, finance and trading companies as well as casinos, for years to come.
    > “Lazarus is a rather unusual nation state sponsored group. On one hand, as many other similar groups do, it focuses on conducting cyberespionage or sabotage operations. Yet on the other hand, it has also been found to influence attacks that are clearly aimed at stealing money. The latter is quite unique for such a high profile threat actor because generally, other actors do not have financial motivations in their operations” - Konstantin Zykov security researcher, Kaspersky Global Research and Analysis Team.
    > “The vast amount of samples we found demonstrate how Lazarus is one of the most active APT groups, constantly developing and evolving threats in a bid to affect large-scale industries. Their successful execution of these RATs proves that even when a threat seems to disappear, it can be resurrected in a different guise to attack new targets.
    > We have discovered an asset-backed crypto scam called Marine Chain operated by North Korea enablers in Singapore & at least one other scam coin called HOLD/HUZU
    > In December 2019, Lazarus Group had 470 separate cryptocurrency addresses at its top 20 exchanges that had received at least $1,000 worth of stolen cryptocurrency. By the end of December 2020, that number had risen to 2,078. This suggests that Lazarus Group is spreading its funds around more to mitigate the risk of any one address being identified and frozen. It also fits a pattern of adaptability on the part of Lazarus Group — each year, their money laundering strategy changes as services improve their security efforts.


# The Lazarus Group is called by many, many names
    - The Lazarus Group naming and attribution originally stems from the February 2016 Operation Blockbuster report on the 2014 Sony Pictures Hack.
    - As security researchers continued to analyze earlier and ongoing cyber attacks, it became clear that perpetrators shared code, infrastructure and malicious tools but also appeared to have different motivations or mandates.
    - This is partially due to the fact that the group's malware and tactics change, making definitive attribution difficult. They obfuscate their trail and leave no trace behind. Often a known group will be called by a certain name for months or years, only later to be definitively linked to Lazarus.
    - This is also partially due to the fact that there's not one room with 1000 North Korean hackers in it. There are actually different teams with different mandates and operating under different departments and levels of government. Different groups work on different hacks, have different methods, different motivations, etc.
    - Generally, today, in 2022, you should assume the moniker Lazarus Group refers very broadly to any cyber / threat activity attributed to North Korea unless explicitly specified otherwise.
    - The financially-motivated group responsible for the attacks on banks, financial companies, trading companies, casinos and cryptocurrency exchanges became known as`Bluenoroff` and is either a subgroup of Lazarus or a group originally spun out of Lazarus.
    ### Outlining the Specific Naming Conventions by Specific Folks
        - Kaspersky - Lazarus Bluenoroff
            - refers to the original perpetrators of Operations Troy / Sony Pictures / Operations Dark Seoul as Lazarus. While investigating the SWIFT Heists they linked attack systems and lateral movement tools to Lazarus but noted that Lazarus was still engaged in cyberespionage and cybersabotage campaigns at the time. They began referring to the group that attacked banks and financial manipulations as Bluenoroff, a subgroup or separate but closely affiliated group, possibly spun out and comprised of members of the original Lazarus group.
            - https://media.kasperskycontenthub.com/wp-content/uploads/sites/43/2018/03/07180244/Lazarus_Under_The_Hood_PDF_final.pdf
        - U.S. DoJ, US Treasury, OFAC, FBI: HIDDEN COBRA BeagleBoyz
            - Generally refer to all malicious cyber activity by the North Korean government as HIDDEN COBRA and further specify subgroups on an as-needed basis. For example: "To differentiate methods from other North Korean malicious cyber activity, the U.S. Government refers to this team as BeagleBoyz, who represent a subset of HIDDEN COBRA activity."
        - US Army - Bureau 121 Andarial Bluenoroff Lazarus
            - Bureau 121 to describe the higher level organization of ~6,000 members and Andarial, Bluenoroff, and Lazarus to describe the subordinate units responsible for `reconnaissance`, `financial cybercrime`, and `social chaos`, respectively.
        - Mandiant - Lab 110 Andarial APT37 APT38 TEMP.Hermit Bureau 325 CERIUM
            - In 2022, private security researcher group **Mandiant**, introduced Lab 110, an expanded and reorganized version of "Bureau 121" with Andarial, APT38, and TEMP.Hermit who focus on `targeting military and government personnel`, `financial compromises via destructive malware`, and `collecting strategic intelligence`, respectively.
            - In this same report by **Mandiant**, they explore Bureau 325 which was formed in response to COVID-19. This group likely pulled top members from Bureau 121, bringing their tools, fingerprints, and patterns with them. Their initial mandate, and now one of their sub-units, is the COVID-19-focused unit CERIUM. More recently this group has targeted defectors, defense and governments, bloggers, media, cryptocurrency services, and financial institutions
    ### List of Names
        - RGB -> 3rd Bureau -> **Bureau 121 / Lab 110** (broadly "Lazarus")
            - Bureau 121 aka Lab 110 aka (broadly) "Lazarus"
            - Open-source [reporting](https://risky.biz/laz/) often uses the Lazarus Group title as an umbrella term, referring to numerous clusters that we track separately.
            - E-4. Most EW and cyberspace warfare operations take place within the Cyber Warfare Guidance Unit, more commonly known as Bureau 121, with four subordinate units below Bureau 121: The Andarial Group, The Bluenoroff Group, The Lazarus Group, Electronic Warfare Jamming Regiment. 
            - E-4. There are over 6,000 members in Bureau 121, many of them operating from other countries, such as Belarus, China, India, Malaysia, and Russia. North Korean computer hackers have even been able to access secure systems and steal South Korean war plans.
            - Lab 110 is likely an expanded and reorganized version of "Bureau 121" often noted as North Korea's primary hacking unit.
            - Lab 110 contains some elements that are most closely aligned with the organization, publicly reported as "Lazarus Group."
            - Lab 110 has operated out of front companies historically based in northeast China, among other locations. Previously [identified](https://int.nyt.com/data/documenthelper/274-park-jin-hyo-complaint/7b40e5ed5b185f141e1a/optimized/full.pdf#page=1) [fronts](https://intelligence.fireeye.com/reports/18-00014948) include Chosun Expo Joint Venture in Dalian and Chosun Baeksul Trading Company in Shenyang. 
            - https://ccdcoe.org/uploads/2019/06/Art_08_The-All-Purpose-Sword.pdf
        - RGB -> 3rd Bureau -> Bureau 121 / Lab 110 -> **The Andariel Group**
            - Silent Chollima == Dark Seoul == Rifle == Wassonite
            - Another subgroup, Andarial, is active only in South Korea and seeks to perform various attacks that focus on stealing confidential data from the military and defence industries.
            - Is focused on targeting South Korean organizations and businesses, as well as military agencies, defense industries, political organizations, security companies, ICT companies, and energy research institutes, ATMs, banks, travel agencies, cryptocurrency exchanges, and online gambling users.
            - The group was observed using a variety of tools and tactics in their operations, such as DDoS attacks and wipers, misdirection techniques (campaigns disguised as hacktivist attacks, or a “false flag” scenario), spear-phishing, supply-chain attacks, watering hole attacks exploiting Active-X vulnerabilities, exploitation of vulnerabilities in security and IT asset management systems.
            - Andariel’s malware arsenal includes well-known backdoors, such as Aryan and Gh0st RAT, and in-house developed backdoors like Andarat, Andaratm, Rifdoor, and Phandoor.
            - 1,600 members (+/-) whose mission is to gather information by conducting reconnaissance on enemy computer systems and creating an initial assessment of the network’s vulnerabilities. This group maps the enemy network for potential attack.
            - Andarial was responsible for causing server errors in the 3.20 (DarkSeoul) attack on 20 March 2013, and since the second half of 2016 it has been more focused on attacking the financial industry. 
            - Focuses its operations on foreign businesses, government agencies, financial services infrastructure, private corporations, and businesses, as well as the defense industry.
            - The group also conducts cyber crime likely as an extra source of income to the government as we observed in signature malware [activity](https://advantage.mandiant.com/reports/21-00014321) by this actor; however, targeting of military and government personnel appear to be the primary focus. 
        - RGB -> 3rd Bureau -> Bureau 121 / Lab 110 ->** The Bluenoroff Group / APT38 / CryptoCore**
            - Bluenoroff ==  Stardust Chollima == BeagleBoyz ==  Nickel Gladstone
            - CryptoCore == Dangerous Password
            - APT38 is a financially-motivated threat group that is backed by the North Korean regime
            - The group mainly targets banks and financial institutions and has targeted more than 16 organizations in at least 13 countries since at least 2014.
            - 1,700 (+/-) whose mission is to conduct financial cybercrime by concentrating on long-term assessment and exploiting enemy network vulnerabilities. Bluenoroff exploits the systems for financial gain for the regime or to take control of the system. (2020)
            - Meanwhile, the Bluenoroff group, a subgroup of the Lazarus Group, is more focused on attacking financial institutions and cryptocurrency exchanges.
            - The activities of the Lazarus Group have been reported not only in Korea but in a number of countries 2](https://www.virusbulletin.com/virusbulletin/2018/11/vb2018-paper-hacking-sony-pictures/#ref2), [3](https://www.virusbulletin.com/virusbulletin/2018/11/vb2018-paper-hacking-sony-pictures/#ref3)].
            - APT38 is a financially motivated group sponsored by North Korea, known for significant financial compromises and its use of destructive malware against financial institutions. The group has been attributed to sophisticated compromises targeting Interbank Fund Transfer Systems to steal millions of dollars at a time across multiple countries worldwide.
            - A related, and likely subgroup of APT38 that also primarily focuses on financial activity, is referred to in the open source as “CryptoCore” or “Dangerous Password”
            - Stardust Chollima
                - https://www.crowdstrike.com/blog/meet-crowdstrikes-adversary-of-the-month-for-april-stardust-chollima/
                - STARDUST CHOLLIMA is a targeted intrusion adversary with a likely nexus to the DPRK.
                - This adversary is typically involved in operations against financial institutions with the intention of generating liquid assets for the DPRK.
                - Previous activity tied to this adversary includes campaigns focused on abusing Society for Worldwide Interbank Financial Telecommunication (SWIFT) systems, as well as intrusions against global banking networks via strategic web compromise operations.
                - STARDUST CHOLLIMA uses several implants that share a code framework tracked by CrowdStrike as “TwoPence.” This actor also uses techniques such as code protection tools like Enigma protector, password protected executables and secure deletion functions to remain hidden on target system for long periods of time by avoiding legacy security products.
                - Recent Falcon Intelligence reporting has been published to customers assessing that STARDUST CHOLLIMA is suspected of targeting Latin America-based organizations since mid-2017.
                - STARDUST CHOLLIMA primarily targets its victims with the aim of acquiring funds. 
                - CrowdStrike has not directly observed STARDUST CHOLLIMA conducting intelligence-gathering or destructive operations. It is not known at this time whether the TwoPence framework is used exclusively by STARDUST CHOLLIMA or if elements of it are shared between other related DPRK adversaries such as LABYRINTH CHOLLIMA, RICOCHET CHOLLIMA or SILENT CHOLLIMA.
                - Currency generation represents an additional mission of DPRK actors beyond destructive attacks and espionage; this may reflect the impact of sanctions levied against the DPRK by the international community and the 2017 banning of the DPRK from [SWIFT.](https://www.reuters.com/article/us-northkorea-banks-swift/swift-messaging-system-bans-north-korean-banks-blacklisted-by-u-n-idUSKBN16F0NI)
                - CrowdStrike identified earlier attempts at revenue generation by SILENT CHOLLIMA prior to tracking STARDUST CHOLLIMA, which leveraged unique tools and infrastructure; however, no overlap between the two actors was identified. In addition to financial sector targeting, there is some technical overlap between the [Wannacry ransomware](https://www.crowdstrike.com/blog/falcon-intelligence-report-wanna-ransomware-spreads-rapidly-continually-encrypts-victim-files/), which began self propagating in May 2017, and both STARDUST CHOLLIMA and LABYRINTH CHOLLIMA.
                - The earliest observed version of WannaCry, created in February 2017, generates a custom TLS handshake message as part of its C2 protocol that is sent before actual payload data is transmitted. This handshake message selects a random number of cipher suite constants from a hard-coded array, resulting in changing patterns of network traffic. Some variants of Hawup also generate a fake TLS header with a random selection of cipher suite identifiers that is prepended to actual C2 traffic. While the code is not the same, the concept and structure are similar enough to assume a relation.
                - All WannaCry samples, many Hawup variants, and many tools based on the TwoPence library were compiled using Microsoft Visual Studio 6, which is rarely observed almost 19 years after its release. A hypothesis explaining these similarities is that the different actor groups have access to the same development resources, perhaps even a shared code library, but they engage in different types of attacks according to their respective missions. Community or industry names Lazarus Group, and Bluenoroff have been associated with this actor.
            - https://www.clearskysec.com/cryptocore-lazarus-attribution/
            - https://www.bleepingcomputer.com/news/security/cryptocore-hackers-made-over-200m-breaching-crypto-exchanges/
            - https://attack.mitre.org/versions/v8/groups/G0082
            - https://content.fireeye.com/apt/rpt-apt38
            - https://securelist.com/lazarus-under-the-hood/77908/
            - https://www.us-cert.gov/ncas/alerts/TA17-164A
        - RGB -> 3rd Bureau -> Bureau 121 / Lab 110 -> **The Lazarus Group / TEMP.Hermit**
            - Although TEMP.Hermit is most frequently aligned with Lazarus Group reporting, often times, researchers and open sources lump all three of these actor sets – and sometimes even all of the North Korean APTs – merely as “Lazarus Group”.
            - TEMP.Hermit has been around since at least 2013. Their operations since that time are representative of Pyongyang's efforts to collect strategic intelligence to benefit North Korean interests. This actor targets government, defense, telecommunications, and financial institutions worldwide and the term “Lazarus Group” refers most often to this cluster of activities.   
            - Unknown number of members whose mission is to create social chaos by weaponizing enemy network vulnerabilities and delivering a payload if directed to do so by the regime. This group preloads the network with codes for later activation that disrupt or destroy the network. The Lazarus Group unleashed the WannaCry malware in 2016–2017, causing massive problems around the world—including in the U.S.
        - HIDDEN COBRA
            - BeagleBoyz
        - MSS -> APT37
            - APT37's previous campaigns targeting foreign joint venture partners as well as threat activity against defectors, defector support agencies, and humanitarian organizations indicate APT37's activities most likely align with the agenda of Ministry of State Security.
            - APT37's assessed primary mission is **covert intelligence gathering in support of DPRK's strategic military, political, and economic interests.**
            - A lack of recent, significant activity from this actor matched with an uptick in similar targeting from units within the “Kimsuky” actor-set may indicate a shift or consolidation within North Korea’s cyber leadership. 
            - https://advantage.mandiant.com/reports/21-00027289
            - North Korean cyber espionage group that has been active since at least 2012
            - Targets victims primarily in South Korea, but also in Japan, Vietnam, Russia, Nepal, China, India, Romania, Kuwait, and other parts of the Middle East
            - Been linked to following campaigns between 2016-2018: Operation Daybreak, Operation Erebus, Golden Time, Evil New Year, Are you Happy?, FreeMilk, Northern Korean Human Rights, and Evil New Year 2018.
            - https://attack.mitre.org/versions/v8/groups/G0067
        - APT-C-26
        - Appleworm
        - DPRK3
        - G0032
        - G0067
        - Group 77
        - Guardians Of Peace aka New Romantic Cyber Army
        - Hacking Team 
        - NICKEL ACADEMY
            - https://www.secureworks.com/about/press/media-alert-secureworks-discovers-north-korean-cyber-threat-group-lazarus-spearphishing
        - Office 91
        - Red Dot 
        - Team Whois
        - Zinc 
