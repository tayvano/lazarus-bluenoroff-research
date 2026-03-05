# IoTeX

Date:: 2026-02-20

Amount Stolen:: $8.8m

---

## ASSESSMENT

THIS AND INFINI ARE LIKELY EXPOSED KEYS VIA GITHUB, NPM, DOCKER, ETC.

THE OVERLAPS WITH DPRK AND MALICIOUS IT WORKERS IS BECAUSE THOSE GUYS ALSO DO THE SAME THING AND GET REKT

THE EMPLOYEES WHO WERE REKT ARE, UH, UNCLEAR. MAYBE SCARED, MAYBE DID OTHER BAD THINGS, MAYBE FLAT OUT WRONGLY ACCUSED.

WISDOM: JUST BECAUSE PEOPLE LIE DOESNT MEAN THAT PEOPLE LIE ABOUT **THIS THING.** PEOPLE LIE ALL THE FUCKING TIME. INTENTIONALLY, UNINTENTIONALLY, BECAUSE THEY ARE GUILTY OF THIS CRIME, BECAUSE THEY ARE ASHAMED OF ANOTHER NON-CRIME.

The following are the notes I took at the time of the investigation (the above is writen before pushing this up, no idea if i ever finished taking all my notes)

## Details


> IoTeX.io bridge hacked due to owner private key compromise
> The total loss is yet to be known, but our estimates are around $8.46 million
> Attacker compromised the owner key of the TransferValidatorWithPayload contract and called upgrade() to transfer ownership of the bridge's TokenSafe and MinterPool to themselves. 
> They then drained all bridged assets from the TokenSafe ($4.37M) and minted 821M CIOTX via MinterPool ($4.09M). Funds routed to multiple beneficiary addresses.
> Drained from TokenSafe: 1,144K USDT + 1,364K USDC + 635 WETH + 6.1 WBTC + 20K DAI + 8.7 PAXG + 13.8M IOTX + 45.8K BUSD + 2,835 UNI
> Minted via MinterPool: 821M CIOTX + 9.3M CCCS/CCS
> 0xe6a191a894dd3c85e3c89926e9f476f818ee55d9 - Attacker
> 0x6487b5006904f3db3c4a3654409ae92b87ed442f - Primary beneficiary

