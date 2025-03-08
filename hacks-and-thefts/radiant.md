# Radiant Capital

Date:: October 16th, 2024

Amount Stolen:: $50,000,000

Tags:: 🍎 Applejeus

---

## Details

Radiant Capital posted on X acknowledging issues with its lending markets on BNB Chain and Arbitrum. Trading on Base and Mainnet markets has been paused. According to SlowMist’s security team analysis, the incident occurred after the Radiant attacker illegally gained control of 3 multisig permissions and upgraded to a malicious contract to steal funds.

> Within the ZIP file, the attackers delivered a sophisticated piece of malware — INLETDRIFT — contained within Penpie_Hacking_Analysis_Report.zip. It established a persistent macOS backdoor while displaying a legitimate-looking PDF to the user. It employed a malicious AppleScript to communicate with the domain atokyonews[.]com.

> Mandiant attributes this attack to UNC4736, commonly referred to as AppleJeus or Citrine Sleet. Mandiant assesses with high-confidence that UNC4736 has a Democratic People’s Republic of Korea (DPRK) nexus. Specifically, this group is aligned with DPRK’s Reconnaissance General Bureau (RGB) and has close ties with TEMP.Hermit.

Add'l Signers: 

- 0xbbb33DE35C4489e98965945b088Ea5361Df9eb26
- 0xD0A16E09d8B0D77503C5f3eC05287B06C6C6cfCF
- 0x0c75Fa5a5F1C0997e3eEA425cFA13184ed0eC9e5
- 0xe1c6AED39d02d0898a72C77a3b8E29810dfb0140 (New)
- 0x7E733Bed445460b5F67929594C3B16eD450f8E89 (New)
- 0xBc565990D1b406C0cB6f458B60aD29a8ebd0CE52 (New)
- 0x28a664Bd3962eec459B6f3477E0EeADC1fa0B926 (New)

## Onchain

### SAFE Transactions

- The transaction they wanted to sign: https://app.safe.global/transactions/tx?id=multisig_0x111CEEee040739fD91D29C34C33E6B3E112F2177_0xc5848ce13112f5637d1831e8388b11120f4a6edc772abbb993c2f91cc09d9dc7

- API Version: https://safe-client.safe.global/v1/chains/42161/transactions/0xc5848ce13112f5637d1831e8388b11120f4a6edc772abbb993c2f91cc09d9dc7

- The transaction that actually got broadcasted: https://app.safe.global/transactions/tx?safe=arb1:0x111CEEee040739fD91D29C34C33E6B3E112F2177&id=multisig_0x111CEEee040739fD91D29C34C33E6B3E112F2177_0x5c28ef88f6696dd8c5c5e4ba5632374d5de9e6cb9ebf75884332f29ef9fad416

- API Version: https://safe-client.safe.global/v1/chains/42161/transactions/multisig_0x111CEEee040739fD91D29C34C33E6B3E112F2177_0x5c28ef88f6696dd8c5c5e4ba5632374d5de9e6cb9ebf75884332f29ef9fad416


### Attacker

- Attack Transaction on BSC: https://bscscan.com/tx/0xd97b93f633aee356d992b49193e60a571b8c466bf46aaf072368f975dc11841c

- Attack Transaction on ARB: https://arbiscan.io/tx/0x7856552db409fe51e17339ab1e0e1ce9c85d68bf0f4de4c110fc4e372ea02fb1

- 0x57ba8957ed2ff2e7ae38f4935451e81ce1eefbf5 - Malicious Contract + New Owner

- 0x3c2bc83dcd293cc8a23526a37aaeedd83ebd62de - Other Malicious Contract

 - Testing on ARB: https://arbiscan.io/tx/0xab34055320676b35d4c6c5936dabc4101b45eda0d66b94ee02f10a96e8a1dd45

- 0x57ba8957ed2ff2e7AE38F4935451E81Ce1eEFbf5 Attack Contract

- 0x0629b1048298AE9deff0F4100A31967Fb3f98962 Other Multisig Deployer

- 0x0629b1048298AE9deff0F4100A31967Fb3f98962 Primary Attack Funds Receiver 1 - Sep 27 Oct 02 Oct 10 Oct 14 Oct 16 - ARB BSC BASE ETH

- 0x9c5939aac4f65a0ea233e657507c7b54acde2841 Attacker Funds Receiver Oct 16 Oct 16 BSC

