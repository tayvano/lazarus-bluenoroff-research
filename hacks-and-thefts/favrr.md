# Favrr

Date:: June 25th, 2025

Amount Stolen:: $650,000

Tags:: 💼 


---


## Note

This is mostly ZachXBT's work and research. I've just copy/pasted.

- [Source: zachxbt](https://x.com/zachxbt/status/1938598925004607629)


## Background

- Favrr Marketplace is a dynamic and gamified platform where users can buy, trade, and hold digital assets called FAVEs, which represent popular people, places, trends, and even foods. Positioned as the “Fandom Exchange,” Favrr allows users to financially engage with their passions as if they were stocks, using a unique trading mechanism based on cultural and social relevance rather than traditional financial metrics.

- The core experience begins with the Initial Fan Offering (IFO)—Favrr’s version of an IPO—where users can claim FAVEs before they are open to public trading. Once the IFO ends, these FAVEs can be traded using FAV points, the platform's utility currency. This setup encourages strategic trading similar to a stock market, with the goal of growing one’s FAV portfolio and outperforming other users. Assets range from real-life figures like Elon Musk or Marie Curie to pop culture icons, cities, animals, and trending concepts like “Unicorns” or “Pizza.”

- [Source: quadrigainitiative](https://quadrigainitiative.com/casestudy/favrrmarketinsidertechnicalissueduringdexlisting.php)


## Onchain


#### Favrr ITW 1 - Santokh Veenasenan

- 0x17087f92d16049e9097413b4964663b754c1e43d - Payroll

- 0x477d13ee1e1304292d270bfac1aa496902e6851f - Another DPRK ITW consolidation

- github.com/savvy-bit

- santokh.veenasenan@gmail.com



#### Favrr ITW 2 - Nicolas Chi

- 0x641279133f6f560c3f512b8e2d286ae2c53c31ee - Payroll

- 0xCC8020bed135ba9eCf9312Ea0c36234A0BcEC05F - Payroll

- 0xe826c702c35d728315351aec9e93bcf461989de6 - Gate

- 0x21b75888c19eef98c3a8a16efd8f0cb4ba9cf24b - Gate

- 0xab7cd6714cc78ad46592628e79392a5b863f6b6a - Gate

- nic92047@gmail.com



#### Favrr ITW 3 - Alex Hong 2

- 0x69EACe431fEC9E6b1535DaFA3873BB23C995Be93 - Payroll

- 0xdC43B90db03B575B760Ef7B401AA647881f15081 - Payroll

- 0x3c2D3aF542D742e48Eb0454133BE4DE9eF524e10 - Payroll

- 0xc5abde4ce8c5740f4bad62c3b05e4da31d229659 - See https://chollima-group.io/posts/dubai-crypto-moonstonesleet-pivot-odyssey

- x.com/AlexHong953

- alexhong950503@gmail.com

- alexh.engineering@gmail.com 

- alex@favrr.com



#### Favrr ITW 4 - Ikeda Okura

- 0xeabeb8D76E27248eC35333bAdaad9219D8f5797 - Payroll

- 0x6c90b98b8c5c41d615300b9ed774f85b29078ca2 - ifeel.eth, DPRK IT: 1:25-cv-01769

- Ikeda Okura is also chainlito aka woof_decentra

- 01769 Mar 28 2022, ifeel.eth

- okura.ikeda0325@gmail.com



#### Favrr ITW 5 - Victor Lee

- 0x50D6B6cF0066A0d3eBF321493da2E77CC40Ddd8C - Payroll

- victor3290lee@gmail.com

- github.com/blue32captain 



## Further Reading

- https://twitter.com/zachxbt/status/1938598925004607629

- https://twitter.com/favrr_market/status/1938135850375655511

- https://quadrigainitiative.com/casestudy/favrrmarketinsidertechnicalissueduringdexlisting.php

- Attributed in [MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities]./pdfs/2025-10-22_MSMT-Report.pdf)



## ZachXBT's Thread

1/  Multiple projects tied to Pepe creator Matt Furie & ChainSaw as well as another project Favrr were exploited in the past week which resulted in ~$1M stolen

My analysis links both attacks to the same cluster of DPRK IT workers who were likely accidentally hired as developers.

2/ On Jun 18, 2025 at 4:25 am UTC ownership for ‘Replicandy’ from Matt Furie & ChainSaw was transferred to a new EOA 0x9Fca.

Jun 18, 2025 6:20 pm UTC: 0x9Fca withdrew mint proceeds from the contract

Jun 19, 2025 5:11 am UTC: 0x9Fca unpauses the mint

The attacker then minted NFTs and sold into bids causing the floor price to fall to zero.

3/ On Jun 23, 2025 the attacker transferred ownership from the ChainSaw deployer to 0x9Fca for Peplicator, Hedz, Zogz.

Similarly the attacker minted NFTs and sold them into bids causing the floor price to fall to zero.

- 0x9Fca3AC75cd66f3c62bea8231886513b9fe191BD

4/ In total I estimate $310K+ from their projects was stolen and transferred primarily between the three address below. 

- 0xf6a9349c54d51f7f76bbd2afd755b5dd75e617ee - Chainsaw Thefts

- 0x7e580f916a8e93871b72a694407fb7d790de96a6 - Chainsaw Thefts

- 0x58f4299465b261e79713e5c78a7629cd656aed36 - Chainsaw Thefts

5/ The attacker transferred 2.05 ETH to exchange 1 on Jun 18 at 7:47 pm UTC.

By performing a timing analysis I could locate the destination transaction where 5007.91 USDT was received and transferred to MEXC.

- 0xf87fbc5e8fff065b413d3d48932b6fb5585d93d5

6/ Tracing back from the MEXC deposit address 0xf87 revealed many other stablecoin deposits received each month ranging from $2K-10K for various projects.  

As those teams were helpful with providing info and the DPRK ITWs were removed so I will not name the project.

7/ Two GitHub accounts used by suspected DPRK ITWs in this cluster can be seen below and listed wallets on their account.  

- DPRK ITW 1: devmad119 - 0x93d5785d759563b5b8eb98eaff9196dddf7179f3

- DPRK ITW 2: sujitb2114 - 0x6c88dd91de053fca915baece6868f6c32d20adea

8/ Other indicators revealed from internal logs point out irregularities in a suspected DPRK IT workers resume. 

Why would a developer who claims to be living in the US have a Korean language setting, Astral VPN usage, and have an Asia/Russia time zone?

9/ Tracing back from the MEXC deposit 0xf87f lead to another different DPRK ITW consolidation: 

- 0x477d13ee1e1304292d270bfac1aa496902e6851f

10/ DPRK ITW consolidation 0x477 received payroll from the project Favrr which was exploited for $680K+ on June 25, 2025

I suspect they have a second ITW on payroll as well because the exploiter address is tied to a Gate deposit address 0xab7 which ITW 2 sent payroll to. 

- Favrr ITW 1 0x17087f92d16049e9097413b4964663b754c1e43d

- Favrr ITW 2 0x641279133f6f560c3f512b8e2d286ae2c53c31ee

11/ The Favrr CTO Alex Hong has a background which appears suspicious and is likely one of the two DPRK ITWs hired. 

His LinkedIn was very recently deleted. 

I also reached out to a project he supposedly worked at but could not verify his work history.

12/ Soon I plan to publish my stats on total payments being sent out to DPRK ITWs at companies/projects to provide insight into how bad it is. 

It’s depressing how many teams hire DPRK IT workers when basic due diligence would likely have prevented it.

The lack of communication from Matt Furie & ChainSaw since the incident occurred has been disappointing with their only warning to the community deleted without explanation. 

The stolen funds from the ChainSaw incident mostly remain dormant.

The stolen funds for Favrr were transferred to Gate and a few nested services. 

I have been unable to get in touch with the teams due to DMs disabled and no way to easily contact them on Telegram or Discord.

Source: https://x.com/zachxbt/status/1938598925004607629