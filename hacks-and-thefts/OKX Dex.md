# OKX Dex

Date: December 12, 2023

Amount Stolen:: $2,390,976 (142k USDT + 475k USDC + 799.77 WETH)


## Description

- OKX DEX, a trading aggregator for cross-chain transactions, experienced an access control exploit on December 12, 2023
- The proxy admin owner upgraded the DEX proxy contract to a new implementation contract, which may have led to the compromise of the private key of the OKX DEX. 
- The stolen native ETH was distributed between three addresses, while the rest of the stolen stable coins were bridged to Arbitrum and Avalanche chains via Stargate Bridge.
- The DEX proxy was removed from OKX's platform's trusted list following the incident. 
- When users exchange, they authorize the `TokenApprove` contract, and the DEX contract transfers the user's tokens by calling the TokenApprove contract.
- The DEX contract has a `claimTokens` function that allows a trusted DEX Proxy to make calls, with its functionality being to invoke the `claimTokens` function of the `TokenApprove` contract to transfer tokens authorized by the user. 
- The trusted DEX Proxy is managed by the `Proxy Admin`, and the Proxy Admin Owner can upgrade the DEX Proxy contract through the Proxy Admin. 
- On December 12, 2023, at 22:23:47, the Proxy Admin Owner upgraded the DEX Proxy contract to a new implementation contract through the Proxy Admin.
- The new implementation contract's functionality is to directly call the `claimTokens` function of the DEX contract to transfer tokens. Subsequently, attackers began calling the DEX Proxy to steal tokens. 
- The Proxy Admin Owner upgraded the contract again at 23:53:59 on December 12, 2023, with similar functionality, and continued stealing tokens after the upgrade.
- This attack may be a result of the Proxy Admin Owner's private key being leaked.


## Links

> The OKX exploiters' address was eventually funded from 0xeb982159ec32b601b6201a0553a05745a14e8f6c at transaction  0x4c3cfdf935aef79d46510c86bad7c5099dc7ca04d5d002ba1f9abd05769132c5.
> The second OKX exploiter wallet 0xFacf375Af906f55453537ca31fFA99053A010239 rx'd funds via 0x9ada20B835Aa178813A8C174F1F93B1dc1BFA775 6 days ago, a wallet linked to the UNO hack. Further links can be established to FixedFloat, Binance, Gate, Mexc and Changenow.
> Other wallets with identifiers include 0x83461A5429779Be0A089E8F94d6C9b7064C90Ad1 who is the owner of rabit.blockchain, rabit.wallet, and rabit.nft UD this address sends funds to 0xedb868e95c2d123d264be2b02bf4a19f891f87f6, linked to 0x2eD65De2823676d315ec034d4c549BB3F0a846AE and eventually back to 0x67CF820F5cBd7B710A346d139E954f93C984111C, a wallet that transferred funds directly to OKX exploiter 0xFacf375Af906f55453537ca31fFA99053A010239
- https://twitter.com/0xKoda/status/1735068052381901261
- https://twitter.com/0xKoda/status/1735068052381901261/photo/1
- https://twitter.com/0xKoda/status/1734786009517510957
- https://twitter.com/okxweb3/status/1734794114657657004
- https://twitter.com/AnciliaInc/status/1734795426572980696
- https://twitter.com/WuBlockchain/status/1734784767760195671
- https://web3isgoinggreat.com/?id=okx-dex-hack




## On-Chain