- 0xa0e768a68ba1bfffb9f4366dfc8d9195ee7217d1 Attacker Funds Receiver Oct 16 Oct 14 Oct 16 BSC ARB

- 0x961a19d16db31add5e257bc3d73b403ee0d3680e Attacker Funds Receiver Oct 18 Oct 18 ETH

- 0x8B75E47976C3C500D0148463931717001F620887 Attacker Funds Receiver Oct 16 Oct 16 ARB ETH

- 0xb7779da5386db9163be64a46a1a2341a08dfa445 Bridges Out Arb Oct 18 Oct 18 ARB
- 0xba7044917b5baebf58ff0f08fe44dd4b5100cd7c Oct 18 ARB
- 0x9fe47731361e3f4f654429886843bde735c58ca3 Oct 18 ARB
- 0x2daba958d7b3df6ebb880bbf4607765f7e9ea6d5 Oct 18 ARB
- 0xdeeb7a9816be8e3af002c1e7eda9bbd48e3c008e Oct 18 ARB
- 0xcc50124dbf947718595f2922f536320558cafbfe Oct 18 ARB
- 0x9f309b26c789058dfbdc40c88afe9fde67db51c3 Oct 18 ARB
- 0xd26083aa477489e7e5e7740a550485b49e52594c Oct 18 ARB
- 0x3e6e2e6331ced6c83352ca2133427cf8dd494659 Oct 18 ARB
- 0x94b8d2daeddd59677a6c5cf395a80872e568bb46 Oct 18 ARB
- 0xf67f9924b85ba893ac7427b122a6ab38dd3040cd Oct 18 ARB
- 0x150003cb3480ba279ee2e614c41edada55753bb1 Oct 18 ARB
- 0xb20aa942bd2851d34a84e32606036e8cfae17f80 Oct 18 ARB
- 0x3b06bcab1edbcb8dc8e05734be34ae78b33e9fae Oct 18 ARB
- 0xef453951f699f146b8b7d0e5b1ea2b8b59df4f5e Oct 18 ARB
- 0xc5e93c13cca02772553bb98cf223480dff1019bc Oct 18 ARB
- 0x4afbd65e78bf55cf95b6d4699f0edfe4cd180b6f Oct 18 ARB
- 0xdEcF6C2Ee70D2b96f55073331347BdF6f8D25668 Oct 18 ETH
- 0x491C24A82c0B042cF34Bfa59e340aFf5F98b44b1 Oct 18 ETH
- 0x803536aad020da0a27b36aa2a847867070276045 Oct 18 ETH
- 0x5b9aa4832af1d559ee29053403e9b94e242b534c Oct 18 ETH
- 0x118452da70dfd9267145dcf1b17837e9a4b991ba Oct 18 ETH
- 0x7695312efdbcd949f66440f24594da42bfa3b870 Oct 18 ETH
- 0x010ae218aF35Beb83A2eEB05dFba30DC18575c12 Oct 18 ETH

- 0xc4173a794122644870c8fd07c226acf992507897 Attacker Funds Receiver Oct 17 18  BSC ARB
- 0x101f095b3978bc475bdb240e977521f513dfab28 ETH: Bridges in from ARB 0xC4173a794122644870C8fd07c226acF992507897, BSC: comes from Polynetwork Exploiter - 0x2c43a4d2eda4269f043951c42efac9ba63eeb884 Oct 18 ETH BSC

