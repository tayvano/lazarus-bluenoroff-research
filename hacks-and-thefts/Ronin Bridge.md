# Ronin Bridge

Date:: April 14th, 2022

Amount Stolen:: $625,000,000

## Details

The FBI continues to combat malicious cyber activity including the threat posed by the Democratic People's Republic of Korea to the U.S. and our private sector partners. Through our investigation we were able to confirm Lazarus Group and APT38, cyber actors associated with the DPRK,  are responsible for the theft of $620 million in Ethereum reported on March 29. The FBI, in coordination with Treasury and other U.S. government partners, will continue to expose and combat the DPRK’s use of illicit activities – including cybercrime and cryptocurrency theft – to generate revenue for the regime.

Network lost $625M after an attacker compromised 5 of its Validators were compromised  and generated valid transaction signature. 

Laundered Via:: FTX, Huobi and Crypto.com

The massive hack was only noticed 6 days later after a user reported trouble withdrawing the the bridge.

Sky Mavis’s Ronin validator nodes and Axie DAO validator nodes were compromised resulting in 173,600 Ethereum and 25.5M USDC drained from the Ronin Bridge. Attackers used hacked private keys in order to forge fake withdrawals. Sky Mavis’ Ronin chain currently consists of 9 validator nodes. In order to recognize a Deposit event or a Withdrawal event, 5 out of the 9 validator signatures are needed. 

The attacker managed to get control over Sky Mavis’s 4 Ronin Validators and a third-party validator run by Axie DAO.  The validator key scheme is set up to be decentralized so that it limits an attack vector, similar to this one, but the attacker found a backdoor through our gas-free RPC node, which they abused to get the signature for the Axie DAO validator.   

This traces back to November 2021 when Sky Mavis requested help from the Axie DAO to distribute free transactions due to an immense user load. 

The Axie DAO allowlisted Sky Mavis to sign various transactions on its behalf. This was discontinued in December 2021, but the allowlist access was not revoked.  Once the attacker got access to Sky Mavis systems they were able to get the signature from the Axie DAO validator by using the gas-free RPC.  

Actually, it seems like they gained control over 4 Validators, and tricked the fifth one into signing (by using some deprecated api). Their article does a fairly good job describing the 5th validator, but they limit info about the first four to "managed to get control over Sky Mavis’s four Ronin Validators" and "attacker used hacked Private Keys in order to forge fake withdrawals". A bit sus. literally insane that they sent funds to a cex. like wtf

The Ronin Bridge exploit is the largest DeFi exploit ever committed with evidence that the North Korean Lazarus Group was behind the attack. At the end of March, Ronin, an ETH sidechain built for the nonfungible token game named Axie Infinity, was hacked for over 173,600 Ether (ETH) and 25.5 million USD Coin (USDC) for over $600 million. The company officially reported that the hackers managed to get access to private keys to validator nodes resulting in the compromise of five validator nodes. Later reports showed how an advanced spear phishing attack was the main cause for this exploit. The Ronin chain consisted of nine validator nodes and the hackers managed to get access to four of them along with a third-party validator run by decentralized autonomous organization Axie DAO.

The gaming-focused Ronin Network announced Tuesday a loss of over $625 million in USDC and ether (ETH).According to a blog post published by the Ronin Network’s official Substack, the exploit affected Ronin Network validator nodes for Sky Mavis, the publishers of the popular Axie Infinity game, and the Axie DAO.An attacker “used hacked private keys in order to forge fake withdrawals” from the Ronin bridge across two transactions, as seen on Etherscan.While the Ronin sidechain has nine validators requiring five signatures for withdrawals and is meant to protect against these types of attacks, the blog post notes that “the attacker found a backdoor through our gas-free RPC node, which they abused to get the signature for the Axie DAO validator.” The hacker was able to obtain 5 keys which were sufficient to execute the hack. The hack took place on March 23 and was not reported until March 29 when a user attempted to withdraw 5000 ETH from the bridge.The blog post pegged the losses at 173,600 ether and 25.5 million in USDC, currently worth in excess of $625 million.Update 4/19:The FBI has confimed that North Korean hackers or the Lazarus Group were responsible for the theft.Updated 4/22Binance reported that the company recovers $5.8 from the stolen funds as the exploited attemtped to launder through the exchange.Updated 5/3Peckshield reported that Over 90% of the stolen funds have been transferred out of the exploiter's wallet, including ~71,000 $ETH ($213m) already


## On-Chain

