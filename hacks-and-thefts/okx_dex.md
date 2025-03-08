# OKX Dex

Date: December 12, 2023

Amount Stolen:: $2,390,976 (142k USDT + 475k USDC + 799.77 WETH)

Tags: 🎙️ Contagious Interview

---


## Details

The proxy admin owner upgraded the DEX proxy contract to a new implementation contract, which may have led to the compromise of the private key of the OKX DEX. After the upgrade, tokens started being stolen from the platform. The stolen native ETH was distributed between three addresses, while the rest of the stolen stable coins were bridged to Arbitrum and Avalanche chains via Stargate Bridge. The DEX proxy was removed from OKX's platform's trusted list following the incident. The total loss amounted to 2,390,976 USD worth of assets, including 142,034 USDT, 475,929 USDC, and 799.77 WETH.


## Description

> On December 12, 2023, at 22:23:47, the Proxy Admin Owner upgraded the DEX Proxy contract to a new implementation contract through the Proxy Admin. The new implementation contract's functionality is to directly call the claimTokens function of the DEX contract to transfer tokens. Subsequently, attackers began calling the DEX Proxy to steal tokens. The Proxy Admin Owner upgraded the contract again at 23:53:59 on December 12, 2023, with similar functionality, and continued stealing tokens after the upgrade. As of now, the attacker has profited approximately 430,000 U.
> This attack may be a result of the Proxy Admin Owner's private key being leaked. Currently, the DEX Proxy has been removed from the trusted list.
> OKX DEX contract: 0x70cbb871e8f30fc8ce23609e9e0ea87b6b222f58
> OKX DEX TokenApprove contract: 0x40aa958dd87fc8305b97f2ba922cddca374bcd7f
> DEX Proxy: 0x55b35bf627944396f9950dd6bddadb5218110c76
> Proxy Admin: 0x3c18f8554362c3f07dc5476c3bbeb9fdd6f6a500
> Proxy Admin Owner: 0xc82Ea2afE1Fd1D61C4A12f5CeB3D7000f564F5C6
> Upgrade Txn: https://etherscan.io/tx/0xc6a5a7bc31bbc9a7530189e718f7ed96789fa65c56c3a4a08079a95074e280c8
> Upgrade Txn: https://etherscan.io/tx/0x22ebd267d7344780e6d63cf3a76bab57b8f8fa41cf58df1a2e1707d75d8bee89
> Suspected Attacker: 0xFacf375Af906f55453537ca31fFA99053A010239
> Profit Address: 0x1f14e38666cdd8e8975f9acc09e24e9a28fbc42d