- 0x97a05becc2e7891d07f382457cd5d57fd242e4e8 Primary Attack Funds Receiver 2 Oct 16 ARB BSC ETH
- 0x911215cf312a64c128817af3c24b9fdf66b7ac95 Attacker Funds Receiver Oct 16 Oct 02 Oct 16 ARB BSC
- 0xcf47c058cc4818ce90f9315b478eb2f2d588cc78 Attacker Funds Receiver Oct 16 Oct 16 BSC
- 0x62dc783c63be0ea579fdb0922d25f15355d89041 Bridging Out Oct 19 BSC
- 0x73f07f6f32f6e0734c3d0c322dd01a6e7fb5a2da Bridging Out/In Oct 19 BSC
- 0x6a45c4f8bc174b7d5e4d61468bf5a3229aa004f1 Bridging Out/In Oct 19 ETH BSC
- 0x9c1ced1f5052145a42f38ace66d792a5687e3769 Bridging Out Oct 19 BSC
- 0x4ea96ecdca02210f3efd20d2e15151476da916ba Bridging Out/In Oct 21 ETH BSC
- 0x1ef8cbe2d8bda101bc22fedda2cfd0a169c4b269 Bridging Out Oct 21 BSC
- 0xb0457005efe908e4c82c5ebcba0561a77899bc84 Bridging Out/In Oct 21 ETH BSC
- 0xdd1c5f6da617f5afcd44e62c0fcacb54c06d6fac Bridging Out/In Oct 21 ETH BSC
- 0x7e5f04568957e367d03e1e926bdf1bb6c10434c7 Bridging Out/In Oct 21 ETH BSC
- 0xa991b0ce56246901d6084c00f15d056a9c4f9e71 Bridges In Oct 21 ETH
- 0x9beeecc34fad6367c991fd6b701fdc477e54ce34 Bridges In Oct 21 ETH
- 0x6a7af1b2077707886aa7f2e122cd819bddd50383 Bridges In Oct 21 ARB
- 0x589e8b991c2afd2d8d4def8f7f0cbf67073a9b19 Bridged In Oct 19 ETH
- 0x7997e80f4bd9563d61ee4d06108f7d6ceb23ab21 Bridges In from BASE 0x94b8d2daeddd59677a6c5cf395a80872e568bb46 Oct 21 ARB
- 0x4f97fd28f1b2b1a2e33f7f031fb6b9cc95871a7a Bridges In Oct 21 ARB

- 0x3d4c56cdb97355807157f5c7d4f54957f0e9af44 Radiant Exploiter Contract Oct 17
- 0x579145d6d1f26a460d9bdd3040c37517dac379ac Radiant Exploiter
- 0x5eb63694a18b618c4ebdd9ca3333fa7f9b8b9cb4 Radiant Exploiter
- 0xbc20e84d80a684daea4468be6f199a233a3d2363 Radiant Exploiter
- 0xb0fc65b29c4e8cc56de26e52ad26e7ac776c41fa Int Oct 18 BSC
- 0x070ca92f568037d351666b3918a0f6ba7ad20ed1 Approval Drainer, setBenefit in txn https://bscscan.com/tx/0x02a62f11b9042d3333e7b4ce8859eefab941190e0faeaca152414774803ede70  Oct 18 BSC
- 0xf4e49bd4d560b036dd6fe43850daad3b4f7b7849 Radiant Attacker Oct 14 BSC

- 0xcCfE10Cbc381dD6752fA34253a17e7e7c0cf7951 Test Multisig (3/3) Sept 25 BSC ARB
- 0xD899F3d8ff2A723642d5C55eD1998713C530b7b3 Test Multisig Deployer
- 0x84597A585028A74c783ACAdD4879329537304e45 Test Multisig Signer
- 0x4DF237b40088152c81406152A8a63a0841F4cdad Test Multisig Signer
- 0xECe8eBB0F1c31bE085C1Dd899299f01c0aEC95A1 Test Multisig Signer


- 0x3C2Bc83Dcd293Cc8a23526A37aaeEdD83eBd62de Other Multisig
- 0x0629b1048298AE9deff0F4100A31967Fb3f98962 Other Multisig Deployer

- 0x57ba8957ed2ff2e7AE38F4935451E81Ce1eEFbf5 Other Multisig - mentions 0xfedc4d6a71fc869e315b6a3e192725ddc92df5a - mentions 0x911215cf312a64c128817af3c24b9fdf66b7ac95
- 0x0629b1048298ae9deff0f4100a31967fb3f98962 Other Multisig Deployer

- 0xa5918f4b242F32CF6a47A3a631406734767533bD Other Multisig Oct 04 BSC
- 0x602B9Da1c4940391260114aB6EA54e71ed70a5B4 Other Multisig Deployer, receives from 0x602b9da1c4940391260114ab6ea54e71ed70a5b4  Sep 25 BSC

- 0x921b00fa38911337aed702fb4857877c1aca1141 Other Multisig Oct 02 ARB
- 0x0629b1048298AE9deff0F4100A31967Fb3f98962 Other Multisig Deployer Oct 02 ARB

