# Polynetwork July 2023

Date:: July 1, 2023

Amount Stolen: ~$10,000,000 (shitcoins theoretical value puts this theft at about $34 billion though lol)

Tags:: 🍎 Applejeus

---

## Details

It appears they were able to manipulate one of the core pieces of logic that all the relayers/signers use called `side-voter`

https://www.virustotal.com/gui/file/471a086b71271ff8ad203f4c9330354a0900f56dbf68dffa192f3ce48f95afd0/details

This may or may not be where [the code shown in the screenshot here](https://polynetwork.medium.com/the-poly-network-exploit-analysis-b0a77aff6078) comes from.

It is also referenced in this code though so unclear if this is the side-voter code or where the code where they found `side-voter` referenced

It's unclear to me how exactly they did this as the repo itself is private / gone?

I was able to find what I assume is a clone of said repo here https://github.com/polynetwork/ont-voter (given the install instructions)

However this was many months after the attack so that really only sheds light on what the original side-voter code did and what all it may access etc

The screenshot included in their post-mortem is compiled code which means that the malicious code was either inserted via a malicious, targeted package or via code written directly to that codebase itself

I suspect it may be the former simply bc the code has both reference to an external c2 and a few layers of obfuscation, both of which are easily detectable if there is any code review whatsoever. 

However, its obviously possible they were allowing folks to push without basic peer review.

One of the observed IPs relating to this theft is a Russia TTK which has also been previously seen with DP/SQSQ.


## Signers

- 0x4c46e1f946362547546677Bfa719598385ce56f2
- 0x3dFcCB7b8A6972CDE3B695d3C0c032514B0f3825
- 0x51b7529137D34002c4ebd81A2244F0ee7e95B2C0
- 0xf81f676832f6dfec4a5d0671bd27156425fcef98 (not used)


## Attackers

- 0xe0Afadad1d93704761c8550F21A53DE3468Ba599
- 0x8E0001966e6997db3e45c5F75D4C89a610255b2E
- 0xdddE20a5F569DFB11F5c405751367E939ebC5886
- 0x4FbC021742A4664D1cf8e9d2730b8519B9Dcc523
- 0xD475747a4937a66Cc7D4a2c7eA7F6e827D0f7390
- 0xb69f28d84497107c2740471926cc258ba1b855e9
- 0xd26785b00c3c55e16adef88272113260f3a05892
- 0xf3066df075efbca47963e8e883e4055c02b0eb8a
- 0xc1bd2cba5d22442753f8f1b37663d419743d8f04
- 0xde4f68afa85bc0f3ace517edd1d340739a053109
- 0x56bfd55bf0c9af3df534991f2cc19dd3fd4c4ca8
- 0x8a782ff9894b670208ead3c65475c5ed399630ec
- 0xe5fa7e2aec791da10c5d5f397c4013e7c42ddab9
- 0xf5b6697cae8cd2f372f3f4e20d683bbaa7b4943a
- 0xbcac1c15afea9cd5a4879c8a476bc6494d544eb6
- 0x8fbb28385d11439f146f4567c9aa7754020ee84a
- 0x561226cd4acb38a677f5dfda8d444627dc3aa8e9
- 0xd4738340da5955e8fcfe8191eb6c1db6e2842205
- 0x78f42b87456e3da809697c52c3f449f494f9126d
- 0x3f9eddd144e7f2ebb2c9fbbe64370bb3e7860067
- 0x8f3c6ba00878ed1eae7d47bd0c2d9d4dd0a2d020
- 0xe43896d3465d8da600d36278311b7afea1e04f65
- 0x481a3bfa0beae3b205ec92d7e09f1ada8d7036e1
- 0x40f3494138d33eb994747de482e58809ad772930
- 0x3c1c4beb2c90b32b7c6f269bfa026544ce7e9593
- 0xe38eb2d09a3ab3aea2c008e1d77605cebeda3ff6
- 0x988d681153a318bd9c88a51ec07a77fc44df5bc2
- 0x0236b55862ca10c1142f36a3450d7a4ceec9cfb9
- 0x89b214f632b109d86ad94fff6c6c15444799069b
- 0x23f4ca51aa75d9d3f28888748d514173394cc671
- 0x2f6c25e3c93c0fc7fdde2ece8e370ae152a57b82
- 0x3d66756be05b9a54138530c3e5103a7a489e7047
- 0xc8ab4aa93949c377c32c069272425bd42738c42f
- 0xdbda0c0cd018fc5466dbd57823ce81a93805874d
- 0x767ec1183eab2d3c90162d95bb9f1d282d65fc71
- 0x924ca257ca304e39b0ff559a4e6b1a51e689dc9c
- 0x11c924f0b50c51cbf9ac31a20365a38f24d4a4e8
- 0xcc2bb79b9413150f389c0cc2c646c6904f69f7af
- 0x32380bf820a2fdd5a2384c5b1c4c31343e0ecb61
- 0xb491d5b773156362c355fa8b1ce4bb94e8173baf
- 0x8537180a2168762baf10cf712fc52428d6d9d69d
- 0x88452d6fdfb804becea4a19a63f83441a1ceb3d1
- 0xfd3e731aff8b930337302f26eef015cfa022b778

### ETH

- 0x0dfeb429166e629204aca66467484cd88cb9701c - gas giver eth
- 0xe19e22dacc3a90b3919c45017b5fc7966c6d5776 - Calls exploit
- 0x63e1e406bc4e8a678dd8b563cbc5d1aaa76bff96 - Calls exploit
- 0xa5521e72d13e9377af0b87f48d5612d28d69745e - Calls exploit
- 0xabc4fd4cd0dc01e5216089f54c1a72d219073b1d - Calls exploit
- 0x4773c5b6ac10907f9829c4bc4461da56eedf0518 - Calls exploit
- 0x09d33e1c8633706b632827077890ce243ba75bdd - Calls exploit
- 0x36bc76bd36bb851bad29d5b490936a9b1e2c7b9a - Calls exploit
- 0x92c8d8df4298e156f2eec86802d509c44223b8e7 - Calls exploit
- 0x400b95f59d81dfa4d534b89c26713ddac4ed97b0 - Calls exploit
- 0x9e4fe5eaa9df5f8525697aff6c119298db832bc6 - Calls exploit
- 0x3f380a456276a8399fc743b00206ba5a5106e738 - Calls exploit
- 0x2eda32e232f7ae12d1863b63e4b082257bc6184c - Calls exploit
- 0x79f365e893ca06d42a6fe5f33e849c72cf7bcd70 - Calls exploit
- 0xa128ab842253bfa9e5a22da6de275874b0645ad6 - Dormant
- 0xb491d5b773156362c355fa8b1ce4bb94e8173baf - Dormant
- 0x6c215ef1b17ae48b29a31348a36c14d89343cd68
- 0x211ae110e2318c7cfa9391b390e5021709218d12 - Receives Funds
- 0x1417ba048c1fb874b00f519d5ef68e8955bbe729 - Receives Funds
- 0xf3066df075efbca47963e8e883e4055c02b0eb8a - Receives Funds
- 0x6c215ef1b17ae48b29a31348a36c14d89343cd68 - Receives Funds
- 0xcc2bb79b9413150f389c0cc2c646c6904f69f7af - Receives Funds
- 0x9e98612e0abb4e2034d2de7f23cf56644e56f89b - Receives Funds
- 0xbcac1c15afea9cd5a4879c8a476bc6494d544eb6 - Receives Funds
- 0x5979fbfe759f77287b4f8129cd3949d6bd87a9f9 - Receives Funds
- 0x8d62f78a18ab68c7808183609b25b29e476b3573 - Receives Funds
- 0xe5fa7e2aec791da10c5d5f397c4013e7c42ddab9 - Receives Funds
- 0x85ef23553eae46ee8759ee347d2b2fb1ee99bb60 - Receives Funds
- 0xbf6302cbb051e1579fe0ee116daf708739ca4ae6 - Receives Funds
- 0x8d72f9597571b6f1ba416beff61ef204732446a7 - Receives Funds
- 0x56bfd55bf0c9af3df534991f2cc19dd3fd4c4ca8 - Receives Funds
- 0x014601788fc6fad7e0febfb42b51a4b28b573e22 - Receives Funds
- 0x5e194eff9d3533e20e090350669080378973d176 - Receives Funds
- 0xf019aa6bc0b81cc4c1c04a0357b06d9cf93fcc7d - Receives Funds
- 0x4f2eb166c06c042c34f45069f945c55a78388756 - Receives Funds
- 0x88452d6fdfb804becea4a19a63f83441a1ceb3d1 - Receives Funds
- 0xc8ab4aa93949c377c32c069272425bd42738c42f - Receives Funds
- 0xfd3e731aff8b930337302f26eef015cfa022b778 - Receives Funds
- 0xcc92506d7824395583978f3374bbb828c4b965e0 - Receives Funds
- 0x21f1628f288fc54c61284cfdc8275daf7d057118 - Receives Funds
- 0xb69f28d84497107c2740471926cc258ba1b855e9 - Receives Funds
- 0x38ad785acf804c070a2dec73cfbf85f4c08fd913 - Receives Funds
- 0x3f7ad10096c36a21bbe679e3f957c7fe7c60ccb2 - Receives Funds
- 0x712d243e558f7a6d7f6e14348b5ddf02255a28a7 - Consolidation
- 0x087bdca684585a433e5750b42dabb3f1e160c097 - Consolidation
- 0x834bb1447f302dbc0cfc9d7cd7d4f23be295c6c3 - Consolidation
- 0x1222daa8ad5fa47238c857bbb278a43aaa582e36 - Consolidation

### BSC

- 0x1634Bf68e6b3Bb8D79388EfB3d1A5215506FBbEd - gas giver bsc


### Polygon
- 0x09F92eDce2E46C399BFE7881a7619598AF8436d5 - gas giver polygon
- 0x55aba51912e14dde79028eaae27ecfeafdc10c89
- 0x1bdc7e0e43699a3bdf1a61c389960cebe86e575f
- 0x26d3b81ac45a03b8cead79d52b633da57c513447
- 0x2d0b7efe74066709e63903f79e5468093754233c
- 0x96db9a29b66428b0e3d3c323edbfcb1cf40c837e
- 0x0583dcacbce66139fc2fdbbe5c0e745b014f860f
- 0x12a825a99b22dd1854474d8e0002af5e27194e15
- 0xd83b70bce8c0fe6ee82ee6598eb5f25590f6026b
- 0xc1bd2cba5d22442753f8f1b37663d419743d8f04
- 0x89b214f632b109d86ad94fff6c6c15444799069b
- 0x3744af4dea8e89be1f0de83352cb0dddcf493f3a
- 0xd20ae6250bac194bdc5ef21140fdfa35bd58ff7e
- 0x561226cd4acb38a677f5dfda8d444627dc3aa8e9
- 0xee8c2aca13d8e8f0517e745c2c0289ebf6139f1f
- 0x9450c9131e4ca9467272ba9eab2d6c337fb0f5ac
- 0xda85fa9b2606f6cf271064fa57276f9b0b0d6755
- 0xe0afadad1d93704761c8550f21a53de3468ba599
- 0xfbe3588dfd70bc4ab21bfa83ed7f8f3f17d3013b
- 0xe5fb77fac1ccaa2b6dac50586ebc8054f4dc9784
- 0xa7f399bc78cd7452a53f948102a4743e8ff1876d
- from FixedFloat


### AVAX

- 0xe0afadad1d93704761c8550f21a53de3468ba599
- 0x16b63311111ab05df32156f65e5dd57fcb1b9067
- 0xb3427393e405a73b4dad1dbd9cbbe64ba068131d
- 0xe6826a6f65005e56e5a54b15e03c3320cffe8ac8
- 0x4abae49bc91aa5672b8691840c7419d442aaad0b
- 0xaf4560b5c976be5a17e986a3fce1e661bf09cab2
- from FixedFloat 0x84130f0ba12808d4173df0939869b4888f50277bd5436e34fbe1ee1496ac6dea

### Arbitrum
- 0xe0afadad1d93704761c8550f21a53de3468ba599
- 0x8ef35fcc2c2f97b894649a7da1b250a64491ac6f
- 0x00b724c3670776f7073db1038ccc981d9755bd96
- 0x90f1f1c37314bd137a3ebc866dbfe3facc7f929f
- 0x4b6c5dfc9b67de3ec1dfb2f68e4929bcd54c6b02
- from ChangeNOW 0xacd22fb3805b94c030dff10c11a22191293879cbf1c9556d660ada8a43639d05
- 0x2de7f660ebb78252f7cc243bb2e35c558e43b58e Dormant

### Optimism

- 0xe0afadad1d93704761c8550f21a53de3468ba599
- 0xb89aa92a388466dd144d59ce1625565b99b2a1c8
- 0xa55cf585e3acbaf3bc487f81f55cb63f076a636b
- 0xabe51d35316efd1eb3b7c9473fd0b85c0cc6e0b2

### Fantom
- 0xe0afadad1d93704761c8550f21a53de3468ba599
- 0x2f1fb4fb671a35eeb92ae7af9ff147a351c4d483
- 0x5e8196d62a2b32063b2730102bdcbb116266adda
- 0x2ca62ebad90428457142132544d15a218aa46677
- from FixedFloat 0xcad1e6451625448e93b9869992fb3f59c61ff0bf07d6cf94a3ccc46d951de7ae


### Tornado Cash Deposits

| Address                                    | #   | Amt    | Amt | Asset | First Seen       | Last Seen        |
| ------------------------------------------ | --- | ------ | --- | ----- | ---------------- | ---------------- |
| 0x2f6c25e3c93c0fc7fdde2ece8e370ae152a57b82 | 32  | 1556.6 | 0   | ETH   | 2023-09-27 15:08 | 2023-09-27 15:44 |
| 0xdbda0c0cd018fc5466dbd57823ce81a93805874d | 18  | 1500   | 0.3 | ETH   | 2023-09-11 04:40 | 2023-09-11 05:02 |
| 0x3d66756be05b9a54138530c3e5103a7a489e7047 | 21  | 1371   | 0   | ETH   | 2023-09-19 06:56 | 2023-09-19 07:38 |
| 0xc8ab4aa93949c377c32c069272425bd42738c42f | 21  | 1253.1 | 0   | ETH   | 2023-10-12 01:08 | 2023-10-12 01:29 |
| 0x32380bf820a2fdd5a2384c5b1c4c31343e0ecb61 | 6   | 301    | 1.1 | ETH   | 2023-10-11 03:34 | 2023-10-11 03:52 |
| 0xe0afadad1d93704761c8550f21a53de3468ba599 | 1   | 0      | 1   | ETH   | 2023-07-01 13:50 | 2023-07-01 13:50 |


## URLs

- https://dedaub.com/blog/poly-network-hack/

- https://polynetwork.medium.com/the-poly-network-exploit-analysis-b0a77aff6078

- https://www.serial-coder.com/post/poly-network-in-depth-analysis-of-the-biggest-heist-in-defi-history/