– [Slowmist](https://twitter.com/SlowMist_Team/status/1734790816806449567)


## URLs

- https://twitter.com/okxweb3/status/1734794114657657004
- https://twitter.com/AnciliaInc/status/1734795426572980696
- https://twitter.com/WuBlockchain/status/1734784767760195671
- https://web3isgoinggreat.com/?id=okx-dex-hack
- https://cointelegraph.com/news/okx-dex-2-7-m-exploit-proxy-admin-contract-upgrade


## Onchain
- 0x70cbb871e8f30fc8ce23609e9e0ea87b6b222f58 - OKX DEX Contract (Victim)
- 0xf85f008fe404d4d2cc2196175e1328545f47b8cd - OKX DEX Compromised Key
- 0x0d8fd76cedccc2b386972cad7fa567daa1fd70a1 - OKX DEX Compromised Key
- 0x5b6f25a9c1019a3104bede0f97adba9f0b1620c2 - OKX DEX Compromised Key
- 0x97fc2b556fb65a935d0b47acdd410b88527c7dee - OKX DEX Compromised Key
- 0x40aa958dd87fc8305b97f2ba922cddca374bcd7f - OKX DEX TokenApprove Contract (Victim)
- 0x55b35bf627944396f9950dd6bddadb5218110c76 - OKX DEX Proxy (Victim)
- 0x3c18f8554362c3f07dc5476c3bbeb9fdd6f6a500 - OKX DEX Proxy Admin (Victim)
- 0xc82Ea2afE1Fd1D61C4A12f5CeB3D7000f564F5C6 - OKX DEX Proxy Admin Owner (Victim)
- 0xFacf375Af906f55453537ca31fFA99053A010239 - OKX DEX Attacker
- 0x0519efacb73a1f10b8198871e58d68864e78b8a5 - OKX DEX Attacker
- 0x1f14e38666cdd8e8975f9acc09e24e9a28fbc42d - OKX DEX Primary Theft
- 0x48e3712c473364814ac8d87a2a70a9004a42e9a3 - OKX DEX Theft/Laundry
- 0xa15fe801dd5fd31a684c444b6980dbaf0c78d5ad - OKX DEX Theft/Laundry
- 0xfe55502a57f388a69602b2780071b759a520468f - OKX DEX Theft/Laundry
- 0x22a2931cb2a7b782d65b2b5562829e84d941b0f0 - OKX DEX Theft/Laundry

- 0x74d5c848afee3547fbd27810e4f5b5e05fefaa23 - OKX DEX Laundry, ETH
- 0xe0f83f8fdcb6535a288938b90bf6a5f334a7d966 - OKX DEX Laundry, ETH
- 0xb0ac5cbde2054144450570ca685ff84cd8fd1f75 - OKX DEX Laundry, ETH
- 0xc2e656f7b7617c4c1b2a6df1803d633a2f35c728 - OKX DEX Laundry, ETH
- 0xe8a66a5862ba07381956449e58999db541e4de93 - OKX DEX Laundry, ETH
- 0x8094b97a1663b7b73d6c76811355a734ba6f4a1a - OKX DEX Laundry, ETH
- 0xb31a2196050a3b861c65f23e180e56ed51cf75d7 - OKX DEX Laundry, ETH
- 0x0c1f0233091d6ed371dc84a0ad1602209bca429c - OKX DEX Laundry, ETH
- 0x17865c33e40814d691663bc292b2f77000f94c34 - OKX DEX Laundry, ETH
- 0xfd681a9aa555391ef772c53144db8404aec76030 - OKX DEX Laundry, ETH
- 0x141f12ab25fcd1c470a2ede34ad4ec49718b5209 - OKX DEX Laundry, ETH

- 0xd8a3cc60bd5cf288cec7d302c2fed7f4309dcebd - OKX DEX Laundry, BSC
- 0xd8a3cc60bd5cf288cec7d302c2fed7f4309dcebd - OKX DEX Laundry, Polygon
- 0x9272ff2e2d0cd9589ffd5063735ec4e1c492df21 - OKX DEX Laundry, BSC
- 0xb31a2196050a3b861c65f23e180e56ed51cf75d7 - OKX DEX Laundry, AVAX
- 0x0a7642dde5ec4df78951b87e57bd706753118da2 - OKX DEX Laundry, Arbi
- 0x0a7642dde5ec4df78951b87e57bd706753118da2 - OKX DEX Laundry, Polygon
- 0x82cb1ee28176f85d991ddbcb2082e276d2a31c12 - OKX DEX Laundry, Polygon, BSC
- 0x0a7642dde5ec4df78951b87e57bd706753118da2 - OKX DEX Laundry, BSC
- 0x17865c33e40814d691663bc292b2f77000f94c34 - OKX DEX Laundry, BSC
- 0xfd681a9aa555391ef772c53144db8404aec76030 - OKX DEX Laundry, BSC

- 0x9272ff2e2d0cd9589ffd5063735ec4e1c492df21 - OKX DEX Laundry, Polygon
- 0xb2a722870178e92ba681236c77609214265d25d1 - OKX DEX Laundry, Polygon + BSC
- 0x4aa219587d24b4c9f8cda278b041d4ca59251282 - OKX DEX Laundry, Polygon
- 0xa39e76a2979928ef953c8a5347c24fc26c14228d - OKX DEX Laundry, Polygon
- 0x422657e54ea52490d61d728ed27911e13c8a0e23 - OKX DEX Laundry, BSC
- 0xebffcbd787d90a46822fe9f1a2b1a5132badcc02 - OKX DEX Laundry, BSC
- 0x4d2b465caf91198551b830361429adcec07467cf - OKX DEX Laundry, BSC
- 0x2f8faeaecac4c4a3d8ed487c4cf2d26e250bdaec - OKX DEX Laundry, BSC
- 0xa39e76a2979928ef953c8a5347c24fc26c14228d - OKX DEX Laundry, BSC
- 0xaabc9e5fb0b9d2e64de1e9dcf8fcce709d9f81e0 - OKX DEX Laundry, BSC
- 0x38be86d46c8b8fba115f26231581ff3291bd7122 - OKX DEX Laundry, BSC
- 0x0d1712a7d4eaf64c134701acd672f4904784033b - OKX DEX Laundry, BSC
- 0xa62dbc185b8983eb5df4984414ba3f3562361e06 - OXK Dex Laundry, ETH

- 0x1db4d664d818d4c710d0aeb2d7d6b3ad885a8f19 - Thefts from Compromised Keys
- 0x22d833d1034dbd09c83ae834bf333a09bdfba316 - Thefts from Compromised Keys
- 0xffddaceac03fcc578eabce05425cc9649531efd7 - Dust
- 0xa62dbc185b8983eb5df4984414ba3f3562361e06 - Dust
- 0xeb982159ec32b601b6201a0553a05745a14e8f6c - Dust

- 0x2eD65De2823676d315ec034d4c549BB3F0a846AE
- 0x9ada20B835Aa178813A8C174F1F93B1dc1BFA775
- 0x67CF820F5cBd7B710A346d139E954f93C984111C
- 0x5633C37C48806a662341c2f509774731882Ea91D
- 0x83461A5429779Be0A089E8F94d6C9b7064C90Ad1
- 0xedb868e95c2d123d264be2b02bf4a19f891f87f6


Malicious Transactions:
- https://etherscan.io/tx/0x7a9c03576158b08bd896293fffcb11dd2fcc09c3d896335affee9968b4a1db5c
- https://etherscan.io/tx/0x78bfe55b18e53513b5c17869f39cc9cc21f3d6d2b6b44d1ceb9762789449dcd2
- https://etherscan.io/tx/0xf69cf6cc56849be0ee93e8651fdf3622639b7a99e1a620c744f3fef8a5743236


## Deposits to Railgun

- 0xd8f5c2d55f11ca0e8763019350ab7e77cbe9c425 $130k (Upwork / npm)
- 0xa62dbc185b8983eb5df4984414ba3f3562361e06 $80k (OKX Dex)
- 0x41153344260678596bb8c4f4f017caf48e440ff2 $80k
- 0x141f12ab25fcd1c470a2ede34ad4ec49718b5209 $86k (OKX Dex)
- 0xbbea72b68138b9a1c3fec2f563e323d025510a4c $73k (OKX Dex)
- 0xe152d7a03bf08ae4c854a8503a640dca80dd1d5e $21k
- 0x4a0cf014849702c0c3c46c2df90f0cad1e504328 $113k
- 0xe8b57d2aafb55ea673b1cd3930ab3c523f7f49d0 $71k
- 0xd54bc609fba8da4a8f33975457b887ac14e74f75 $97k
- 0x8b2a8fad289eb9b8d0e9c81fb7f803b00bc91878 $306k
- 0x7be76a223d8537e61f42b90957cf20c6d662c10e $46k
- 0xfcac7a9d0356d2370fb7e8425d8c88678f637ede $190k
- 0x8dc4d3785906d989c928c1a14fb6f85a7d571701 $63k
- 0x34b18e6e5fe7c639f672dd9f3d061c325e6fb942 $57k
- **Total: $1,500,000**

- Total Accounted For: $751k

## Withdrawals from Railgun

- 0x956cfd206dd1bd2b684efb969ec11713b476a9b7 $45k
- 0xccbbf5dbd0570a56594bd1cfa58b8fec8953fcbb $61k
- 0x0049507cbabd96702d9e6e047c54d1777b61a32d $87k
- 0xaae73f76a0f775602e4824c3a26c89a3b67eea20 $80k (Paxful Depo)
- 0x076715d27eeeae29a0093bfa0660431493c958bf $21k
- 0xfbcea750b14d2906fbe2e627cbf4ee89582f64ce $185k
- 0x5633c37c48806a662341c2f509774731882ea91d $160k
- 0x4f6c04117395bfbbadd991f82a464d7454b669a1 $67k
- 0x3cbc9e4b4e601a2ff6bb6eac6f1008369e2d3fb9 $236k
- 0xb2e2c9f088bc959e4d09e271066b5cbd4f664760 $234k
- 0xb86927e481b4ca99218a1303dbc754f39cd9bef7 $105k
- 0xb250861f4e64ea7bfb270502b969811f05f7c997 $56k
- **Total: $1,337,000**


- 0x4dc6111e2d1d4ce3e9627dfeba0863a03cd0c23a Paxful
- 0xac367fe52fb52f3b6e81c8125656d276eba740d4 Paxful 
- 0xaae73f76a0f775602e4824c3a26c89a3b67eea20 Paxful
- 0x3c4309a418ea99a495eb5d5754810f91627d9a8c Paxful
- 0xac367fe52fb52f3b6e81c8125656d276eba740d4


## Connections

> The OKX exploiters' address was eventually funded from 0xeb982159ec32b601b6201a0553a05745a14e8f6c at transaction  0x4c3cfdf935aef79d46510c86bad7c5099dc7ca04d5d002ba1f9abd05769132c5.
> The second OKX exploiter wallet 0xFacf375Af906f55453537ca31fFA99053A010239 rx'd funds via 0x9ada20B835Aa178813A8C174F1F93B1dc1BFA775 6 days ago, a wallet linked to the UNO hack. Further links can be established to FixedFloat, Binance, Gate, Mexc and Changenow.
> Other wallets with identifiers include 0x83461A5429779Be0A089E8F94d6C9b7064C90Ad1 who is the owner of rabit.blockchain, rabit.wallet, and rabit.nft UD this address sends funds to 0xedb868e95c2d123d264be2b02bf4a19f891f87f6, linked to 0x2eD65De2823676d315ec034d4c549BB3F0a846AE and eventually back to 0x67CF820F5cBd7B710A346d139E954f93C984111C, a wallet that transferred funds directly to OKX exploiter 0xFacf375Af906f55453537ca31fFA99053A010239
- https://twitter.com/0xKoda/status/1735068052381901261
- https://twitter.com/0xKoda/status/1735068052381901261/photo/1
- https://twitter.com/0xKoda/status/1734786009517510957