- 0xa088f925989970efeeedc0f144d89d77f7124f16 From BSC, Oct 22
- 0x9032b2193596f753b59caa984fa9d8f696c349e6 From BSC, Oct 22
- 0x1db33559c4c928adfe51ebe89926379e5fd53d3e From BSC, Oct 22
- 0x5c2df5f14c15eff9f7d8dca8dd712f0eb3dcea99 From BSC, Oct 22
- 0xd306f84b1871a31fa1e8e357249ab321ca7c1aac From BSC, Oct 22
- 0x2b9ce9a16e918613d7a643615161707274d34508 From BSC, Oct 22
- 0xc4a2bd9185f4dd6f5c4731cd45c16b92ee92d1c1 From BSC, Oct 22
- 0xcd69d20b41fddbf1c37e51a590628367a742d50f From BSC, Oct 22


### Victim addresses (keys not compromised though)
- 0x111CEEee040739fD91D29C34C33E6B3E112F2177 (Safe)
- 0x20340c2a71055FD2887D9A71054100FF7F425BE5
- 0x83434627e72d977af18F8D2F26203895050eF9Ce
- 0xbB67c265e7197A7c3Cd458F8F7C1d79a2fb04d57


### Hyperliquid Depositors (Arbitrum)
- 0x00e1559184bf1da0256a495ae9baec11bca60eb7
- 0x1a7813975499a0deb04b09146d2285751072590f 
- 0x2de7f660ebb78252f7cc243bb2e35c558e43b58e
- 0x348fc4dfdcd3427d8a4b43ad965b4443d55cf955
- 0x34aa91e574aa963675107011dcf0392c5521005a
- 0x52263caec2e144c3a84cc16d014157360ac85a89
- 0x5b10daedc2d7b5ce47f6b3072188f758f1b14481
- 0x60aba279e49e5a05dc7e3c84f2204a6afb032119
- 0x7997e80f4bd9563d61ee4d06108f7d6ceb23ab21
- 0x9e045ef8712607c1d8d04e2eaa9a2781149d5cf8
- 0xd16c40c6b4abe94421e42c664efab33d0b6b6515
- 0xf48514487dd161b28109c7b1185b69e11b2dce63


## URLs

- https://medium.com/@RadiantCapital/radiant-capital-incident-update-e56d8c23829e
- https://rekt.news/radiant-capital-rekt2/
- https://twitter.com/hackenclub/status/1846624373161013388
- https://twitter.com/bantg/status/1847120310618767633
- https://twitter.com/AnciliaInc/status/1846605867753591002
- https://twitter.com/danielvf/status/1847023591117795708
- https://twitter.com/AnciliaInc/status/1846606649009885515
- https://twitter.com/RDNTCapital/status/1846634050100039881
- https://x.com/patrickwardle/status/1866586260049105409




## Relevant Bridges via Chainge Finance


