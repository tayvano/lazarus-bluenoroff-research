# Uno Re DAO

Date:: November 14th, 2023

Amount Stolen:: $219,000 + 32.4M UNO

Tags: 🎙️ Contagious Interview

---

## Details

From the UNO Re DAO:

"On the recent attack on our capacity pools - what happened, event response, and what the plan ahead is:

The malicious party took over the ‘claims assessor’ role via a compromised owner/admin account, and used it to process a huge fraudulent “policy claim” that led to the drainage of our pools.

Consequently, a total of 32.4M $UNO, 127.9K $USDC, 59.3K $USDT, and 18.4 $ETH was misplaced.

Following these events, we’ve since focused on Fund Recovery and damage mitigation; the exploiter has been contacted on chain (https://etherscan.io/tx/0x153fa7888fee5641e4bbb622bc6e0a1b56d144b62a658da555aa793e786f6acf ), and we’ve also worked with teams over at KC, Gate, and MEXC to freeze funds. 

Our ETH-BSC bridge has also since been disabled. 

$UNO contracts were paused for a brief time to afford us enough time to coordinate with our CEX partners, however they’ve since been unpaused in the interest of maintaining decentralisation. 

We're currently also updating our dApp; at present, please do not interact with it or protocol contracts until further notice. 

Our focus now is two-fold; to release a much more comprehensive post-mortem of the entire event, and a Recompensation plan. 

All staker positions within the pools pre-event are recorded, and will be made whole again.  

(Our tokenomics has a completely reserved Reinsurance Liquidity cell built into it for unforeseen contingencies, which could play a role within this Recomp plan.)

The post-mortem will be published on all our socials, and the Recomp plan will undergo the UNO DAO voting process before being actioned. 

We’re already on our way to recovery, and will keep all DAO members, our community, and capacity providers in the loop at every step of the way via frequent updates like this."

The IP 85.255.176.177 was observed during initial laundering. Tactics and indicators changed later in the flows and for later laundering seessions.

It's highly likely this incident is similar to the one experienced by Terraport and that initial access was gained or significantly aided by one or more DPRK IT workers who were unknowingly employed and/or contracted by the UNO Re DAO.

For this reason, IoCs, Onchain flows, and other elements differ from the DPRK private key compromises that you are likely more familiar with. e.g. The attacker in this instance responded to the team's Onchain messages with a message of their own which rarely, if ever, occurs with DPRK hacks.

Similarly the team does not recall and has not identified receiving one of the infamous Google Docs "Risks of DeFi/Stablecoins(Protected)" that have been especially prevelant and damaging during Q3/Q4 2023.



## Onchain

- https://etherscan.io/tx/0x153fa7888fee5641e4bbb622bc6e0a1b56d144b62a658da555aa793e786f6acf - Message from Uno Team to Attacker
- https://etherscan.io/tx/0x0acdad46f954854acf66f4fc84be2e9ccd3b451139106beaf5b50a7d350f1bc5 - Message from Attacker to Uno Team
- 0xb782425e27a88921189a05be7199748ddbdb71bf - Uno Deployer (Compromised)
- 0x9ada20B835Aa178813A8C174F1F93B1dc1BFA775 - Primary Attacker
- 0x86d49a933d1f6aa1218dfa91250733d9818e36fa
- 0x73904fa075500920fa381c9393819cbe0304b425
- 0xf027a4d8cd87a4ed93b6a332025d73435750f7df
- 0xe4e9b9b6cc9a9c440f932be4a27d4454fe0f6952
- 0x61D885ae7d491A8dEAC79D27C416caf6057C01FA
- 0x45e23fd25aab40e0804fe3a030a24629c369aadd
- 0x5d83c1626ccf39905666379aa71d4a58578bb047
- 0x0942fd57b556c2410b44eb860ceaff224a5f0992
- 0x886e620e86489245ac1885fc827fe2e61b02eaad
- 0x0c1f0233091d6ed371dc84a0ad1602209bca429c
- 0xC1818eEc6C6aff1bD3c2e067511baB5c5396dd54
- 0x63bc27d147a21c1dc8e109ff8d655ea3a47fd1cd
- TLQt68BabARrHQe2C9bJ3dAHGE8Wxv1rTm - Via Allbridge
- TYiX9TcqN9vCWh6mffJSKkwpcCkKNEmDpJ
- TJoLLLMKHyAM4N8ie7L8E3ygG7ZHPFKU7W
- TGEfB2J6rRXDQxAvuhbK3DPUx559XZtp8X
- TTXBLFXWPrtuYLeQX7aT95bMYueVfQVHYu
- TYrQmL73dKjcRWNMCnQov3tk1zZAvfwAzq
- TPJaS8p6TiEV2A9KaBQkjHfLB7SmJxDeav
- TQXZ7s3mftvgehaGSxkMgWd71kNhtHN5fy
- TXREeVJtduJoy8fLPhQKnzo8ySUifAotQX
- TU2ABoNUXj5XkVL4sM1DWE4qCy5nbNZn7Y
- TGJHUunDU9zMQ2u9MpWoDmY2s2VjQm7UxM
- TGTDzAVfNBakewde186gDfubuxCQ6gy5UM
- TW6LRz4NnpTxU85CosLdqhg7WPpZwbNeCV
- TDRz3EKe4QMpAVri7WoWtQjymqPuJ6SHPU
- TEZzcUF8SfxfvqsWqAzJA145BMTQoCmpmB
- TJZDAAP4QMrtzsPw8R8mRq1feqBUYS6MdH
- TCaVKwJHAzChyRcUCpKHVUzXpsvGfQe6rZ
- TFW2F1ZpC54bbs6WeHabg2oQ75F1orbjX4
- TDATk2SqW9DGfiweXUURHWbrWWbiBZLjp5
- TGXdX8njwPQXiyGaxNqjV5twSvdF1Zscv9
- TRNXU4XDvBhBgrUsVVQLoj9E3f3vPxuMZZ
- 0x0c6256ee8e5627e3db68825b563dc483b892dd8f - Dust on BSC



#### ETH Theft Address 0x86d49a933d1f6aa1218dfa91250733d9818e36fa
- $230k -> Theft Address 0x73904fa075500920fa381c9393819cbe0304b425
- $103k -> Gate 0x2618eb69b40e6db8ca732ddb2df5416a4d36e7ae
- $35k -> MEXC 0x03742e4c76f35927f247169ef5560b0c750442e6

#### BSC Theft Addresses 0xf027a4d8cd87a4ed93b6a332025d73435750f7df ->
- $60k -> Stagate -> BSC Theft Address 0xe4e9b9b6cc9a9c440f932be4a27d4454fe0f6952
- $192k -> Gate -> to BSC Theft Address 0xe4e9b9b6cc9a9c440f932be4a27d4454fe0f6952
- $252k -> BSC Theft Address 0xf027a4d8cd87a4ed93b6a332025d73435750f7df

#### BSC Theft Addresses 0xf027a4d8cd87a4ed93b6a332025d73435750f7df 

-> FixedFloat/ChangeNow Deposit Addresses:
- 0x242a49ccd144b704e8a1a2ef09297a563099d09a
- 0x91394f3432a8c59746c3fdb8dac6f378c0db07bd
- 0xafb1542851fc1426c9cead3b9ec41eee0ffcf71a
- 0x55dba2b3b148955385584d69506aa13a666246db
- 0xf39d5dd4b4ba9da847d45208fa756c590b3e6d1b
- 0x1388c7f974d9eea9644b32ee288abb4c4b00ab9c
- 0x8219a0c3a728bf72cfe3c1a9a2ae6118ad8d8e8e
- 0xf6493e543e68af142d7d7037905a5a2591add977
- 0x1a0de3dfa9d4d20dd7561964743ab84b8ce4c12e
- 0x8f37221d2d068a4bd3af80250b8276cadf8376dd
- 0x65beeb3483e80b70ca91c1de692ec1b91b6734dd
- 0x21bc2f1cf845cda1e753949f63bed354eeccf11d
- 0xc2e07ad7abeafc6aa80b6d4f76980f59505961db
- 0x8dc408cc38aa8f0acd7478af57ce3cfe3543ea99
- 0x9a313456b43bda9b8e5f5dd9fbf1c8a7374b6687
- 0xb1d3327617fe5fe68df38d12d65ddd2f5f7bc29a


### BSC Theft Address 0x9ada20b835aa178813a8c174f1f93b1dc1bfa775 ->

- Gate Deposit Address 0x2618eb69b40e6db8ca732ddb2df5416a4d36e7ae

- MEXC Deposit Address 0x9dc68cb1c82deabdd211cc7d89ec1effc74ccd7e


### ETH Theft Address 0x73904fa075500920fa381c9393819cbe0304b425

-> FixedFloat Deposit Addresses:

- 0x62136412cfef1bf3f470f31220145dfd3522b615
- 0xaa63ca233d27748fd002d41ed00d8503d7951147
- 0xa9d4230f3be5e8d590842d19219c003ca9e0e83a
- 0x04d871530ef846218dee7f7a8b6416725b4cb285
- 0xc222a7a0f72eb68c22dcb112a17ddd2cb1c36134
- 0xe91916db9eafc8a721e81891824a7399f14d7879
- 0x03b03407f38377262cab4d50d7b48f8dc37ddb9b
- 0x44a3beae6c69cb08021cf2d793d282549e18ff0e
- 0x8c1a4f1af24f08824b97be64a20f8f4fc52e85d7


#### BSC Theft Address 0x86d -> $403k ->

-> FixedFloat/ChangeNOW Deposit Addresses:
- 0x79f7ea0f953298f966416e1782721d7f829d2722
- 0x02d296a40d52ae858153f72fea2208e27ec98515
- 0x89eacc64480510befcf7f02278799592129f0543
- 0x6bd7778e65d93360fff5b46df601160f46746b1d

#### Tron Laundry Address TYiX9TcqN9vCWh6mffJSKkwpcCkKNEmDpJ

- $214k from TJoLLLMKHyAM4N8ie7L8E3ygG7ZHPFKU7W
- $135k from TGEfB2J6rRXDQxAvuhbK3DPUx559XZtp8X
- $9k from TTXBLFXWPrtuYLeQX7aT95bMYueVfQVHYu
- $47k from TYrQmL73dKjcRWNMCnQov3tk1zZAvfwAzq

#### Tron Laundry Address TJoLLLMKHyAM4N8ie7L8E3ygG7ZHPFKU7W
- $185k from FixedFloat
- $40k from ChangeNOW

#### Tron Laundry Address TGEfB2J6rRXDQxAvuhbK3DPUx559XZtp8X
- $135k from FixedFloat
- $50 from ChangeNOW

#### Tron Laundry Address TYrQmL73dKjcRWNMCnQov3tk1zZAvfwAzq
- $8k from FixedFloat
- Sends $406k to:
- TPJaS8p6TiEV2A9KaBQkjHfLB7SmJxDeav
- TQXZ7s3mftvgehaGSxkMgWd71kNhtHN5fy
- TXREeVJtduJoy8fLPhQKnzo8ySUifAotQX
- TU2ABoNUXj5XkVL4sM1DWE4qCy5nbNZn7Y
- TGJHUunDU9zMQ2u9MpWoDmY2s2VjQm7UxM
- $160k -> TGTDzAVfNBakewde186gDfubuxCQ6gy5UM
- $230k -> TW6LRz4NnpTxU85CosLdqhg7WPpZwbNeCV ->
- $212k -> CoinCola TDRz3EKe4QMpAVri7WoWtQjymqPuJ6SHPU
- $6.6k -> Bitget TEZzcUF8SfxfvqsWqAzJA145BMTQoCmpmB



## IoCs

November 15, 2023:

- IP 85.255.176.177
- en-CA,en;q=0.9
- Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36
- Timezone: America/Toronto


## URLs

- https://twitter.com/unoreinsure/status/1724537541267697878
- https://justice.gov/opa/pr/justice-department-announces-court-authorized-action-disrupt-illicit-revenue-generation
- https://zetter-zeroday.com/p/how-north-korean-workers-tricked
- https://ic3.gov/Media/Y2023/PSA231018
- [Annex 95: Suspected DPRK cyberattacks on cryptocurrency-related companies (2017-2023) investigated by the Panel](../pdfs/2024-03-07_UN-Security-Council_s-2024-215.pdf)