- 0x1f14e38666cdd8e8975f9acc09e24e9a28fbc42d - OKX Dex Exploiter
- 0x2eD65De2823676d315ec034d4c549BB3F0a846AE - OKX Dex Exploiter
- 0x9ada20B835Aa178813A8C174F1F93B1dc1BFA775 - OKX Dex Exploiter
- 0x22a2931cb2a7b782d65b2b5562829e84d941b0f0 - OKX Dex Exploiter
- 0x67CF820F5cBd7B710A346d139E954f93C984111C - OKX Dex Exploiter
- 0x0519efacb73a1f10b8198871e58d68864e78b8a5 - OKX Dex Exploiter
- 0x5633C37C48806a662341c2f509774731882Ea91D - OKX Dex Exploiter
- 0x83461A5429779Be0A089E8F94d6C9b7064C90Ad1 - OKX Dex Exploiter
- 0xB2a722870178E92BA681236C77609214265d25D1 - OKX Dex Exploiter
- 0xFacf375Af906f55453537ca31fFA99053A010239 - OKX Dex Exploiter
- 0xa15fe801dd5fd31a684c444b6980dbaf0c78d5ad - OKX Dex Exploiter
- 0xedb868e95c2d123d264be2b02bf4a19f891f87f6 - OKX Dex Exploiter
- 0xfe55502a57f388a69602b2780071b759a520468f - OKX Dex Exploiter


Malicious Transactions:
- https://etherscan.io/tx/0x7a9c03576158b08bd896293fffcb11dd2fcc09c3d896335affee9968b4a1db5c
- https://etherscan.io/tx/0x78bfe55b18e53513b5c17869f39cc9cc21f3d6d2b6b44d1ceb9762789449dcd2
- https://etherscan.io/tx/0xf69cf6cc56849be0ee93e8651fdf3622639b7a99e1a620c744f3fef8a5743236


Stargate Bridging Transactions:
- https://etherscan.io/tx/0xd2b424b17e0959d260df748ef9d8b62120abe64d011ae68e00e8d3874d99ed28
- https://etherscan.io/tx/0x444fe10b2487c2c3cfa79fd878f3c0c5f520a9b4e94a44a6ce8e5a2bd8d9dd8b



# Upwork Crypto Developer Job Scams

IT Workers

The following is related to exploits with OKX Dex, UnoRe DAO, Arbi, Terraport, etc. etc.


## On-Chain

- 0x964891e39275280f731ccf9f3f42ab72e86739ad
- 0x89dc4eabade33dcf6b0a1166348802dc24ee16f7 
- 0xd8f5c2d55f11ca0e8763019350ab7e77cbe9c425


## Deposits to Railgun

- 0xd8f5c2d55f11ca0e8763019350ab7e77cbe9c425 $130k
- 0xa62dbc185b8983eb5df4984414ba3f3562361e06 $80k (OKX Dex)
- 0x41153344260678596bb8c4f4f017caf48e440ff2 $80k
- 0x141f12ab25fcd1c470a2ede34ad4ec49718b5209 $86k (OKX Dex)
- 0xbbea72b68138b9a1c3fec2f563e323d025510a4c $73k (OKX Dex)
- 0xe152d7a03bf08ae4c854a8503a640dca80dd1d5e $21k
- 0x4a0cf014849702c0c3c46c2df90f0cad1e504328 $113k
- 0xe8b57d2aafb55ea673b1cd3930ab3c523f7f49d0 $71k
- 0xd54bc609fba8da4a8f33975457b887ac14e74f75 $97k
- Total Accounted For: $751k

## Withdrawals from Railgun

- 0x956cfd206dd1bd2b684efb969ec11713b476a9b7 $45k
- 0xccbbf5dbd0570a56594bd1cfa58b8fec8953fcbb $61k
- 0x0049507cbabd96702d9e6e047c54d1777b61a32d $87k
- 0xaae73f76a0f775602e4824c3a26c89a3b67eea20 $80k (Paxful Depo)
- 0x076715d27eeeae29a0093bfa0660431493c958bf $21k
- 0xfbcea750b14d2906fbe2e627cbf4ee89582f64ce $185k
- 0x5633c37c48806a662341c2f509774731882ea91d $160k
- 0x3cbc9e4b4e601a2ff6bb6eac6f1008369e2d3fb9 $96k
- Total Accounted For: $735k


- 0x4dc6111e2d1d4ce3e9627dfeba0863a03cd0c23a Paxful
- 0xac367fe52fb52f3b6e81c8125656d276eba740d4 Paxful 
- 0xaae73f76a0f775602e4824c3a26c89a3b67eea20 Paxful