| Timestamp           | Chain | Value         | Value USD | From                                               | To                                                 | Txn Hash                                                           |
| ------------------- | ----- | ------------- | --------- | -------------------------------------------------- | -------------------------------------------------- | ------------------------------------------------------------------ |
| 2024-07-20 8:42:59  | ETH   | 5             | $17,448   | 0x26bb9df242112940eb5ef0e61c494030351fc9ff         | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0xc62fe16ad1252d295e211b6734e33312c977341024284cad8407b369cdaeedcd |
| 2024-07-20 8:43:56  | BSC   | 29.49260828   | $17,443   | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0x94187bd7d88448585ef291fd3bea03ae67f9179a         | 0x0e8d2b708996fff8510039fd4c98486f7be24636e6b6a34c509c08239d4b681e |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-07-20 8:52:59  | ETH   | 0.1           | $349      | 0x26bb9df242112940eb5ef0e61c494030351fc9ff         | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x07234af92353451924a3fee5240378f5a73b99f400c939b4fcfbe0e8e4e668a1 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 2:45:32  | ARB   | 0.0099        | $24       | 0x9ee08404dafd085fc6dc678183164cf474b81f85         | CHAINGE 0xf422ec7591e83612a39dbdf94563f20133ef2d9f | 0xb16e6be2c86ae429cb158b311c66814cf13c7f396e6ab21d4dc6ab014c66f3ac |
| 2024-10-14 3:07:09  | BSC   | 0.04063936068 | $24       | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0xa0e768a68ba1bfffb9f4366dfc8d9195ee7217d1         | 0x4c9f998f2b6f2338e002efcd7a10a0430245abf1d4cb81e4f4e1c4e43eef9665 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 2:39:47  | ETH   | 2.43          | $5,970    | 0xdb0d54c00ee259ce6588bb426889466d1e471655         | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x71b9d69c8dd3f2c3514d9b9e774769496b14c7d2c6283f4330eb7f0c956893dc |
| 2024-10-14 3:34:18  | BSC   | 10.40161841   | $6,108    | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0xf4e49bd4d560b036dd6fe43850daad3b4f7b7849         | 0xb79f580876fd8c327a901d535206b424fc8ecde8426b9020a73575bfb65fd631 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 2:43:44  | ARB   | 60.28         | $148,105  | 0x9ee08404dafd085fc6dc678183164cf474b81f85         | CHAINGE 0xf422ec7591e83612a39dbdf94563f20133ef2d9f | 0x2b31728ceab537453fb8e11b37cf104aec15d953fdfa58ab4c6cb3e4d8cce133 |
| 2024-10-14 3:34:33  | BSC   | 257.8505452   | $151,410  | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0x9ee08404dafd085fc6dc678183164cf474b81f85         | 0xaa83b070ff301966ca53b2840833838fcb8b13d92a7c6e4df28266a78fc3a3ee |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 6:41:03  | BSC   | 6.06          | $3,558    | 0x25e49c69cb60022968a4cbd11144ec8a34e01cf3         | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0xd55b96d36977a8ab62f7881ffdae39907bf8092219170a30e45eb6a2d43f4431 |
| 2024-10-14 6:42:59  | ETH   | 1.381645604   | $3,395    | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x25e49c69cb60022968a4cbd11144ec8a34e01cf3         | 0x862f0ef743c5f236fdf31265aeb48825f510f44e7fda7c90f5e411c26b32e1b1 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 7:11:11  | ETH   | 3.04          | $7,469    | 0xf5e4ad3811821430690535ef7af7719ffe6ee9bc         | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0xe51c3089767bba8b2b24b7b2c6d5faa999a011c58456eb6cae2dd386c7bf145f |
| 2024-10-14 7:30:12  | BSC   | 13.1424395    | $7,717    | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0x767ec1183eab2d3c90162d95bb9f1d282d65fc71         | 0xf6f9552f294a10dfaccddc4fa86356857d7324831832087a30bc7b5ce94769a8 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-14 12:03:45 | BSC   | 42.12         | $24,733   | 0x23bf9a40b16e1b4e7ec3a18ee639649350eb34cd         | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0x1fe9a261b92e17a57c4958d82c33d731e8175b12d9f6f0533b74734e8d4a80ff |
| 2024-10-14 12:32:11 | ETH   | 9.597849915   | $23,581   | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x767ec1183eab2d3c90162d95bb9f1d282d65fc71         | 0xb9c74edcca600822e4102c0f59c44678e535851f8be32d7bfb58dec895a0439c |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-15 1:14:47  | BSC   | 73.29         | $43,214   | 0x8071bc1ccdfbfd098b91fc86fb21f2cb9d3cc221         | CHAINGE 0x99a57ac044e6ce44b7e161a07af0d3e693a75b54 | 0xb172d190e03480f4a9bc7ff686baa7198a0941119022847b4f7c912552365aea |
| 2024-10-15 2:37:47  | ETH   | 16.43382488   | $43,082   | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x767ec1183eab2d3c90162d95bb9f1d282d65fc71         | 0x002a8d5026f4cbd1867fc4ec91a4a7d74cdfa6ff12ef1710b47d7e6e2c79c091 |
|                     |       |               |           |                                                    |                                                    |                                                                    |
| 2024-10-16 14:12:05 | ARB   | 2.58          | $6,706    | 0xce22d25a8b37d85c82fa84073816e9ff2bb5ca73         | CHAINGE 0xf422ec7591e83612a39dbdf94563f20133ef2d9f | 0xe42f131294ad48fee78eda18e9dd822b7ed15acda7d63c1c9a1f0184d9969989 |
| 2024-10-16 14:12:59 | ETH   | 2.57550988    | $6,695    | CHAINGE 0x4c5f53015f3adb1b1d15ddf4e17edaae6fa185a5 | 0x0547cc38b8c121de761d394042c45166a811d0ff         | 0x0ec4c13d0683ba30b2fd6c3c2ec867353f02779236728fd6b62810a561c4df03 |
