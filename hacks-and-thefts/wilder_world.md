# Wilder World

Date:: March 16, 2024

Amount Stolen: $2,314,583

Tags: 🎙️ Contagious Interview

---

## Details - March 16

> On 16 March Wilder World had an unauthorized breach that involved 9 legacy vesting contracts. At 3:07 AM UTC 0x37358Aa5D051B434C23Bad744E56E6A484107272 (Zero Name Service: Deployer) transferred ownership of contract 0x6cA959fbc8e3df1fBeA5d9791De0047E1B3a57C6 (proxy) to 0x6584A486F711eB8aC47aBf78A5C8e218Ee758fa9 (attacker).

> The transfer of ownership then granted the malicious wallet permission as contract owner to upgrade the legacy vault contracts to new implementations that they deployed shortly before upgrading.

> The new implementations allowed the attacker to transfer the contract token balances

> The root cause is likely due to a private key compromise of 0x37358Aa5D051B434C23Bad744E56E6A484107272 (Zero Name Service: Deployer) which was used to change contract ownership. An investigation by Wilder World revealed that it was likely a previous contractor who had access to the private keys.

> A total of 515 ETH (~$1,814,583) worth of WILD and MEOW was taken from 9 contracts.

> The stolen assets were transferred to EOA 0x6584A486F711eB8aC47aBf78A5C8e218Ee758fa9. Despite Wilder World issuing a message to the exploiter to return funds the assets were swapped for ETH and transferred to EOA 0x7f0756D3aAAa6E8A34d29e6E8A7a78617d8fF662, where all 515 ETH was deposited into Tornado Cash.