[Source: DefimonAlerts](https://x.com/DefimonAlerts/status/2025148338635469074)


## Onchain

- 0xe6a191a894dd3c85e3c89926e9f476f818ee55d9
- 0x0aed79256c1ca8941f02e074fbfbbc9d9a91dda2
- 0x0dc19b260e8905c05c27b9ee2eccb93ad69cdf1d
- 0x136b4217040fb5f97845026baf46f5c34640802e
- 0x1ac26ea637975b6c70e95af161b38e1977671410
- 0x20e27ac5eeffea46c6714f8bdb8071e6fd42fd48
- 0x39c188029433bdd7965b55959221abe00466565e
- 0x43ed5caadb3fbef610dad8aae621519b20b34de6
- 0x4b6f08cda7024b52d8e342fa8afbd66d09763c73
- 0x6487b5006904f3db3c4a3654409ae92b87ed442f
- 0x7ddb0f8dd54f5f85f4f8f4138f60b096dcd6d9c9
- 0x91b1d8d3601c3b79ebf24ec6bf15db3bf8abd980
- 0x99e8fba54994a5e4a01177a08d15c2bce040aa7a
- 0xa467a6c7ca8e812e997bfe50ce4e7991aad00a88
- 0xa4ef69e38c0d3ecc28f1566678d117dab1ca4552
- 0xb67dc399cd89ce524c251e9d545b05d77ff8958d
- 0xc6763acab735376107c89a436c477d87ac13dcb7
- 0xc9ca98967cc0f9ffb36c9752e8d7536f6b815c1b
- 12V7jhcPnqnGbRFMasSW2CZVBd8qpvUgAK
- 135oSa2fobTxtHtm5dwTREDyRY2o1DG1Aw
- 16xusPKLMyqK68SkhfXDtic6AJPDi51tqh
- 1PN2BoHU4buDQWcrNHk9T9NBA2qX8oyYEc


- 0x6dd31a526ee3ddbc7be888b729a445695c03148e - IoTeX Deployer (Compromised)

- Transfers to 0xE6A191a894dD3c85e3c89926e9f476F818eE55d9

- Transfer Ownership - TransferValidatorWithPayload 0xE7eBA1CEA51EC9B3AcCC16728e3B8786560c59d5

- Transfer Ownership - TokenCashierWithPayload 0x1B9AA865d74b2B77fFdbCF507B56a7b3AB43Bac4

- Transfer Ownership - TokenCashierWithPayload 0xD57bde0a8bb77a2F65769316f6343E0A13a8d7D4

- Transfer Ownership - Unwrapper 0xeDEC2dAD0b20A46678491bb04c53Cdc89f1b4287




## Links to Infini and Cult / LunaFi / Etc

#### Short Version:

- 0x790ac11183ddE23163b307E3F7440F2460526957 (shaneson.eth) -> 0x8885245Ff8fE32AeC463c8f492f11123b8b9213D -> 0x8DE35691601D1979b100C664651A775FB98E2DCC

- https://bscscan.com/tx/0x30b39d695778c52591984bbafa3312983ab1ab46793b79c1dd75ed4b568803f1


#### Long Version:

0x790ac11183ddE23163b307E3F7440F2460526957 (shaneson.eth) is the address linked to the infini exploit and to the dev that made edits to the code causing the exploit. 

When looking at the ioTex exploit this morning, the initial funding tx through CN originated from 0x8885245Ff8fE32AeC463c8f492f11123b8b9213D on BSC. 

0x8885245Ff8fE32AeC463c8f492f11123b8b9213D receives funds directly from 0x790ac11183ddE23163b307E3F7440F2460526957, which shows a link between these two exploits. 

0x11d2De3114A000d93bB74eBfce3ec684fA099E4D is also linked to ioTex, and was gas funded through a Thorchain transaction from ltc1qq2q4s00gvzwwvh24gshut85kv0qw5wfnt5k65v. 

This LTC address also uses thorchain to bridge some funds to 0x1ce56df1B671AeAeFFDB11939C92Fc64658D7172, which are eventually deposited into Kucoin at 0x7711B52B40f0097F370D2EE0CD843D3bC09471C2. 

When looking at other funds that have also deposited into this address, 0xE6871BB8fF5d0c432Ee199C65453456353440728 is another. 

Tracing through this address, there is links to Contagious interview at 0x6cd36B9459dfef332479d50bEc129932285A1656 (https://wearecultdao.medium.com/0xblock-exploited-5da3d0bbc00e and https://github.com/tayvano/lazarus-bluenoroff-research/blob/main/hacks-and-thefts/various_2023_rug_pulls.md)


--

# Infini Hack

Date:: 2025-02-25

Amount Stolen:: $50,000,000

---

- Crypto-focused stablecoin neobank Infini was attacked, with the attacker gaining access to a wallet with admin rights and stealing nearly $50 million from the company.

- https://x.com/MistTrack_io/status/1893926049882239085

- https://quadrigainitiative.com/casestudy/infinimoneyanonymousdeveloperbackdoorvaulttheft.php

### Onchain

- 0xc49b5e5b9da66b9126c1a62e9761e6b2147de3e1 Infini Dev Team (Compromised? Insider?)
- 0x9a79f4105a4e1a050ba0b42f25351d394fa7e1dc Infini Contract (Compromised)
- 0xc75b143301cf47a3ad096ed904f5e3f0831a57fb Infini Christrian2022.eth
- 0x790ac11183dde23163b307e3f7440f2460526957 Infini shaneson.eth

- 0x3ac96134fb0e42a52d33045aee50b89790f05ed0 - Infini Direct Theft
- 0xfcc8ad911976d752890f2140d9f4edd2c64a6e49 - Infini Theft
- 0x762d46904b93a1eedbff2fd50445cb8ffa41f9fb - Infini Theft
- 0x7142829618adeb8c70caf7a2e7ca413cb7bafa41 - Infini Theft / Tornado Cash


- 0xad4722240d5f7250bb679dff26386e6de18178f43b51bc97b7b4301e2edd8b46
- From: 0xc49b5e5b9da66b9126c1a62e9761e6b2147de3e1 - Infini Dev Team
- To: 0x90210001ffdc5c90645c347a583922c1b9fe8e44 - Sweeper Bot (Mar 2025)
- Date:: 2025-02-25 07:30

- 0x40c1b9d3f386daa18e75366a3dc16a237b13406ad23f5a18062f898bbc870d67
- From: 0xc49b5e5b9da66b9126c1a62e9761e6b2147de3e1 - Infini Dev Team
- To: 0xc98963115fd7062a408974d801ca7f2963787687 - Sweeper Bot (Feb 2025)
- Date:: 2025-02-24 02:16

- 0xf44080bcde9784364ad6ed53fd5e4a1dbb47bc6e2a1dc490fe5ece4bbe887815
- From: 0xc49b5e5b9da66b9126c1a62e9761e6b2147de3e1 - Infini Dev Team
- To: 0xabcde69d995a1ae7d976f5bcde00050de809ca08 - Sweeper Bot 
- Date:: 2025-07-24 07:49


> sweeper script, mark him please my address - 0xc2e810EF34593EfEF14460fBC673845978B1181d
- [2024-12-16](https://chainabuse.com/address/0xc98963115fd7062a408974d801ca7f2963787687?chain=ETH)

> If you will ever post your wallet private key on github this wallet will steal everything in your wallet. 0x90210001ffdC5c90645c347a583922c1b9FE8e44 Report this sucker.
- [2025-03-29](https://x.com/nftfanstoken/status/1906069772258738544)

> @aixbt_agent what can you say about this address 0x90210001ffdC5c90645c347a583922c1b9FE8e44
> my eth was stolen too by this address
- [2025-02-14](https://x.com/Mouseng20/status/1890391721545986060)

> The wallet in the script running on the cloud service got stolen. After searching for a long time, I found out it was because when running Docker, I uploaded to Docker Hub and the hacker scanned the private key.
> This is the hacker's address: 0x90210001ffdc5c90645c347a583922c1b9fe8e44
> Money keeps flowing in every moment 😭😭, and the source funds came from @binance. A quick search on Twitter revealed many other victims. @heyibinance
> @cz_binance, big sis or big cousin, can you send someone to check this out?
> Finally, a reminder to everyone: Before uploading code with private keys, first check if the channel is public. Nowadays, all sorts of hackers are using scanners to sweep the web like crazy—once they spot a private key, they grab it in seconds, no chance to breathe. 5555.
> Over a thousand Docker Hub images leaked authentication keys and private keys
> https://51cto.com/article/761765.html
- [2025-05-06](https://x.com/WhoIsBlank888/status/1919781877432647830)

> fuck for this wallet. 0x90210001ffdc5c90645c347a583922c1b9fe8e44
- [2025-04-20](https://x.com/nakcryptos/status/1913968797062758746)

> Whoops... accidentally did a git commit with my phrase in. Took seconds for someone to start draining 0xabcde69d995a1ae7d976f5bcde00050de809ca08 Mostly a test wallet but still.
- [2025-08-31](https://x.com/Rotwang9000/status/1962198454660202782)






---

# Mi Tanda?

- 0x2a12d779e06cac14e7336b9f854f53f250f66ec4 - Austin Lee / nextidearly
- 0xc2c71c5a9393241b94b8be414c4fdc3db6d8d2e3 - Austin Lee / nextidearly
- 0x72c3c8b0cacdf6e36b39c9462a42756b2a294ccb - basedandearly.eth

- 0xae22381f7d107defaf983af703b9fff257615efd - Attacker






---

# Sweeper Bots

https://intel.arkm.com/explorer/entity/e8333382-d09d-4152-86c5-05d6ddcfd12c

0xde617b937b6707179b858cb09645df6aa5922a4e Probably compiled in github, Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc https://chainabuse.com/address/0xde617b937b6707179b858cb09645df6aa5922a4e
0xe69c3c9a3182f77775768c86d3908eca7f62b9cb Probably compiled in github, Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc https://chainabuse.com/address/0xde617b937b6707179b858cb09645df6aa5922a4e
0x333334049d3b456bd17046506eb1b87c8d417d91 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0x4444444455f7a977353e443b2ef36afd1d67ffcc Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0x5555555550a33ff78cece5fe8bcad75486a5dde3 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0x532d6c35178195dde7ff21510eb77d6ff8f08844 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc https://chainabuse.com/report/481f23be-7262-4385-8d63-e852cdaaae38
0x836b003d1fdb16dbea2e34938b62144a826aae86 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0xb8defd92a3e6e1c930b85a02af1024f5defe11b1 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc https://chainabuse.com/report/481f23be-7262-4385-8d63-e852cdaaae38
0xba8d86573139e6640ed30dfcedad268b655ac760 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0xf7ac89b4b91e8c6945b25a82e56699971e7f03b8 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0x222222237c401664d14c615d53e2500d12540d17 Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc
0x64b31298a90edc88f04ed7dd345b16bf659d81d2 Infini, Tay Github/NPM Trace, https://chainabuse.com/report/4ed02b6c-b3ea-4ec5-903b-75a814e9c5bc, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0xabcde69d995a1ae7d976f5bcde00050de809ca08 Infini, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x3f8abb5f743e6123b773067c6a7202275c6c53e8 Infini, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x90210001ffdc5c90645c347a583922c1b9fe8e44 Infini, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0xc98963115fd7062a408974d801ca7f2963787687 Infini, Unclear, https://chainabuse.com/address/0xc98963115fd7062a408974d801ca7f2963787687, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x1234e2efbcb9dbc0a1f61e16440d1131735efb7f Unclear, https://chainabuse.com/address/0x1234e2efbcb9dbc0a1f61e16440d1131735efb7f, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x541b9034c82d7fb564f12ca07037947ff5b4ef2f Unclear, https://chainabuse.com/address/0x541b9034c82d7fb564f12ca07037947ff5b4ef2f, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x1fa63a80d5f3b7b092e6b70dce5beba996a92fa6 Probably Github, https://chainabuse.com/address/0x1fa63a80d5f3b7b092e6b70dce5beba996a92fa6, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x6900ef7bcd4ec8e81d89808b6a089c4f6377e81c Env File, https://chainabuse.com/address/0x6900ef7bcd4ec8e81d89808b6a089c4f6377e81c, Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x1f4ef1ed23e38daa2bd1451d4cef219c93b2016f Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x1fa438c9dde4c8bc5c3411bc1c41b2d5aafb05ff Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x248999aa27c097e02c70558429e75ed1e5d25d83 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x39bfd1e48c38da0d599ff8a4cfb22e9c71ab355c Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x40206c1b9e5b0f2b4a360707472afd1d79d2b562 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x626b3a959a3c6552ed13a967fd747172ac57df24 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x69d2058be5ed028bdb530b870ed44cb878615ac0 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0x8ca0c75932e845ff4291d6ebedc17cfbbc584d40 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0xa129ca835558a0f61a438392d1ae495a4fa32218 Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0xf3e920c95036bd0cff07326833abc2efe27420bd Tay Trace 2 https://chainabuse.com/report/d8908eb8-2e7c-470d-96e1-28cd76d118e5
0xc05c060759b0fc22cc0c7ab7aa609688a06493e0 Unclear, https://chainabuse.com/address/0xc05c060759b0fc22cc0c7ab7aa609688a06493e0
0xa21f6ce344addae8f77965e03a00cc8b2549edca Prob Github, https://chainabuse.com/report/2f432684-e440-43c2-9ceb-b316413d2d98

0x01dc4656603ac33d3eee77f16209552b46f5b7a9
0x76a7d086df4927c588de0f62de79db2ffdead666
0x8bea73aac4f7ef9daded46359a544f0bb2d1364f