- 0x002c93452d54b6d64bfa9879fcab14a74f1bdd44 Ronin Bridge Exploiter May 3rd, 2022 May 4th, 2022 [🔗](https://twitter.com/CertiKAlert/status/1521397324601249794) 
- 0x036587e77eabe6a7e181886a5a6ed10dc25654f9 Ronin Bridge Exploiter  3
- 0x098B716B8Aaf21512996dC57EB0615e2383E2f96 Ronin Bridge Exploiter 1
- 0x0dcb08eabb2bedf838226fb7b2c15a69132df8b2 Ronin Bridge Exploiter
- 0x13113ccfe609c081bb9a7f7d69484b96b90b39fc Ronin Bridge Exploiter
- 0x15e270175f4f2347153d4d113b459590888613e7 Ronin Bridge Exploiter 75.51% or 75.94% via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9
- 0x1aff30f79a05d6505c7846c13dd669858eb52f49 Ronin Bridge Exploiter
- 0x24b6694982843b03c75bb25e1fb74167b55b57b6 Ronin Bridge Exploiter
- 0x28f080edf51145c3f511415b8c2afaebb605a70b Ronin Bridge Exploiter April 23rd, 2022 Ronin Bridge Exploiter - 7023.77 $ETH were sent from sanctioned address April 23rd, 2022 11:25:58 AM UTC 0x3Cffd56B47B7b41c56258D9C7731ABaDc360E073 TX ID: 0x007d395c79ab8ae041e452d4d724645f0d43cb9cd8edb20341f67e9de5e6099c
- 0x29fc9b71492ec63696cf9cd56e9832a42b0dced0 Ronin Bridge Exploiter  4
- 0x3f1b0a5064cc517aa6a2f31f8f07a206f4d7f07a Ronin Bridge Exploiter May 8th, 2022
- 0x49788613913050ce0da9c8313654cee3f4848a9e Ronin Bridge Exploiter
- 0x4bf2c2956942b2dd40517bce423917311f564d16 Ronin Bridge Exploiter 75.51% or 75.94% via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9
- 0x4fe666ecc5263f5dbb34adb8bc1c8cbb9bbcd1cc Ronin Bridge Exploiter  6
- 0x5967524ce3bc2bc422e584e33bd50921a22e3c0a Ronin Bridge Exploiter April 27th, 2022
- 0x5b5082214d62585d686850ab8d9e3f6b6a5c58ff Ronin Bridge Exploiter  7
- 0x5d84a732b355ada31a36b33c446e3dee28f51555 Ronin Bridge Exploiter  2
- 0x622163f3f21752d359216343df88e9108495ca14 Ronin Bridge Exploiter May 2nd, 2022 May 3rd, 2022 [🔗]() 
- 0x77532dd2eb6e8eaf416f39c65f48cd2369782828 Ronin Bridge Exploiter  9
- 0x7e3167771bf23ac10930803589d1424903b36584 Ronin Bridge Exploiter  5
- 0x8c5f8af7a932613efe12cc25d38387e9654517a7 Ronin Bridge Exploiter via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE
- 0x8fa7b50fc8306ab3de028254df72bf08216742b6 Ronin Bridge Exploiter
- 0x930a2e736f91680dca726d8db87a7beca443f2bd Ronin Bridge Exploiter TC->Ren
- 0x93df2c9c8786242b8fdca3f96b3914b8b4a9f704 Ronin Bridge Exploiter via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE
- 0x979443bebd684daee44ea7a6d599bd6ed4cafd55 Ronin Bridge Exploiter via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE
- 0x99b6843f8410ee696b7487a5535dd5b0ca32a12d Ronin Bridge Exploiter via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0x9b72b693440042c3a8045c569c1f9b61b5a92fa9 Ronin Bridge Exploiter via 0x08723392Ed15743cc38513C4925f5e6be5c17243
- 0x9e1e41985048c07a68a67f632f82799baaf903b1 Ronin Bridge Exploiter via 0xa0e1c89Ef1a489c9C7dE96311eD5Ce5D32c20E4B
- 0x9ec8433487939bc432e79fa471a8605610659e41 Ronin Bridge Exploiter via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9
- 0x99b6843f8410ee696b7487a5535dd5b0ca32a12d - Ronin Bridge Exploiter via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0xa3d34ba0400a3952a6c81c4629c3971f1537ae6f Ronin Bridge Exploiter 75.51% or 75.94% via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9
- 0xa4ade1e23f0f98524727797b4975b450a4a8775c Ronin Bridge Exploiter via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0xa58b6105e208cb23e7566d69120319e30a1a9ec4 Ronin Bridge Exploiter via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0xab346efef1ffe377cdad686abeab62e83df1099f Ronin Bridge Exploiter via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE via 0x3Cffd56B47B7b41c56258D9C7731ABaDc360E073 0xb3656c5ed7ef97b4c9097d416df98e2e2a5dd81d 
- 0xbad37a7dfea2aa4fa0198ee4c644632a2d7c91c2 Ronin Bridge Exploiter May 12th, 2022via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE
- 0xbc25d57412a04956cdd95af07825c5c1f34d29eb Ronin Bridge Exploiter  8
- 0xc68b2c011f8df2190f239ddf5d49cb59324528e7 Ronin Bridge Exploiter May 13th, 2022 via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE
- 0xcb3106424ff43365f084df13aba1526769120a79 Ronin Bridge Exploiter May 9th, 2022 via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0xd98d925685908152f18c32697e0d3894a5c672c0 Ronin Bridge Exploiter May 7th, 2022 via 0x35fB6f6DB4fb05e6A4cE86f2C93691425626d4b1
- 0xdd6458eb5090832eb88bffc7adf39b0f3cdd6683 Ronin Bridge Exploiter April 28th, 2022 via 0xa0e1c89Ef1a489c9C7dE96311eD5Ce5D32c20E4B 
- 0xde4612757719829d1df069213a5f4317bb7503e7 Ronin Bridge Exploiter May 18th, 2022 via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9 
- 0xe8b2b5a8a4174b256828fca0f40a8831521160e5 Ronin Bridge Exploiter May 16th, 2022 75.51% or 75.94% via 0x3e37627dEAA754090fBFbb8bd226c1CE66D255e9
- 0xedb60566f3fd86c2cd9db744d59f019dae0e45a6 Ronin Bridge Exploiter via 0x53b6936513e738f44FB50d2b9476730C0Ab3Bfc1 April 21st, 2022 April 22nd, 2022 April 23rd, 2022 May 2nd, 2022 May 4th, 2022 May 7th, 2022 July 20th, 2022 
- 0xf5806e5c1c9402dcc87e9adf47bc7bc2f18cf556 Ronin Bridge Exploiter May 13th, 2022 via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE April 27th, 2022 April 28th, 2022 April 29th, 2022 May 11th, 2022 May 12th, 2022 May 22nd, 2022
- 0xf7b31119c2682c88d88d455dbb9d5932c65cf1be Ronin Bridge Exploiter
- 0xf945fa5b71cfaa2736b427b7213cff14cc83279c Ronin Bridge Exploiter May 22nd, 2022 via 0x08723392Ed15743cc38513C4925f5e6be5c17243 May 4th, 2022 May 10th, 2022 May 18th, 2022 May 19th, 2022
- 0xfe4a0d465636ba3f6906818af88c1e01ae0d9d6e Ronin Bridge Exploiter May 13th, 2022 via 0xF7B31119c2682c88d88D455dBb9d5932c65Cf1bE May 11th, 2022 May 22nd, 2022


## Tornado Withdrawals (Medium-Low Confidence, I don't remember how careful I was tracing these)

- 0x837d2c2ba22ec450359f3046f67b7270c8812e57
- 0x46cd908a7a91100660dc51fea020515b11ab124e
- 0x0433c6202c28ec2b3fba10d70d6795318b4cd260
- 0xc5427a1d2de32aea742093a2e6b38c59cb9e5cf2
- 0x748e938845594ec296f57e4ed7fc5281e218d613
- 0xd3397c8460e96dad334d476477522086f76a5628
- 0xa6e908f1828048aa09664e832233a9800ad72d16
- 0xa0c614ff67d8687d248a3bf49f12d145e711bd7e
- 0x161bac1349568cf5ca1a7af05a118e8079e6a28d
- 0x7a0254e134c00fa7b9f82264fc7960bce2ff0dac
- 0xa2524611561d053f17c45af9b746f9a7df2221a3
- 0x7bc4db9ac25768598f3abdf89b41c1daf4d6c762
- 0x1401d8805b8579692d56d514d5183272d1ca3673
- 0x780f41a4ae446dc10d78b0070108864f701db214
- 0x6db52d90e0cca1db7cff815b8334c5c70db7fe6a
- 0x069d95b81f3120ada24a0f7e097cc3cea908a8c6
- 0x8c59c33dbc99b83a78d825f6bdb0ebb5c54543d6



## April 14th, 2022 - Report: The FBI attributed North Korea based Lazarus Group to the Ronin Bridge -  Addresses added to OFAC list

According to the FBI, the infamous cybercrime group Lazarus has been implicated in the March Axie Infinity exploit that saw $625 million taken from the game's blockchain bridge.

Lazarus are a criminal group with strong ties to North Korea, and are suspected of being behind infamous cyberattacks including the [WannaCry ransomware that impacted a wide number of industries including hospitals and manufacturing, as well as legislative and justice systems.

The U.S.Treasury department has added the crypto wallet that received the stolen funds to its sanctions list, which may make it substantially harder for the attackers to withdraw the money.

The wallet still contains around 150,000 ETH, valued at around $445 million, but has been slowly siphoning it out to various other wallets, exchanges, and tumblers over the past weeks.

Validator Security Breach US Treasury Department has sanctioned the address that received the stolen funds.  


## Links

- https://twitter.com/blocksearch/status/1514685894619549703
- https://twitter.com/Ronin_Network/status/1530076035345453056
- https://blog.mollywhite.net/axie-hack/
- https://bridge.roninchain.com/
- https://home.treasury.gov/policy-issues/financial-sanctions/recent-actions/20220414
- https://rekt.news/ronin-rekt/ 
- https://roninblockchain.substack.com/p/community-alert-ronin-validator
- https://roninblockchain.substack.com/p/community-alert-ronin-validators
- https://twitter.com/CertiKAlert/status/1521397324601249794
- https://twitter.com/Ronin_Network
- https://twitter.com/TheBlock__/status/1544684472704159747
- https://www.coindesk.com/tech/2022/03/29/axie-infinitys-ronin-network-suffers-625m-exploit/
- https://www.fbi.gov/news/press-releases/fbi-statement-on-attribution-of-malicious-cyber-activity-posed-by-the-democratic-peoples-republic-of-korea
- https://www.web3rekt.com/hacksandscams/ronin-network-12

## Commentary

> "The Ronin bridge has been exploited for 173,600 Ethereum and 25.5M USDC. The Ronin bridge and Katana Dex have been halted." – @Ronin_Network
- [https://twitter.com/Ronin_Network/status/1508828722085867521](https://twitter.com/Ronin_Network/status/1508828722085867521)

> "Imagine stealing 600 million 6 days ago and depositing money on FTX" – Igor Igamberdiev
- [https://twitter.com/FrankResearcher/status/1508832517826174989/photo/1](https://twitter.com/FrankResearcher/status/1508832517826174989/photo/1)

> "there had to have been someone who noticed the 600M exploit on chain, 50x lev shorted Axie Infinity and Ronin, then got liquidated because.. no one else realized for six days"
- [https://twitter.com/ExaltedFoks/status/1508836040894828544](https://twitter.com/ExaltedFoks/status/1508836040894828544)

> We discovered the attack this morning after a report from a user being unable to withdraw 5k ETH from the bridge." 173600 ETH went out and they notice this 5 days after lmao
- [https://twitter.com/Sleapy31/status/1508832156512137223](https://twitter.com/Sleapy31/status/1508832156512137223)

> Ronin's multisig holders. https://pbs.twimg.com/media/FPB-ipBXIAM5MP6.jpg
- [https://twitter.com/dogetoshi/status/1508845086137884676](https://twitter.com/dogetoshi/status/1508845086137884676)

> This even tops the Wormhole Bridge hack. They forgot to mention the money he stole from the Validators themselves in addition to the bridge (an additional ~8500ETH)
- [https://twitter.com/siegerhino2/status/1508842734416707584](https://twitter.com/siegerhino2/status/1508842734416707584)

> Our team is in touch with Axie Infinity team providing assistance in tracking this issue.  –CZ
- [https://twitter.com/cz_binance/status/1508869326916530176](https://twitter.com/cz_binance/status/1508869326916530176)

> "Important announcement regarding a security breach on the Ronin Network." – Axie Infinity
- [https://twitter.com/Ronin_Network/status/1508828719711879168](https://twitter.com/Ronin_Network/status/1508828719711879168)

> "So the biggest #play to earn game all this time was the @Ronin_Network itself?" – @chainyoda
- [https://twitter.com/chainyoda/status/1508864824867966978](https://twitter.com/chainyoda/status/1508864824867966978)

> By the way, @0xPolygon is secured by a 5-of-9 multisig. Just like @Ronin_Network. And they've refused many, many, many times to answer any questions about how those keys are secured. Do you think that what happened to Ronin's bridge could ever happen to Polygon's bridge? Hmm?
- [https://twitter.com/Mudit__Gupta/status/1508884826987843584](https://twitter.com/Mudit__Gupta/status/1508884826987843584)