–[Cerik](https://certik.com/resources/blog/private-key-compromises)


## Details - April 2, 2024

While investigating the GNUS Token Exploit, I traced back 63.47 ETH string of funds to the address 0xa75587029b13632dda5dc40711ebdfc5ddc6bfb5 which exclusively transacts on April 2, 2024. It receives from 0x7829afa127494ca8b4ceef4fb81b78fee9d0e471 ("Zer0 Name 1") and a few other addresses. 

Also on April 2, 2024 0x7829afa127494ca8b4ceef4fb81b78fee9d0e471 transfers the ownership of contract 0x0122a448E395cc9602019A2E2B9B7c841B1D61F4 to new owner 0xa75587029B13632dda5dc40711EbdFC5ddc6bfB5.

Also on April 2, 2024 0xee2e4fbe10a437e1b1561687d4e5133dd397ab96 (which also receives funds from both the Cloud AI and Murall exploits) receives $276k MEOW Token from 0xc33f704415384d63765e9200cbcfccf3536fe137


## Onchain - March 16

- 0xd393224e6ebbfb46c6a09a6fd8acc596f6392402 - Compromised Contract
- 0x956234670110d154abb591fb46fc3b5a455a3c97 - Compromised Contract
- 0xb7dfcb421412f16b25ddd4ad4bdd73d0883136d8 - Compromised Contract
- 0x8e4c057032436498817de977dc1ae10e3dfd23c1 - Compromised Contract
- 0x5521d7e4d9ae2294ecdf505fd138b8924ea7a8e2 - Compromised Contract
- 0xe516ef5d103bf567238db2a5f88781d18214ff6c - Compromised Contract
- 0x6e9c63af66e1f59137214d51ab7716e8db9d6467 - Compromised Contract
- 0x109f7b8608785201a9aaa4d75dbf03a9fa663187 - Compromised Contract
- 0x441b52f945b6f3e7d2019f2a0a3537dba1a7ef87 - Compromised Contract
- 0x37358Aa5D051B434C23Bad744E56E6A484107272 - Compromised Zero Name Service: Deployer - Transfers Ownership
- 0x6cA959fbc8e3df1fBeA5d9791De0047E1B3a57C6 - Compromomised Contract (had ownership transfered)
- 0x6584A486F711eB8aC47aBf78A5C8e218Ee758fa9 - Primary Theft (515.5 ETH)
- 0x7f0756D3aAAa6E8A34d29e6E8A7a78617d8fF662 - Theft -> Tornado Cash (515.5 ETH)


## Onchain - April 2

- 0x7f3a152f09324f2aee916ce069d3908603449173 - Compromised
- 0x621863fd50cad605f832c5f4989ada63b536b180 - Compromised
- 0x424d286589b7339867bb96e7984e2264f2d041bc - Compromised
- 0x52fc9eb1bcce87dfe70ca40f612899d1d202a139 - Compromised
- 0x00f665d2cff2ddb79bb370120480cf9ef334bc97 - Compromised
- 0x7829afa127494ca8b4ceef4fb81b78fee9d0e471 - Compromised (Transfers Ownership)
- 0x0122a448E395cc9602019A2E2B9B7c841B1D61F4 - Compromised Contract (had ownership transfered)
- 0xa75587029B13632dda5dc40711EbdFC5ddc6bfB5 - Primary Theft (63.47 ETH)
- 0xee2e4fbe10a437e1b1561687d4e5133dd397ab96 - Primary Theft ($275k MEOW)

- 0x17e604b5ac6ede6f548668359dad8e2ad76c94f9 - Sends 63.47 ETH -> 210k USDT to Consolidation 0xb40
- 0x633743f6c0b01bcffc010d253e1c7248d1aa7227 - Sends $23k to Consolidation 0xb40
- 0x8942b24177c7fc75dba186589cef30c482d55da9 - Sends 171.9 ETH ($554k) to Consolidation 0xb40

- 0xb40fef5db4c4e245abcdd7edcaf91d0b3ed34570 - Consolidation (Receives 210k USDT + 23k USDT + $554k ETH)

- 0xadcae70b7913cfc628be138ddd11cfc39ab99451 - Laundry (4 hops)
- 0xd104858af1b3f3b6aede8cd854808064eb6909a3 - Laundry (4 hops)
- 0x169e3749282e0e2eefae9895180e82d95531c42f - Laundry (4 hops)
- 0xb61031881b9320184421c3abc8bce7073964e6ff - Laundry - ETH -> BSC Stargate
- 0xa942f59708e32edc298b7b96428b9f4859b620b1 - Laundry - BSC from Stargate
- 0x587e172b116ea0c157ecfb0b479dfc825b465220 - Laundry - BSC
- 0x3f87f358f67916545721b930d181f8b853805c3f - Laundry - BSC
- 0xda581fdf12df38c5281ef73fcb7cf3b4d55e2f1b - Laundry - BSC
- 0x53b930155de610649e7a4ca07b84b7f936c48667 - Laundry - Polygon -> Defiway
- 0x1849a502eb1cc7329f9e703d4d5b129722384bf0 - Laundry - Polygon -> Defiway

- 0x1a25af691bbee954e1bd1fdf2414486d367457db - Laundry - BSC
- 0x1bb3ccca65ebfca4557c58081391b1c907fdd91c - Laundry - BSC to Polygon
- 0x71c99be4c01ba02ee5cf00d4e29e04781a015eaf - Laundry - Polygon from BSC, to Defiway
- 0x0cf9f7bd61d3df5de2728f69a88da91170ad6b13 - Laundry - BSC
- 0xd0f7ecf1580b607c3df7e7d9e9b3a611bbf2ab3f - Laundry - BSC
- 0xe8cd6d763e2a3813b0a49a61818623ece9d3dfef - Laundry - BSC
- 0x2d790b454d491e0f53f7a066f151f47bd7c6d0b3 - BSC to Polygon to Defiway
- 0xb1d901df78b5c8b47b2a1eeec526a3caa3a2e500 - BSC to Polygon to Defiway
- 0xd206c6be926126bfe8fb838d73068c0d5421d049 - BSC to Polygon to Defiway

- 0x582b199d1db02203f64458830fb09531a98d6f99 - From Changelly, BSC -> Arbitrum
- 0x7988104620d0d128e3abeeaf454538b47a44b74f - From 0x582 + Linkedin Job Scams
- 0x850ed0d8b8748c56e122870d9150efb2332646d4 - BSC -> Arbitrum

- 0x0f2ad7a72f72817a4be6f683cd0693163f2b9f1f - BSC -> Stargate
- 0xf74b7486f6f6ec82b2d7b3abf2b79ba948290fbf - Stargate -> Polygon
- 0xd75fee035fe076f4c43960a9fbc2fb9c389d7c7c - Polygon, $50k to Defiway, $150k continues on
    - 0xa6ba9a87f75d86449b76ff110ecd4a88e5996ff7 - Polygon, Laundry $150k USDT to BSC

- 0xbb823caa668b9de2317cf3c7be5277519f2ff257 - Laundry
- 0xe02a6d10ea3ef73fec6c87697e0ec07a8021617d - Polygon, from MEXC Apr 5 2024
- 0x3e2c1b98277fc061f8ca4868eee9309c61f33a1c - Polygon
- 0xda581fdf12df38c5281ef73fcb7cf3b4d55e2f1b - Polygon
- 0xf318d71541a072583ee2f3720b757afb604b4eca - Polygon, Laundry $70k USDT to BSC
- 0x7d9a5a198c3fc7caa947f3d8376d2d5d26de14ac - BSC, from Polygon, to Defiway
- 0x3012a1294ade42dd131d34ebc923e2a55fc0c6ff - BSC, from Polygon, to Defiway
- 0xfd8a4501a374b07bb152440ae003648daa606fba - BSC, from Polygon, to Defiway
- 0xf9685608612bd65d147c939d0ce9a3e0e2a8b1df - BSC, to Defiway

- 0xfa987b52c1a0570044d2d7f06706f68bb2c3b36f - Laundry
- 0x3e9ae95d395d3b7dd48f49f0093c75dffec09d2a - ETH, to 0x66d
- 0xdb505e529b6bb36e85400fbc4b95077aadf3f97a - ETH, to 0x66d
- 0x66da37ebb6f587d51aa485d7a5ff8db34f358b04 - ETH, to Stargate
- 0xbee9a13af5f0ab416f0cd0878f954d7bb12281a0 - BSC, from Stargate
- 0xf02fde1530845d36f352bf8512595c2227280476 - BSC, from Stargate
- 0x1fd75e7e02cf776801559ee46dda214d93906eab - BSC, to Defiway
- 0x6c13e27240ea3d2e12b37bfef76337a9ff44eaf3 - BSC, Dormant
- 0xda581fdf12df38c5281ef73fcb7cf3b4d55e2f1b - ETH -> BSC Apr 19
- 0x18e9ef38778bddaa9795c1969628de6892e3fc8b - BSC, to Defiway
- 0x21879646f8246305a8effe3544f986baa1be80c2 - BSC, Simpleswap?

- 0x7d9a5a198c3fc7caa947f3d8376d2d5d26de14ac - Dust from 0x1a2 + $70k from Polygon 0xa6b
- 0x6c13e27240ea3d2e12b37bfef76337a9ff44eaf3 - Dust from 0xda5
- 0x21879646f8246305a8effe3544f986baa1be80c2 - Dust from 0x6c1
- 0xfd8a4501a374b07bb152440ae003648daa606fba - Dust from 0x3012
- 0x3f87f358f67916545721b930d181f8b853805c3f - Dust from 0xf318
- 0xbe1566497c7f581258c14bf297a8f4e747ddf013 - Dust from 0x3e2

- 0xf2e43d4c4cac88cd86c3700482094c9bc73cecee7ef05a6a158128cc751d312f - April 2nd Theft Txn
- 0xee2e4fbe10a437e1b1561687d4e5133dd397ab96 - Primary Theft ($275k MEOW), ETH -> BSC 
- 0x59523347198bef5e24d57c129d393bb0390338c0 - Laundry 
- 0xe59e3ca05510cad092c3514e4fb45976f2d48f59 - Laundry
- 0x5ffe27c4038e033959812527e76bc7bc436afd9f - To Defiway
- 0xabe402e27750bf13641a96fbb2677bf7a2a58a88 - Laundry - BSC, to Polygon
- 0xa9527ecd5a3fd16f123d98029187597bcffef5b4 - Polygon from SBC
- 0xeb283be1150a7ece0545b5ac300fbb2ee9447c91 - Polygon, to Defiway

- 0x1bb3ccca65ebfca4557c58081391b1c907fdd91c - Dust from 0xabe
- 0xd0f7ecf1580b607c3df7e7d9e9b3a611bbf2ab3f - Dust from 0x1bb
- 0x0cf9f7bd61d3df5de2728f69a88da91170ad6b13 - Dust from 0xd0f




## URLs

- https://certik.com/resources/blog/private-key-compromises



## Connections

- 0xee2e4fbe10a437e1b1561687d4e5133dd397ab96 is involved with CloudAI and Murall Hacks


