# Loopring    

Date:: 2024-06-09

Time:: 17:41

Tags:: ❓TraderTraitor   

G:: 399685

---

## Notes

Attributed in [MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities](./pdfs/2025-10-22_MSMT-Report.pdf)

I've got nothing to say it is or isn't DPRK. It sat dormant from June 2024 all the way to March 2025.

Then goes to eXch, BitcoinVN, and Swapuz.

It was then laundered in batches. Directly from the theft address. No handoff is very unusual for DPRK. I would also be **insanely** surprised if this was TraderTraitor specifically.


## Details

Ethereum Layer 2 protocol Loopring posted on Twitter that the some Loopring Smart Wallets were targeted in a security breach. 

The attack exploited wallets with only one Guardian, specifically the Loopring Official Guardian.

The hacker initiated a Recovery process, falsely posing as the wallet owner to reset ownership and withdraw assets. 

The attack succeeded by compromising Loopring's 2FA service, allowing the hacker to impersonate the wallet owner and gain approval for the Recovery from the Official Guardian. 

Subsequently, the attacker transferred assets out of the affected wallets.

Although Loopring markets its wallet application as "Ethereum's most secure wallet", that's evidently a pretty low bar. 

They disclosed that they had suffered a breach in their wallet recovery service, which allows individuals to designate trusted entities to recover assets or freeze compromised accounts. 

An attacker was able to "recover" assets from wallets that had only designated a single Loopring guardian, pilfering at least $5 million.

Loopring announced that they had suspended their account recovery operations, and were working with law enforcement to trace the attackers.



### Commentary

> We continue seeing the trend noted last week where the majority of losses are no longer caused by smart contract exploits. 
> Loopring is one such example where a flaw in their 2FA recovery service was used to drain multiple wallets with losses exceeding $5M. The incident affected wallets that configured a single recovery wallet, namely Loopring’s official guardian account. A few lessons:
> Wallet providers must provide secure configuration by default. We can’t assume users to do the right thing or fully understand risk.
> Single points of failure like an official Guardian account create outsized risk and attract bad actors.
> Web2 security controls like 2FA can and will fail.
> See Vitalik’s recent post on Reddit [How I think about choosing guardians for multisig and social recovery wallets](https://old.reddit.com/r/ethereum/comments/11tijiv/how_i_think_about_choosing_guardians_for_multisig/) for more tips on secure implementation.

[Source: BlockThreat](https://newsletter.blockthreat.io/p/blockthreat-week-23-2024)


### Team Statement

> A few hours ago, some Loopring Smart Wallets were targeted in a security breach. The attack exploited wallets with only one Guardian, specifically the Loopring Official Guardian. The hacker initiated a Recovery process, falsely posing as the wallet owner to reset ownership and withdraw assets.
> The attack succeeded by compromising Loopring's 2FA service, allowing the hacker to impersonate the wallet owner and gain approval for the Recovery from the Official Guardian. Subsequently, the attacker transferred assets out of the affected wallets.
> We are actively collaborating with Mist security experts to determine how our 2FA service was compromised. To protect our users, we have temporarily suspended Guardian-related and 2FA-related operations. Following this action, the compromise has ceased.
> Loopring is working with law enforcement and professional security teams to track down the perpetrator. We will continue to provide updates as soon as the investigation progresses.
> The hacker addresses involved are:
> 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102
> 0xbacef3a142e39f14f4f15e22e9248ee4141af18f
> If you have any information that could help us track down the hacker, please share it with us.
> Stay tuned for more information. Security and user protection remain our top priorities.

[Source: Loopring](https://twitter.com/loopringorg/status/1799791898296451515)



## Further Reading

- https://theblock.co/post/299177/loopring-suffers-5-million-hack-after-guardian-two-factor-authentication-service-is-compromised

- https://quadrigainitiative.com/casestudy/loopringofficialguardian2favulnerability.php

- https://twitter.com/loopringorg/status/1799791898296451515

- https://twitter.com/loopringorg/status/1801268180364530172

- https://twitter.com/loopringorg/status/1800846819666108482

- https://twitter.com/loopringorg/status/1800141336470810660

- https://old.reddit.com/r/ethereum/comments/11tijiv/how_i_think_about_choosing_guardians_for_multisig/



## Onchain

- https://etherscan.io/tx/0xf0a02e3dc32e380f5fbc832981963277f7b2ce9345040ddf1f3016724b84e251

- 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 - Primary Attacker
- 0xbacef3a142e39f14f4f15e22e9248ee4141af18f - Primary Attacker (Gas/Caller)

- 0xada16604c3ea42c2988b31d4cfeeace3d4dcd1c1 - Intermediary (2025-03-06)
- 0x86be93e5183c7924995098b2b0ddb60dd9429d14 - Intermediary (2025-03-06)
- 0xf781ccc4082692e80659f68bde96a1ca3300ea1a - Intermediary (2025-03-07)
- 0xc8f1ff9d2701a8b2c4f946faf0d8c8fe464057e8 - Intermediary (2025-03-09)
- 0x0c75df358bebca7a204fed45db9ac235b60a0559 - Intermediary (2025-03-10)
- 0x33c2d25792bdc2bcb2609ce96e819ae5d6378789 - Intermediary (2025-03-10)
- 0xb11d934e0c49c5c400a766664464ca6b6aaa9ec6 - Intermediary (2025-03-11)
- 0x69ddfafffd9426ebfad160d654645aa46ea4649f - Intermediary (2025-03-11)
- 0xe642d3415d222aaf19e20484476ef443c5ac176b - Intermediary (2025-03-11)
- 0x7932b04d7b2cf16e183fd44b521ab1336756df2f - Intermediary (2025-03-11)
- 0x48c2fabbed679b5ca1caba0817d528404fdc2162 - Intermediary (2025-03-13)
- 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 - Intermediary (2025-03-14)
- 0xa5892c54759f9e296e67b2a6afbdf908676cd875 - Intermediary (2025-03-18)
- 0xe5e95f541624af7dd42c5efaea4c56e3a0acf73a - Intermediary (2025-03-19)
- 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba - Intermediary (2025-04-21)
- 0x786c44914ea8d29f96e649741bc14a60660704ce - Intermediary (2025-04-22)
- 0xdafbf7e88e8ef502aadad88e660157f192ac4de7 - Intermediary (2025-05-08)
- 0x576c78b6eb5a9ae94d1c0b2e8ecf840a90a16310 - eXch Depo (2025-03-06)
- 0x7070777ddce376a625d16cbe5b84428cc481c126 - eXch Depo (2025-03-06)
- 0xb93b989658ef9e5fc28a4b1fd9ca78791ac8ec4c - eXch Depo (2025-03-06)
- 0xe3abb195f93a93372fec3b42ef86c2d3e63f3e52 - eXch Depo (2025-03-09)
- 0xc5a96f0007445e17796438286b151a66629a743d - eXch Depo (2025-03-09)
- 0x3f3e8a263d0e79d3f1f2bf720254de4f5a748530 - eXch Depo (2025-03-09)
- 0x15c65b58f9a6f2cd1ba637551b1cb17437d81020 - eXch Depo (2025-03-09)
- 0x13879e25d699478f89fa005422d54946d9915df5 - eXch Depo (2025-03-10)
- 0x47bc1fbe484006474279750f2b3d9592fcb46c55 - eXch Depo (2025-03-10)
- 0x1fe35c433ddb342f9e01933da6e0c90c3be56fd6 - eXch Depo (2025-03-11)
- 0x7d03c57fa61d82e84ef5e6f6a8e9b69257f96335 - eXch Depo (2025-03-11)
- 0x78f6104dfbd96be478e7640ae4dea132e8d51874 - eXch Depo (2025-03-11)
- 0x4d44df6dd513b50630ce51dc34974cc3a710b57c - eXch Depo (2025-03-11)
- 0xc81097dcf71c02de27f0517da6e6b1fc7a4d41cc - eXch Depo (2025-03-13)
- 0x8d38685c9940a6bc3396adf310daf8bc27944df9 - eXch Depo (2025-03-13)
- 0x002536416d7a20848067fde6bb4cd28bc742271c - eXch Depo (2025-03-13)
- 0xb7b6a1336d3d308101faa1223da644d0fbb63062 - eXch Depo (2025-03-14)
- 0x416db290926960e9835d3cb8c0404c333c56a00b - eXch Depo (2025-03-14)
- 0xa5c05b6ae64e457aa2168d73942a5460f4924a0e - eXch Depo (2025-03-14)
- 0xb89d9ade1d6551e60595bf68afdc4476a21836a3 - eXch Depo (2025-03-19)
- 0x186cbf884dac7af20ae0155c3b42ac2faf9f141c - eXch Depo (2025-03-20)
- 0x3ccd3b1d441a793aaccc878bfa9ace607acbfc53 - eXch Depo (2025-03-20)
- 0x9c34fc8f1596003e414e9efe4f11d5eeef152b4a - eXch Depo (2025-03-20)
- 0x66d84ccffedd168c6047a4ecce8affdf39d20e28 - eXch Depo (2025-04-21)
- 0x0b56e51a80a5196377da96d2d106af37d434930f - eXch Depo (2025-04-21)
- 0xdff121fb757e0223f17129fa987978dd374b8f2f - eXch Depo (2025-04-22)
- 0x8e143ae951b5cd1bc5b99cdc3667723b6c7f8ce9 - eXch Depo (2025-04-22)
- 0x7b58824b01a33528a0149fd52b9d06f5361756bd - eXch Depo (2025-04-22)
- 0xca1379a7dccb147164b209d15b37290912332d7c - BitcoinVN Depo (2025-05-27)
- 0x94cad8b95d11f03a5f53cf157a0ad0211e8dd2a1 - BitcoinVN Depo (2025-05-27)
- 0xe6b8eca2fdc67a253388c9d4e21b0fb3c1e66a83 - BitcoinVN Depo (2025-05-27)
- 0xdd79196331202cd923f3e7bd4280018ca2d67543 - BitcoinVN Depo (2025-05-27)
- 0x4c725719a5bcc1d7aa1194bac3beb36ee0ac839b - BitcoinVN Depo (2025-05-27)
- 0xe3333e86e82669eeb00dc7638181058220b1b85e - BitcoinVN Depo (2025-05-27)
- 0x3cfaf7b910828b9344aa8a9f97f59220318617d4 - BitcoinVN Depo (2025-05-27)
- 0x7e4c190db365550f11debe63903ebc4558f17451 - BitcoinVN Depo (2025-05-27)
- 0x8a1c20e4e79d979ac1f7514fef2b0e36e554f96b - BitcoinVN Depo (2025-05-27)
- 0xd83f0f62547ba4e6df2bb166c5e18570d17af55b - Swapuz Depo (2025-05-28)
- 0x72703217f0b33fa2fcdf3aedd5118bcce52cb328 - Swapuz Depo (2025-05-28)
- 0xfaa9121849f299385acd5017fd5d086de219368c - Swapuz Depo (2025-05-28)
- 0x069304073cdace751a863fc4658bfd1a7d95c4f9 - Swapuz Depo (2025-05-28)
- 0xa53106af6b95751f205cedaa8617249e0e379d7a - Swapuz Depo (2025-05-28)
- 0x9bed6e3dab814c13df27b1fbb8bf0b4f7ada8ed6 - BitcoinVN Depo (2025-05-28)
- 0xfcbf282facb57df4c12fcc45700ab3ea01fb8f3c - BitcoinVN Depo (2025-05-28)
- 0xd79c92078e765b2809805844c54c6ba0ef57f6f7 - BitcoinVN Depo (2025-05-28)
- 0x2bc9cbb613876409012ab5c801a980d66d9f3ef5 - Swapuz Depo (2025-05-29)
- 0x3995f826abc0ffaf03cab6931fb9b3d982a55686 - Swapuz Depo (2025-05-29)
- 0xc73d1ea63439f6e664befd0a515f940fc0ff4bef - Swapuz Depo (2025-05-29)
- 0xc5e652584600c7a0d92209fd9e79283d7e7f2122 - Swapuz Depo (2025-05-29)
- 0xa3dc37b85cebebf3bfabe3a5bf84d3381633739d - Swapuz Depo (2025-05-29)
- 0x36ed6385a7f7083cf2b9a05806abec3978683fed - BitcoinVN Depo (2025-05-29)
- 0x46d40089485e582972c98320029a683e41669a39 - BitcoinVN Depo (2025-05-29)
- 0x37b5bd8e79508b141e7c1f555fe8230e2a9267a8 - Swapuz Depo (2025-05-30)
- 0xc3c94ed121b70d80b04565a93faaf65c5521734b - Swapuz Depo (2025-05-31)
- 0xe6059e72e85e310757363127ea8d53493c619ecf - Swapuz Depo (2025-06-07)
- 0x0f45123c682250e4f6c53841f0c493dda2e41a6e - Swapuz Depo (2025-06-07)
- 0xb6baebbf3546d72619677508d668a8a5e781531c - Swapuz Depo (2025-06-07)
- 0xd64b36a33274167402598fa6af35e750120bc3a2 - Dormant (2025-06-07)



### Tornado Cash

- 2025-05-26 01:59 - 0.1 ETH Depo
- 2025-05-26 07:11 - 10 ETH Depo
- 2025-05-26 07:19 - 10 ETH Depo
- 2025-05-27 02:30 - 10 ETH Depo
- 2025-05-27 02:37 - 10 ETH Depo
- 2025-05-27 02:51 - 10 ETH Depo





### Full Txn List


| Timestamp        | From Label       | From                                       | To Label         | To                                         | Amount         | Asset        | Value (USD) | Txn Hash                                                                                         |
| ---------------- | ---------------- | ------------------------------------------ | ---------------- | ------------------------------------------ | -------------- | ------------ | ----------- | ------------------------------------------------------------------------------------------------ |
| 2024-06-08 17:34 | Victim?          | 0x8e534af51fb580c546f30d4175014af4bee921d8 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | 0.5199995244   | ETH          | $1,917      | [🔗](https://etherscan.io/tx/0x1d76e080bac5c89b12f315d3cad88307b7b2a5ff03fb3e0a152ede08b081ddc5) |
| 2024-06-08 17:34 | Victim?          | 0x59f3163ab39b8b90daf57508bc1faecb2f2cd374 | Victim?          | 0x8e534af51fb580c546f30d4175014af4bee921d8 | 0              | ETH          | $0          | [🔗](https://etherscan.io/tx/0x1d76e080bac5c89b12f315d3cad88307b7b2a5ff03fb3e0a152ede08b081ddc5) |
| 2024-06-08 17:39 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x63e7bcadc5661b6abe62bff4f52cc20c70006371 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xb7a923bf7130db0117d3b94f154accfcc241d84e679bc1fc2b1b5d1d22c085ab) |
| 2024-06-08 17:41 | Victim Wallet    | 0xad29f3bd54a606d6570fe92295b48a7d392dd4e2 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 189914.4155    | LRC          | $46,324     | [🔗](https://etherscan.io/tx/0xf0a02e3dc32e380f5fbc832981963277f7b2ce9345040ddf1f3016724b84e251) |
| 2024-06-08 17:47 | Victim Wallet    | 0x5b000d1ccb6127d8a244d35d28287419f7c1db82 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 28.20580018    | ETH          | $103,973    | [🔗](https://etherscan.io/tx/0x9b16d8bc7bf9209bea3391a684c2b78a1bfdf7d683eb3e5cd0ce51b3e26278c9) |
| 2024-06-08 17:50 | Victim Wallet    | 0x51ef507e59d66918ae09bfb606060a60399f090d | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.2431568     | ETH          | $37,759     | [🔗](https://etherscan.io/tx/0x319f029928de764215ca6ddfaa49e904a77efa9a21da7c3e378d2325a6af7a42) |
| 2024-06-08 17:51 | Victim Wallet    | 0x2dec0bdf73d6521b98c4e8739edbb2e58e891e00 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 69.12429512    | ETH          | $254,808    | [🔗](https://etherscan.io/tx/0xe569ee801abc04fafca23b6a87d9a37aae4ffad82e12dd445addd0066918b8a4) |
| 2024-06-08 17:51 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x5b000d1ccb6127d8a244d35d28287419f7c1db82 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xbae598df6e630e7081a247b33b6b8cc0a7b8eb6a2b987313b4f74005cc44542e) |
| 2024-06-08 17:51 | Victim Wallet    | 0x52ba88e942a81b6aaaf6ceed3adc6ad9a1b71d38 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 17.45064119    | ETH          | $64,327     | [🔗](https://etherscan.io/tx/0x17ffe2d678aec5eca5c743aabed93f4ed6bd72f32e14954fd7a445781b79eaf2) |
| 2024-06-08 17:52 | Victim Wallet    | 0xc9f29e8a21586f5134fae3d61797731be8c303f8 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 15.05523188    | ETH          | $55,497     | [🔗](https://etherscan.io/tx/0xd8d924a59127d10a100387183ea0fc9e3a3dbb38b9a464d7a55ce689a403206b) |
| 2024-06-08 17:52 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x51ef507e59d66918ae09bfb606060a60399f090d | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xe853605186755347135b0a1849f0a291416a7819f01059c024cc90ad4349c87e) |
| 2024-06-08 17:54 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xe2efc4082108da43eb8082d5c64b8744a69b292d | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xc60096f9534fabb93681d5f17f360b2466496c278940b5ed9874690b5c75ad35) |
| 2024-06-08 17:55 | Victim Wallet    | 0x0ca8dfc9229f25789217dcc4771b1d79b3f961e6 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.08536303    | ETH          | $37,177     | [🔗](https://etherscan.io/tx/0xdf55b70267e71cbee6fff544cb3a0011e564928471a456d0238f4917137deda8) |
| 2024-06-08 17:56 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x08e80e6c538bbb5976159317eba84b325efb16a5 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0x1cb79b310a2ef2fd13af86756a885486f37a976cbd076629c084d0581ed02a5d) |
| 2024-06-08 17:57 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xa84f9f7939e8adf5c5d3cf18664df2908d255042 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xb13eeb26e839a224848ebf8369acd8bf18f9bb5c35f50fa724e69b82a9a6f93e) |
| 2024-06-08 17:58 | Victim Wallet    | 0xf9e84f452a818b383d1b9e7eb74871cbd0ef245d | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 29.90291343    | ETH          | $110,229    | [🔗](https://etherscan.io/tx/0x0fc3d68feab1cf5b4a38cf05aa537e9fe61d0f50b0e20ae107a140ae67e94607) |
| 2024-06-08 17:58 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xbf8fa544f40caedad29949665a58fde8c0ff090d | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xd6da30807344db048d12e812f102d8376d3a0f4a3d045a3a2b82c11d0dc88275) |
| 2024-06-08 18:00 | Victim Wallet    | 0x399d40d5be83a28bb66ec205f6ff738e8a8e9397 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 21.05383625    | ETH          | $77,609     | [🔗](https://etherscan.io/tx/0x41f7effd30d878824d0b8dcb9161e3101280b628178a68e6b1f26b7935c872ea) |
| 2024-06-08 18:01 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb92398584108af3dd8ae9cbf4e2bb7ecded30f75 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x1d2f7830c123a27f1df2c4fa946aa0d91b6070b566927ca13b5c1deda0c848e5) |
| 2024-06-08 18:01 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x2dec0bdf73d6521b98c4e8739edbb2e58e891e00 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xc502cc52152d9befc503b0c69913d7ebccd7159c0eda3934eecc4686058f4ddc) |
| 2024-06-08 18:02 | Victim Wallet    | 0x5b000d1ccb6127d8a244d35d28287419f7c1db82 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 0.003617188845 | ETH          | $13         | [🔗](https://etherscan.io/tx/0x09a50b02f63152b15a81f519c90170aac45ff22a87a592e31cfe2261b0b7ea27) |
| 2024-06-08 18:02 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x52ba88e942a81b6aaaf6ceed3adc6ad9a1b71d38 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xe3f0a81f77b349afbc54649493ee5a55f5eeef0e808a573211a6c9d8b8531a63) |
| 2024-06-08 18:06 | Victim Wallet    | 0xc744087c95007d5061d26ec8c77774ba5e44fe06 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 21.48206933    | ETH          | $79,188     | [🔗](https://etherscan.io/tx/0x1328f3afb376bef9a38642fcb8c1292b2436e6e978d7bf77102e06ba457cfc21) |
| 2024-06-08 18:07 | Victim Wallet    | 0xa0ecfafef37a769067e741c132c591744267e25d | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.43018948    | ETH          | $38,448     | [🔗](https://etherscan.io/tx/0x9d7ecdbd7ebc7732d140ca31373076a5b71a0508c18f9bbcf55140a78fae59e1) |
| 2024-06-08 18:08 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xfa0dd8fc7381939a64be6f150335b072c3e3c98e | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xf5e811fa1694978064e13de75220f92aa6d571c06c34beec8a67ce60c587bc94) |
| 2024-06-08 18:08 | Victim Wallet    | 0x8f3be4c92ea38b1db5501db3838966739494de89 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 12.3137012     | ETH          | $45,391     | [🔗](https://etherscan.io/tx/0xfc1cffc9767545e6d99156592af8dc768e4b85afffb6713334b5ea4d61cdc0a4) |
| 2024-06-08 18:08 | Victim Wallet    | 0x553200b15ab249dd18c5b4f1f1e5a00886562898 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 9.995602643    | ETH          | $36,846     | [🔗](https://etherscan.io/tx/0x2750df2b9eef079f1fd671851261b2b1c56822b8af4bc17185bd16ebe6860354) |
| 2024-06-08 18:09 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x06afc66ff10de97ee56b35867ee5d13e7a7b1b2d | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0xb766fb1a4c51f03aff9d3ea137f25da9bc74d1e932b3e5a2ef494feac3276bdb) |
| 2024-06-08 18:10 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x7d7e9641a67755f7126d1cfc7f99b5bf7a0b8f45 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xe2704a593b03d3d931b8fb53125d1a728836b48f184c82e4ac4df833ce50e72e) |
| 2024-06-08 18:11 | Victim Wallet    | 0xf9468fbd6feb138b118926cd0313d1e4a16e4f50 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 123847.3595    | LRC          | $30,209     | [🔗](https://etherscan.io/tx/0xa519e93efd11a181dde37d9591c0cde184ad099c0b53790448a5ef31a1e806e3) |
| 2024-06-08 18:13 | Victim Wallet    | 0x06afc66ff10de97ee56b35867ee5d13e7a7b1b2d | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 150274.8826    | LRC          | $36,655     | [🔗](https://etherscan.io/tx/0xa13737f20ac48f10d2ce8bc05bee68d4160731d3782a5138c15d5d2a59e2f90a) |
| 2024-06-08 18:14 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xc41d55bec55bd844809e13e19d9acb3a13e941e0 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x62983ff3b0bb08a1f2de7b438067b9bead0224cb81c453b369a6d280c4c19bbf) |
| 2024-06-08 18:15 | Victim Wallet    | 0x9e8449aa1f6a5b547f26f165023c212df07e2064 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 58777684708    | PEPE         | $695,841    | [🔗](https://etherscan.io/tx/0xd88313ab4f9893e1ccae8fa421549c64e0249cd75c6b4a1f7428cd787ae7f9ef) |
| 2024-06-08 18:15 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xd2d4c571d047db54644dc5de65af1b48cfb0e04f | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x3b4719b69bebafbbe88ae4c80d7caa6f9dca886eedd39e6941394ad1afd462b4) |
| 2024-06-08 18:20 | Victim Wallet    | 0x5b000d1ccb6127d8a244d35d28287419f7c1db82 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 61062.58798    | LRC          | $14,894     | [🔗](https://etherscan.io/tx/0x6e01095bdc7d6ce2cf5fad33aca93899005728155bc10652e57d6c375fe8a03a) |
| 2024-06-08 18:20 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x1496ab088ae2302e94b6b9670a9b9091de856f5c | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xa60fca341e0d6d087284e8618943c62d12089b20eb3145b755b19304a636da4d) |
| 2024-06-08 18:27 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x70eeda38dc4685c511e05de9819607d191be7a02 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x483e2229e257fe943d3638fa6a3c01f66a7922d46f1a5bc87a2b5294b2b4f3c4) |
| 2024-06-08 18:28 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xfc0b880ed947985740c1db850f37d3139bc27af8 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xc54e88de987fea94dbdd61caf4b2572a446dcc314cf0c4a7e6e7a702db6752b3) |
| 2024-06-08 18:31 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xe7449c9111936cd1dbc15c63139fb85aa886c4cc | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x9bbf09f9a55a88089c682bbfaef9ab1ec5a4bf8230e580e105631d195bc3d65f) |
| 2024-06-08 18:37 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 13.85237722    | ETH          | $51,063     | [🔗](https://etherscan.io/tx/0xd510bea1de952ccca03cf0b6abdc3b1a131e17da83cf5aaa67757b1e1dc679ad) |
| 2024-06-08 18:37 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 27.66192771    | ETH          | $101,968    | [🔗](https://etherscan.io/tx/0xd510bea1de952ccca03cf0b6abdc3b1a131e17da83cf5aaa67757b1e1dc679ad) |
| 2024-06-08 18:37 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 51.63786127    | ETH          | $190,349    | [🔗](https://etherscan.io/tx/0xd510bea1de952ccca03cf0b6abdc3b1a131e17da83cf5aaa67757b1e1dc679ad) |
| 2024-06-08 18:50 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb98e69b59686be51046a4fa97b86a2fc92d7288e | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xef11cb72b89d76349077b1dd56d43615d666d6591b403c8ae8df472ff6168da3) |
| 2024-06-08 18:52 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb75532e1061245baebcaa2e60fc0c71d7fffc66d | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xd7cb37c0b3960720c42b8ab46df993329b5c47f2b81901396d1f41ef54dae8f9) |
| 2024-06-08 18:53 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x71a9fcf0f3fd483f1c13e6d5836b9736f66a93f7 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x6160b560d2ad3426457f35cdf9c03d8e8de858a90ac4b395462dc93b5057d901) |
| 2024-06-08 18:56 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb92398584108af3dd8ae9cbf4e2bb7ecded30f75 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xdb6196900502345496d16d816345c35a98fc0cd950de6dd7a33876e2ab892261) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 0.5132247      | WBTC         | $35,609     | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 9.996544       | ETH          | $36,850     | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 15.8927426     | ETH          | $58,584     | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 59674.21875    | USDC         | $60,078     | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 21.86711576    | ETH          | $80,607     | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 40             | ETH          | $147,449    | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 44.35977168    | ETH          | $163,521    | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 18:57 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 60.62848837    | ETH          | $223,491    | [🔗](https://etherscan.io/tx/0x3a73899ed54d1946e32bcdd457d2790da009a67b6a689c3429752301579faaf4) |
| 2024-06-08 19:05 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x7d7e9641a67755f7126d1cfc7f99b5bf7a0b8f45 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x0ed041f5aa3ca138b326750df3c1f90ee67a19cbdf2761397eab243865d60136) |
| 2024-06-08 19:29 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.08140432    | ETH          | $37,162     | [🔗](https://etherscan.io/tx/0x6c7a19742626aff189e84b2fdc7ef7bda36193244a95a59b568352c5eadf967f) |
| 2024-06-08 19:29 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 14.86912519    | ETH          | $54,811     | [🔗](https://etherscan.io/tx/0x6c7a19742626aff189e84b2fdc7ef7bda36193244a95a59b568352c5eadf967f) |
| 2024-06-08 19:29 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 50             | ETH          | $184,312    | [🔗](https://etherscan.io/tx/0x6c7a19742626aff189e84b2fdc7ef7bda36193244a95a59b568352c5eadf967f) |
| 2024-06-08 19:29 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x98ed261bdb2da93408b4471d9e6fab6e11437295 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x7642be15e1786634c41f52a0b326587c1703763150d4173264087ef062a4a171) |
| 2024-06-08 19:30 | Victim Wallet    | 0xc41d55bec55bd844809e13e19d9acb3a13e941e0 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 114.209947     | UNI          | $1,136      | [🔗](https://etherscan.io/tx/0xcd71f8a56a999c9843cb4c0b478402c38ecdc361ce7aa857513055b7f03c5530) |
| 2024-06-08 19:30 | Victim Wallet    | 0xc41d55bec55bd844809e13e19d9acb3a13e941e0 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1047.807619    | IMMUTABLE_X  | $2,193      | [🔗](https://etherscan.io/tx/0xb13fece46fadbb92eb5080dd3e7a44246084e40d5f59afacc7d9167b80b45b15) |
| 2024-06-08 19:30 | Victim Wallet    | 0xebc00db31ef22da678822cbae9d54e1cc5af181b | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 15361          | LRC          | $3,747      | [🔗](https://etherscan.io/tx/0xa1aaad78c837c2ee0f152cf93eba7e4f6c3e0cca5a96778db3eef8c78e391fff) |
| 2024-06-08 19:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.66313597    | LIDO_WST_ETH | $45,884     | [🔗](https://etherscan.io/tx/0x30d987922c5cf9e31016b174d24ef6d0547fd8964d3b56ea0f07ca6450d9d085) |
| 2024-06-08 19:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 13.01350954    | ETH          | $47,971     | [🔗](https://etherscan.io/tx/0x30d987922c5cf9e31016b174d24ef6d0547fd8964d3b56ea0f07ca6450d9d085) |
| 2024-06-08 19:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 14.52892792    | ETH          | $53,557     | [🔗](https://etherscan.io/tx/0x30d987922c5cf9e31016b174d24ef6d0547fd8964d3b56ea0f07ca6450d9d085) |
| 2024-06-08 19:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 15             | ETH          | $55,294     | [🔗](https://etherscan.io/tx/0x30d987922c5cf9e31016b174d24ef6d0547fd8964d3b56ea0f07ca6450d9d085) |
| 2024-06-08 19:53 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x9372ad44ef76c6c42ea08bda06961f115c5bb4f4 | 0.005          | ETH          | $18         | [🔗](https://etherscan.io/tx/0x5ae9383977a020567d599f381692f2d9deac9e583aa76f454399dc77de70df7f) |
| 2024-06-08 20:32 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xc0ad40b17c8cd67c3e8d3da0c0d4de74d1a1cd3f | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xb3f68a415d6695417d068ca05728cb1f28d6c907f0d2f522c455e3590e44c54d) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1271.80597     | USDC         | $1,280      | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1.786705767    | ETH          | $6,586      | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 4.522845645    | ETH          | $16,672     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 24050.53768    | USDC         | $24,213     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 12.77679309    | ETH          | $47,098     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 14             | ETH          | $51,607     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 19.9           | ETH          | $73,356     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 21.6           | ETH          | $79,623     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 20.15748405    | LIDO_WST_ETH | $86,738     | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 50.06762035    | ETH          | $184,561    | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 20:54 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 56.98686295    | ETH          | $210,067    | [🔗](https://etherscan.io/tx/0x051065b414e0e9801e850b49860cd2b257d27a28a70025b334b95aacb42dd716) |
| 2024-06-08 21:02 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x3bdebfc8d4ca345f8ee93b44c09d3b7ce7210d9d | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x5926ff390363eaa105781f04f04d0c53ac7e58348a024bd2b228a4d33915ecea) |
| 2024-06-08 21:03 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x2a7cea412a00d5694485843bd53c255ed64b1371 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x8d0c26f62df63272d8cd02fa66abfa8b5e4f5dba54f26404f3c420db7794e0fb) |
| 2024-06-08 21:10 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 0.73170139     | ETH          | $2,697      | [🔗](https://etherscan.io/tx/0xb81dcfd0b51a44340b802d7d6c7aa31e47bcab245af3c4e26553771e92ebb56c) |
| 2024-06-08 21:10 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 2.729814635    | LIDO_WST_ETH | $11,746     | [🔗](https://etherscan.io/tx/0xb81dcfd0b51a44340b802d7d6c7aa31e47bcab245af3c4e26553771e92ebb56c) |
| 2024-06-08 21:10 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 5.612556216    | ETH          | $20,689     | [🔗](https://etherscan.io/tx/0xb81dcfd0b51a44340b802d7d6c7aa31e47bcab245af3c4e26553771e92ebb56c) |
| 2024-06-08 21:13 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x8d40c0fabec34fd79dc3bc5b08352025785439d3 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x32e578cbc7b8be7037f2e15bca43c2d9764b5d63b912f0fdd2a7d5943e585f71) |
| 2024-06-08 21:13 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xec68978fc9da315af3826775d70d3ebaed76c429 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xe6f37400f78ecaf07591544089f3dbe353702ce49bf42d1e7ed8f93cc9d7f194) |
| 2024-06-08 21:17 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x4b58c10cf4068f38a101e51d7ee3b5469c854d5c | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xd501432b3c7cb7440838921797d8d1bdb351aa1397a4acd485ee98d9e624ffd2) |
| 2024-06-08 21:22 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x45326101d40226dc41202cc935062707bb9e7ea2 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x3faf55d4a61c8d533b67d4873719981f108cbd05c01a8486c4841f9f7ec4b3d4) |
| 2024-06-08 21:23 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x57437f04ca7896aab747b988f97d3f01134fa02b | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xceac91f12b32eb09ddc6db7ccab77d041390d85ee5fc74392d4e3887b99ed47b) |
| 2024-06-08 21:28 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x57437f04ca7896aab747b988f97d3f01134fa02b | 0.02           | ETH          | $74         | [🔗](https://etherscan.io/tx/0xcebea78e2b8d6a4f3a947aa00799981fadb6f2e5bcaf397adba677ef1e237292) |
| 2024-06-08 21:31 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 2.453613887    | ETH          | $9,045      | [🔗](https://etherscan.io/tx/0xf9fb194fa8635c7dbaa4225b4c80a302f146edbaf38ce3020c73f4bbe8d53951) |
| 2024-06-08 21:31 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 6.3472595      | ETH          | $23,397     | [🔗](https://etherscan.io/tx/0xf9fb194fa8635c7dbaa4225b4c80a302f146edbaf38ce3020c73f4bbe8d53951) |
| 2024-06-08 21:31 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 6.757422162    | ETH          | $24,909     | [🔗](https://etherscan.io/tx/0xf9fb194fa8635c7dbaa4225b4c80a302f146edbaf38ce3020c73f4bbe8d53951) |
| 2024-06-08 21:34 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xdf5f49455797d146d46c9d9caba116a855c267d4 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x99b8443a00aa040e2bfad5821c22beb81ff7ccf60c26fe6a4cc8d0fd6d228af3) |
| 2024-06-08 21:37 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xfb38ecbe9202375d9152bffe009efaf49b563f96 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x47f799435df8f0c99d05960fb40d8fdc39371f8e39b63d921fd2e97fd8ec5f0e) |
| 2024-06-08 21:39 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x6c108bb2a6f0a607bc35d86d989994cd716b5998 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x7a2261b615e70f6f445a495f881f15b30ae696dc95a5c21f32fdd8fa89da7185) |
| 2024-06-08 21:40 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb81dc3e1d623ce42a7168be0520206e8e4053f52 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x9f84f686106b1afef968e0a5bb6adad7fa188bf87b84735665bc499ffe620d74) |
| 2024-06-08 21:41 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xc737b3d19565431295d1c9b079ca35b862481e50 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x9f23b627801597a4b34178c1d1f3985da791d4db5a84541e152ba395d7cdf416) |
| 2024-06-08 21:42 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x7e99d19b0ac4093d8f5e9a419f311ff4dbf98f46 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xada821fddf341937e1fc4a7c4a2b69b5f308337e41cdc5da84f7e88c69d3bf07) |
| 2024-06-08 21:44 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x83c223979048675dc582299ab1893830328366c1 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x98c8acca1a67c70ff370ec689d191664f114208b639881839c4f707db45369e1) |
| 2024-06-08 21:51 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x5bd60ffc6328801b2091fd504663f0e3c88e0934 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x34b210dbb6770f257a17d698a1444ce51cdac9042f09f813816ef1c4faa9adce) |
| 2024-06-08 21:52 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xb9ec3f9e12fa0d39cf09e35bb8badfcfb0725a94 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xa2645d37ec6e3562a4e8b4f21886137ce9501fe162a4ef8be2bf50618f7de95e) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1.519796749    | LIDO_WST_ETH | $6,540      | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 2.09           | ETH          | $7,704      | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 5.383644922    | ETH          | $19,845     | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 6.7387         | LIDO_WST_ETH | $28,997     | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.77          | LIDO_WST_ETH | $46,343     | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 4.58107434     | CIETH        |             | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 21:53 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 5.22499977     | CIETH        |             | [🔗](https://etherscan.io/tx/0x2662a4e2f39e1fe53c85ce689770dfd91d9e36c7ce07e82f75d097930e2adc7f) |
| 2024-06-08 22:10 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x38a1899fb0bb01d4bcb0e7a3b3f2819e4ad391c1 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xd0ab2629f3fbe2d3d3e47f0c9fedcb7575f73acd03554bdf951667f9beccb365) |
| 2024-06-08 22:11 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xfba5fe364865c1e1e39210ab1917ae1ac74efb65 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x80ebf5d16431f003ac3fd0eb28f8174c869e42999bb000591aa9f1fcb2442392) |
| 2024-06-08 22:13 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x2d492947538dc737626c70130b863aab0c77c115 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x67d97543852de84c07272b4e0dec3d1aca44fcb9a61db4b8bc1177e9c2a72ddf) |
| 2024-06-08 22:14 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0xfc178b54698eebf3c3d2eb3720ea696f757e0d0e | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xe3a83d51a2bf0bdbe7ac4de6c3db7db26a921fd887fbd9c0188291b881612adc) |
| 2024-06-08 22:16 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x7e97fd1d3332a55b08ebab478de9f05e37dc9961 | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0x77770ae64c57a40d4d871460185a8ed368ed04d1d80649783aae212dba8e3304) |
| 2024-06-08 22:17 | Primary Attacker | 0xbacef3a142e39f14f4f15e22e9248ee4141af18f | Victim Wallet    | 0x8f2f2c237322db9aa76cd627221c918a2e0ec8eb | 0.01           | ETH          | $37         | [🔗](https://etherscan.io/tx/0xbb435bba725b809fef867618b13ce5953b9b9f08f77a4a086d99220538446946) |
| 2024-06-08 22:19 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1.88           | ETH          | $6,930      | [🔗](https://etherscan.io/tx/0xb3c54acd736ad4887eed7f2aca8a4f68d7a9a86a7aeb8a7d6950434e9d21670e) |
| 2024-06-08 22:19 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 2.36038743     | ETH          | $8,701      | [🔗](https://etherscan.io/tx/0xb3c54acd736ad4887eed7f2aca8a4f68d7a9a86a7aeb8a7d6950434e9d21670e) |
| 2024-06-08 22:19 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 7.36           | LIDO_WST_ETH | $31,670     | [🔗](https://etherscan.io/tx/0xb3c54acd736ad4887eed7f2aca8a4f68d7a9a86a7aeb8a7d6950434e9d21670e) |
| 2024-06-08 22:19 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 1.74           | CIETH        |             | [🔗](https://etherscan.io/tx/0xb3c54acd736ad4887eed7f2aca8a4f68d7a9a86a7aeb8a7d6950434e9d21670e) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 0.350680074    | ETH          | $1,293      | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 14730.39226    | USDC         | $14,830     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 6.81           | LIDO_WST_ETH | $29,303     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 8.263421658    | ETH          | $30,461     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 8.8873681      | ETH          | $32,761     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 8.958276569    | ETH          | $33,022     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 9.121772832    | ETH          | $33,625     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2024-06-08 22:40 | Victim Wallet    | 0x674bdf20a0f284d710bc40872100128e2d66bd3f | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | 10.5321738     | ETH          | $38,824     | [🔗](https://etherscan.io/tx/0x05898b988c768215e58fd2375403926d768716a55279ce3cbad31645d9604d80) |
| 2025-03-06 02:32 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xada16604c3ea42c2988b31d4cfeeace3d4dcd1c1 | 10             | ETH          | $22,423     | [🔗](https://etherscan.io/tx/0xe7835d8d84ac8680cfc1648036c97c2e4a6dd6a0667ee274eb93b57dc8aa4a2b) |
| 2025-03-06 02:36 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xada16604c3ea42c2988b31d4cfeeace3d4dcd1c1 | 20             | ETH          | $44,846     | [🔗](https://etherscan.io/tx/0x9cea337f2a611778b8a7dd43fe6ce7abeff13218455185ac01acd4b3f0a4fcce) |
| 2025-03-06 02:39 | Intermediary     | 0xada16604c3ea42c2988b31d4cfeeace3d4dcd1c1 | eXch Depo        | 0x7070777ddce376a625d16cbe5b84428cc481c126 | 29.99997046    | ETH          | $67,269     | [🔗](https://etherscan.io/tx/0x29dcbcd53928ae69cbbfd3e67df194459f8b2d6c0a65fa12d1e2f2f957a47c3b) |
| 2025-03-06 08:41 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x86be93e5183c7924995098b2b0ddb60dd9429d14 | 10             | ETH          | $22,423     | [🔗](https://etherscan.io/tx/0x235eea4c3bfa68dc80c2e795262967c16785739751945b9b35502f19a213ce5c) |
| 2025-03-06 08:45 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x86be93e5183c7924995098b2b0ddb60dd9429d14 | 20             | ETH          | $44,846     | [🔗](https://etherscan.io/tx/0x7e6b0915c76c48d53769ebc8e64c3ee144684b1566c29d2e39ea115b282e98a0) |
| 2025-03-06 08:52 | Intermediary     | 0x86be93e5183c7924995098b2b0ddb60dd9429d14 | eXch Depo        | 0x576c78b6eb5a9ae94d1c0b2e8ecf840a90a16310 | 10             | ETH          | $22,423     | [🔗](https://etherscan.io/tx/0xec5426e1ba2ff677afed52937910946e8660a571e8de2dfc1195a304f8c89bbd) |
| 2025-03-06 09:10 | Intermediary     | 0x86be93e5183c7924995098b2b0ddb60dd9429d14 | eXch Depo        | 0xb93b989658ef9e5fc28a4b1fd9ca78791ac8ec4c | 19.99994194    | ETH          | $44,846     | [🔗](https://etherscan.io/tx/0xaca554a915447146f480768200ae35d643c3c0767afff58722958bbe89a198de) |
| 2025-03-07 01:07 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xf781ccc4082692e80659f68bde96a1ca3300ea1a | 30             | ETH          | $66,001     | [🔗](https://etherscan.io/tx/0xb7c57e0d67c4a2ae70b39fa9800899a7bab2877e8e4ff2c3ce56520652b0ac81) |
| 2025-03-09 01:05 | Intermediary     | 0xf781ccc4082692e80659f68bde96a1ca3300ea1a | eXch Depo        | 0xe3abb195f93a93372fec3b42ef86c2d3e63f3e52 | 10             | ETH          | $21,996     | [🔗](https://etherscan.io/tx/0x6d41e7bfa9375763781caaf2cf33e892bb014b15b97592b023740e2a2bdc8aaa) |
| 2025-03-09 01:08 | Intermediary     | 0xf781ccc4082692e80659f68bde96a1ca3300ea1a | eXch Depo        | 0x3f3e8a263d0e79d3f1f2bf720254de4f5a748530 | 19.9999706     | ETH          | $43,992     | [🔗](https://etherscan.io/tx/0x9da88b1e6337e39ec5ca6761e72befa43055a47869a39f8643ec956c3773c456) |
| 2025-03-09 01:16 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xc8f1ff9d2701a8b2c4f946faf0d8c8fe464057e8 | 30             | ETH          | $65,988     | [🔗](https://etherscan.io/tx/0x2ad2e181acbab6c28554ed66cfea2d7ff86b03a35e2af835fa1b62e400ed835e) |
| 2025-03-09 01:43 | Intermediary     | 0xc8f1ff9d2701a8b2c4f946faf0d8c8fe464057e8 | eXch Depo        | 0xc5a96f0007445e17796438286b151a66629a743d | 15             | ETH          | $32,994     | [🔗](https://etherscan.io/tx/0x8beac6d7d382771e93603a9a3e3a283504bca69911ba3e03b4d9d04dcd71e347) |
| 2025-03-09 02:13 | Intermediary     | 0xc8f1ff9d2701a8b2c4f946faf0d8c8fe464057e8 | eXch Depo        | 0x15c65b58f9a6f2cd1ba637551b1cb17437d81020 | 14.99996591    | ETH          | $32,994     | [🔗](https://etherscan.io/tx/0x248ed0a2ebe8a183673ffe2db5926e765132225fa6833a0218bcb370ae466978) |
| 2025-03-10 03:29 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x0c75df358bebca7a204fed45db9ac235b60a0559 | 30             | ETH          | $60,621     | [🔗](https://etherscan.io/tx/0xaf2a32bd4e65507b260b635c300ed55719d7f810ac854b9ab6914e986a07a6ec) |
| 2025-03-10 06:30 | Intermediary     | 0x0c75df358bebca7a204fed45db9ac235b60a0559 | eXch Depo        | 0x13879e25d699478f89fa005422d54946d9915df5 | 29.99997309    | ETH          | $60,621     | [🔗](https://etherscan.io/tx/0x5dfedc6f99ca0bb657c8e9f3855e849b0d3922f401e95e5371e168f54ca8546e) |
| 2025-03-10 06:37 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x33c2d25792bdc2bcb2609ce96e819ae5d6378789 | 30             | ETH          | $60,621     | [🔗](https://etherscan.io/tx/0xc3cdabc92435f0d1e31c1da8c033bc35ec7b2fd530e66d3bbcb55f4097293e15) |
| 2025-03-10 06:40 | Intermediary     | 0x33c2d25792bdc2bcb2609ce96e819ae5d6378789 | eXch Depo        | 0x47bc1fbe484006474279750f2b3d9592fcb46c55 | 29.99998227    | ETH          | $60,621     | [🔗](https://etherscan.io/tx/0x6d08c9791b19e21cfdfe6c715aed7e42deb5dd70737f1241fcdb5d097a3f515d) |
| 2025-03-11 06:41 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xb11d934e0c49c5c400a766664464ca6b6aaa9ec6 | 30             | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x941f3a5d007354e79615f1111c2330c8197ae7ac659666b2039a3535577993da) |
| 2025-03-11 07:09 | Intermediary     | 0xb11d934e0c49c5c400a766664464ca6b6aaa9ec6 | eXch Depo        | 0x1fe35c433ddb342f9e01933da6e0c90c3be56fd6 | 29.9999735     | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x6f6416ca4e8edac2b617daa3a68e2c702852798d9052238f3569339afdf73410) |
| 2025-03-11 07:12 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x69ddfafffd9426ebfad160d654645aa46ea4649f | 30             | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x8ab9c79a97319a63d85a4a5b41411d4c72f9a3e684d555a17ddecb5e43a5deb0) |
| 2025-03-11 07:28 | Intermediary     | 0x69ddfafffd9426ebfad160d654645aa46ea4649f | eXch Depo        | 0x7d03c57fa61d82e84ef5e6f6a8e9b69257f96335 | 29.99997079    | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0xa05ffcd0f993c98c344501a9cca5759fb0a0c2f2e55720b74eade3dea10b05e9) |
| 2025-03-11 07:32 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xe642d3415d222aaf19e20484476ef443c5ac176b | 30             | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x3abd49522dfc6188c5fb4c08194ab3e6e7a1a3988ba8cffcafa3db17ab35833e) |
| 2025-03-11 07:35 | Intermediary     | 0xe642d3415d222aaf19e20484476ef443c5ac176b | eXch Depo        | 0x78f6104dfbd96be478e7640ae4dea132e8d51874 | 29.99996857    | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x9d457313fa2cc1d946da0dbcb407f076c9a514f63bf2ab5459c63da9f0d8e382) |
| 2025-03-11 07:39 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x7932b04d7b2cf16e183fd44b521ab1336756df2f | 30             | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x6692de5555764ea1736b0a154172900a1fd1363c7459264dd9eeabe1461bfa6c) |
| 2025-03-11 07:45 | Intermediary     | 0x7932b04d7b2cf16e183fd44b521ab1336756df2f | eXch Depo        | 0x4d44df6dd513b50630ce51dc34974cc3a710b57c | 29.9999714     | ETH          | $58,057     | [🔗](https://etherscan.io/tx/0x8429491db993762beb41becfdff3f6f7676df4625d6c60c3f6c0f794ad323cf7) |
| 2025-03-13 04:51 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | 30             | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0x427baf56c0fb6a6b0e795b6f6136f7284bf2f14bc584be46e888697d229d3fa6) |
| 2025-03-13 04:57 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | eXch Depo        | 0xc81097dcf71c02de27f0517da6e6b1fc7a4d41cc | 29.99997302    | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0x34e571855539c120d95ed62072c3732cfb92424a44781de238863b6b440a4572) |
| 2025-03-13 05:01 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | 30             | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0xbbcf7af262bafd9076a904a5d85a9b38daa8d98d9b2100e8e59f1ba1e039ede6) |
| 2025-03-13 05:03 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | eXch Depo        | 0x8d38685c9940a6bc3396adf310daf8bc27944df9 | 29.99997745    | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0x0053cf6e95b18e39a1cf1b2c1cb2aaa131e15f9f92b05204a88594736562b952) |
| 2025-03-13 05:04 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | 30             | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0xcc08265b21bf09b4fc15e917cf11f17002534bc02b0c30b7cdd084bec61dd444) |
| 2025-03-13 05:13 | Intermediary     | 0x48c2fabbed679b5ca1caba0817d528404fdc2162 | eXch Depo        | 0x002536416d7a20848067fde6bb4cd28bc742271c | 29.99997926    | ETH          | $57,201     | [🔗](https://etherscan.io/tx/0x16ef3b6051794815607a950dc78cfa195f82995673d4c0ec765a1d2e8e7395e4) |
| 2025-03-14 02:16 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | 30             | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0x3d1d600e5846c877989486e8d6d453e20f2c8294f1cb5ed581a1d663e7118492) |
| 2025-03-14 02:19 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | eXch Depo        | 0xb7b6a1336d3d308101faa1223da644d0fbb63062 | 29.9999723     | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0x6ca8db60c3e6a8e401e90d095609a294549a31ac38199b11d9e80609bd0de175) |
| 2025-03-14 02:21 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | 30             | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0x0b57bdbd695027564051834542e11cb909560c1c0e1cb5b21294f4e67d6e40fb) |
| 2025-03-14 02:25 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | eXch Depo        | 0x416db290926960e9835d3cb8c0404c333c56a00b | 29.99998046    | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0x0b5145be479470e09041cd2bada41baf3da00ad30a3b55dab8c4256d09387f8f) |
| 2025-03-14 02:40 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | 30             | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0xec06b323da1452572851c52741c65c416b6dad07dd8f1947a4dddadebeddd96d) |
| 2025-03-14 02:44 | Intermediary     | 0xbdaef4049cdc0b92c9c969add4ad5a5799421ee2 | eXch Depo        | 0xa5c05b6ae64e457aa2168d73942a5460f4924a0e | 29.99997889    | ETH          | $57,816     | [🔗](https://etherscan.io/tx/0xbc94bf9834373e26c12176159894b38d175ff06118546444004be51058dfd8ba) |
| 2025-03-18 02:38 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xa5892c54759f9e296e67b2a6afbdf908676cd875 | 30             | ETH          | $57,752     | [🔗](https://etherscan.io/tx/0xd3666edb02ccc51485f630866526ae68ac4445ac5165556c6f4f097444edb5ad) |
| 2025-03-18 10:16 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xa5892c54759f9e296e67b2a6afbdf908676cd875 | 30             | ETH          | $57,752     | [🔗](https://etherscan.io/tx/0xd73be2cbbf7c61f253a7a9bcec52d588a48a772b3f190c2e3d23cc644e9b7773) |
| 2025-03-19 05:04 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xa5892c54759f9e296e67b2a6afbdf908676cd875 | 60             | ETH          | $122,995    | [🔗](https://etherscan.io/tx/0x4ef51bce1680edb767edec4e20b32cf8c93b670481f133ddd4d33bfada445546) |
| 2025-03-19 05:07 | Intermediary     | 0xa5892c54759f9e296e67b2a6afbdf908676cd875 | eXch Depo        | 0xb89d9ade1d6551e60595bf68afdc4476a21836a3 | 30             | ETH          | $61,497     | [🔗](https://etherscan.io/tx/0xf2218c8d8b70fe2d06be29b102927021b883b39f2bad908ec9f9aadf23585010) |
| 2025-03-19 10:46 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0xe5e95f541624af7dd42c5efaea4c56e3a0acf73a | 100            | ETH          | $204,991    | [🔗](https://etherscan.io/tx/0xd8290e64c1696b1d0a89b35cf54689ba2d62ad8904d90fb29fc8a3ff0bb6322f) |
| 2025-03-20 02:11 | Intermediary     | 0xe5e95f541624af7dd42c5efaea4c56e3a0acf73a | eXch Depo        | 0x186cbf884dac7af20ae0155c3b42ac2faf9f141c | 33             | ETH          | $67,969     | [🔗](https://etherscan.io/tx/0x443cce0d8a03614c29be499ec565b83bcb5dd4496a72520e78804fd5fae4e2b5) |
| 2025-03-20 02:25 | Intermediary     | 0xe5e95f541624af7dd42c5efaea4c56e3a0acf73a | eXch Depo        | 0x3ccd3b1d441a793aaccc878bfa9ace607acbfc53 | 32             | ETH          | $65,909     | [🔗](https://etherscan.io/tx/0x489821b0874dc39313895038ea555c6cb0df1b568ec8753659af787f6d3203d2) |
| 2025-03-20 02:41 | Intermediary     | 0xe5e95f541624af7dd42c5efaea4c56e3a0acf73a | eXch Depo        | 0x9c34fc8f1596003e414e9efe4f11d5eeef152b4a | 34.99994287    | ETH          | $72,088     | [🔗](https://etherscan.io/tx/0x1b9a68c185d7746f4949b5613211308841cb9fbefbd45d55703f1eb299faad9d) |
| 2025-04-21 05:30 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | 50             | ETH          | $79,332     | [🔗](https://etherscan.io/tx/0x798726ed35a3f93918bc2f6c1ee9d49ffa8e242eae92dc2f8214d3e89f6295e6) |
| 2025-04-21 05:34 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | eXch Depo        | 0x66d84ccffedd168c6047a4ecce8affdf39d20e28 | 49.99998308    | ETH          | $79,332     | [🔗](https://etherscan.io/tx/0x67514d9c301f657acac72c9243bace203c2c21d4c892d63849292ebe46f7516c) |
| 2025-04-21 05:39 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | 50             | ETH          | $79,332     | [🔗](https://etherscan.io/tx/0xed62c0859e3a81a0234df2cb48dcc1f6413f985e480e81e5983d217916c6fce9) |
| 2025-04-21 05:45 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | eXch Depo        | 0x0b56e51a80a5196377da96d2d106af37d434930f | 49.99999058    | ETH          | $79,332     | [🔗](https://etherscan.io/tx/0x7d319a7b162ebac3b360ad7e832b8626566257beb80768f0f36b4597af3ec03c) |
| 2025-04-22 02:17 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | 50             | ETH          | $87,588     | [🔗](https://etherscan.io/tx/0xd8e232451d4cab82bfd99f61d3d5a5beb28a981690ecb37fb8d66690ed5eab61) |
| 2025-04-22 02:22 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | 50             | ETH          | $87,588     | [🔗](https://etherscan.io/tx/0x95afb0cf9eba991b864d22363cb2340ebddd375e1701ae38bec956b727f867f8) |
| 2025-04-22 02:24 | Intermediary     | 0x0841d77dbbcaffb1604ead4f36019f9d3a24ccba | eXch Depo        | 0xdff121fb757e0223f17129fa987978dd374b8f2f | 99.9999874     | ETH          | $175,175    | [🔗](https://etherscan.io/tx/0x45e75a7bccdd64e49363d5998599df262d9f9b0a8b191d48df609db2b4804743) |
| 2025-04-22 03:22 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | 50             | ETH          | $87,588     | [🔗](https://etherscan.io/tx/0xbda8a9c4949a124c0d61922bdc720d22ff820b4555f2e0b7b3d26a7f3cd3ba48) |
| 2025-04-22 03:29 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | 50             | ETH          | $87,588     | [🔗](https://etherscan.io/tx/0x4ff08939a789272fde2afca8a272e5843196b90c2fa4892fddf0e0a6354f7977) |
| 2025-04-22 05:33 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | eXch Depo        | 0x8e143ae951b5cd1bc5b99cdc3667723b6c7f8ce9 | 99.99998827    | ETH          | $175,175    | [🔗](https://etherscan.io/tx/0xb8fc0605c141f0f4d7e9ccf1d560f597e44669ebb59147d76399f7da1a90df50) |
| 2025-04-22 23:28 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | 100            | ETH          | $175,175    | [🔗](https://etherscan.io/tx/0x54665fb93bca5b8b1cb212c27922accf2e43bce0facb92ff1dd4f3b53a6e0e0b) |
| 2025-04-22 23:32 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | eXch Depo        | 0x7b58824b01a33528a0149fd52b9d06f5361756bd | 99.99993426    | ETH          | $175,175    | [🔗](https://etherscan.io/tx/0xa4f987e0773b0b04e82fbb5fcebf7cfd228b53a5affd18c366d80481ec609940) |
| 2025-05-07 06:56 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | 5              | ETH          | $9,089      | [🔗](https://etherscan.io/tx/0x4eedd3ab787d7f19920c936aeff36a8e3ead5967bc1831206cd2a7bf9d3ffda5) |
| 2025-05-08 01:54 | Intermediary     | 0x786c44914ea8d29f96e649741bc14a60660704ce | Intermediary     | 0xdafbf7e88e8ef502aadad88e660157f192ac4de7 | 4.999876067    | ETH          | $10,900     | [🔗](https://etherscan.io/tx/0xc9bf983c6bae235aaef0a79a18908b312b31e6d2dae951c35b85d812ad5985cd) |
| 2025-05-26 01:59 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 0.1            | ETH          | $256        | [🔗](https://etherscan.io/tx/0x8d7a4b8138ffbe3950446f0082bfd93021a3ba50df73f8f51b94d209f152bb11) |
| 2025-05-26 07:11 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 10             | ETH          | $25,614     | [🔗](https://etherscan.io/tx/0xbdf734cc58772b66e5c5ada6ee1a8ec76e7bc7084b65637f4e0e9f2efbf19a6d) |
| 2025-05-26 07:19 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 10             | ETH          | $25,614     | [🔗](https://etherscan.io/tx/0x7a01703658a6c42ed69126b77f53da04bd72f3906231fe5aa98328803efe00a2) |
| 2025-05-27 02:30 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 10             | ETH          | $26,613     | [🔗](https://etherscan.io/tx/0x0a294963cf1209a4e91abf2900a9a0f37e3b9ce7d53fd59e1dc431f04df685b1) |
| 2025-05-27 02:37 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 10             | ETH          | $26,613     | [🔗](https://etherscan.io/tx/0x0b34527be7bac6f1bee63a62294b618194128dedf6cd524858440228399e2233) |
| 2025-05-27 02:51 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Tornado Cash     | 0xd90e2f925da726b50c4ed8d0fb90ad053324f31b | 10             | ETH          | $26,613     | [🔗](https://etherscan.io/tx/0x818b7e328f13763e97ec4e86d93a37d47fd909c5556470523de3f81705fb5ce6) |
| 2025-05-27 07:10 | Intermediary     | 0xdafbf7e88e8ef502aadad88e660157f192ac4de7 | BitcoinVN Depo   | 0xca1379a7dccb147164b209d15b37290912332d7c | 4.99           | ETH          | $13,280     | [🔗](https://etherscan.io/tx/0x72881a1ab86f68b1d57afd1e68e6547f2a4df59925ee587d3a36b7e31e231ca7) |
| 2025-05-27 08:07 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x94cad8b95d11f03a5f53cf157a0ad0211e8dd2a1 | 0.2            | ETH          | $532        | [🔗](https://etherscan.io/tx/0x2283c1e541ae79099106ea007d60d870b3c15370c46e83ff21ad9a232a47ec2a) |
| 2025-05-27 08:23 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0xe6b8eca2fdc67a253388c9d4e21b0fb3c1e66a83 | 1              | ETH          | $2,661      | [🔗](https://etherscan.io/tx/0x9131f7717b181c1ab62a14de3f6ccf9d40e9140d451259fde44e4a9f1a215933) |
| 2025-05-27 08:32 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0xdd79196331202cd923f3e7bd4280018ca2d67543 | 2              | ETH          | $5,323      | [🔗](https://etherscan.io/tx/0x941dbe17ab471b4c8a0003f15ab258067ed5f2ed38196a5c15653106b2dda829) |
| 2025-05-27 08:46 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x4c725719a5bcc1d7aa1194bac3beb36ee0ac839b | 3              | ETH          | $7,984      | [🔗](https://etherscan.io/tx/0x1358924b083f604bdd8a67834ab870f22329ae18395a4ec7a6091e7b972731b6) |
| 2025-05-27 08:51 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0xe3333e86e82669eeb00dc7638181058220b1b85e | 3              | ETH          | $7,984      | [🔗](https://etherscan.io/tx/0xbf24f760871cb15abb368692889bab3f6c71a691d34066c1e7717ed85a33547b) |
| 2025-05-27 08:59 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x3cfaf7b910828b9344aa8a9f97f59220318617d4 | 3              | ETH          | $7,984      | [🔗](https://etherscan.io/tx/0xd43b483949c892117b0d8e993c50b6629248e6ce35ac3a573cc53545a117d448) |
| 2025-05-27 14:19 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x7e4c190db365550f11debe63903ebc4558f17451 | 5              | ETH          | $13,306     | [🔗](https://etherscan.io/tx/0x1d3ac283735729f117323ccfa334104f170ca78a1c70a09ed129d9dfadace46a) |
| 2025-05-27 23:46 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x8a1c20e4e79d979ac1f7514fef2b0e36e554f96b | 5              | ETH          | $13,306     | [🔗](https://etherscan.io/tx/0x354a69d72d0c7a82c2bdf1f002b5e162dacce5c240fcfce685bf8075cbfb4c98) |
| 2025-05-28 00:04 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x9bed6e3dab814c13df27b1fbb8bf0b4f7ada8ed6 | 5              | ETH          | $13,313     | [🔗](https://etherscan.io/tx/0x31e469ea92b5d896118025c749696682b3a8726053cf666a9430f830314df232) |
| 2025-05-28 00:10 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0xfcbf282facb57df4c12fcc45700ab3ea01fb8f3c | 5              | ETH          | $13,313     | [🔗](https://etherscan.io/tx/0xd450bb612d303fa717162a73cc06e261c610fbff8af8ddd3adda4ff30c86dba0) |
| 2025-05-28 00:51 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xd83f0f62547ba4e6df2bb166c5e18570d17af55b | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0x9c40d2aba441309d0a55bfa6cdc26fc6d4ec38fed709dd42c6a783369e6658d7) |
| 2025-05-28 01:01 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x72703217f0b33fa2fcdf3aedd5118bcce52cb328 | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0x53b0321aff50c01b8769fded423590f999b41d608b91785757168182875e7b13) |
| 2025-05-28 02:30 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0xd79c92078e765b2809805844c54c6ba0ef57f6f7 | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0x337334ce4d44f847b41f1ef09b8dc8c43d9b381ef77c4c690ceb76706d39a045) |
| 2025-05-28 02:39 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xfaa9121849f299385acd5017fd5d086de219368c | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0x305fb944cacc674350bd8f0f09b577e26acf4fb4756710f47ada516990c19a96) |
| 2025-05-28 02:48 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x069304073cdace751a863fc4658bfd1a7d95c4f9 | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0x35533aa5bd88ec7360920650d459b26a48034fc3059c9a8e6f6a55a87a009655) |
| 2025-05-28 03:16 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xa53106af6b95751f205cedaa8617249e0e379d7a | 10             | ETH          | $26,625     | [🔗](https://etherscan.io/tx/0xe1f534923f1c5ff96a3f560eeef762e88ee6602799e0eca42ded26f734d2eac0) |
| 2025-05-29 02:40 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x2bc9cbb613876409012ab5c801a980d66d9f3ef5 | 5              | ETH          | $13,402     | [🔗](https://etherscan.io/tx/0x4ec29ef9c8d771aa73780122a135327872670e235542c68678041bb353c3bdb5) |
| 2025-05-29 02:43 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x3995f826abc0ffaf03cab6931fb9b3d982a55686 | 5              | ETH          | $13,402     | [🔗](https://etherscan.io/tx/0x9a942ed31f0531564373c0a91053eb0f35595a06678601daa8b5bdd7b44474a5) |
| 2025-05-29 02:59 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x36ed6385a7f7083cf2b9a05806abec3978683fed | 10             | ETH          | $26,803     | [🔗](https://etherscan.io/tx/0x8bddf24f10f800a853ce00dc85e086db2967822e2412f2df2f2ab54910e6b14c) |
| 2025-05-29 03:21 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xc73d1ea63439f6e664befd0a515f940fc0ff4bef | 10             | ETH          | $26,803     | [🔗](https://etherscan.io/tx/0x817e1bf0a5a67db475d840a09abd3ebae307c2c979b42df727091089fbaa42a1) |
| 2025-05-29 06:38 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xc5e652584600c7a0d92209fd9e79283d7e7f2122 | 10             | ETH          | $26,803     | [🔗](https://etherscan.io/tx/0x5662f96acc256499e2e5c90b7ecca7199fc12a365d9e0d9a969d7bf9164ed6cc) |
| 2025-05-29 06:49 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | BitcoinVN Depo   | 0x46d40089485e582972c98320029a683e41669a39 | 10             | ETH          | $26,803     | [🔗](https://etherscan.io/tx/0xc869f97095adf12cbfe53557367956a9445153334466375ba6ba1f53cff8fda5) |
| 2025-05-29 07:58 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xa3dc37b85cebebf3bfabe3a5bf84d3381633739d | 10             | ETH          | $26,803     | [🔗](https://etherscan.io/tx/0x33325e796d075baad14275025b670257f58b83ea7db118e665ecb5c19666cbaa) |
| 2025-05-30 01:44 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x37b5bd8e79508b141e7c1f555fe8230e2a9267a8 | 10             | ETH          | $26,321     | [🔗](https://etherscan.io/tx/0x003a8721c19d70f76caea6ae797eebddcb64906fa43e5d28285c395ba9ae0bc5) |
| 2025-05-31 10:28 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xc3c94ed121b70d80b04565a93faaf65c5521734b | 10             | ETH          | $25,369     | [🔗](https://etherscan.io/tx/0x9b726823a625fb65d316b89cb64986e44d1513c4ea059077e242c05195b55079) |
| 2025-06-07 15:32 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xe6059e72e85e310757363127ea8d53493c619ecf | 10             | ETH          | $25,399     | [🔗](https://etherscan.io/tx/0xffbecac9d5c2ad8dc98ba5f5c5bb2b2b07c464e1ff7235ef64cddceccc05eb69) |
| 2025-06-07 15:35 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Dormant          | 0xd64b36a33274167402598fa6af35e750120bc3a2 | 10             | ETH          | $25,399     | [🔗](https://etherscan.io/tx/0x651866115fe42853c7b1272fa62b887c0dfe3d16acf78c72f11c445a8ffa245f) |
| 2025-06-07 15:46 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0x0f45123c682250e4f6c53841f0c493dda2e41a6e | 16             | ETH          | $40,638     | [🔗](https://etherscan.io/tx/0xbacab9e5371121c3ad9dbd60129ecdaa683db109eae9f7732e8d5200fd44973f) |
| 2025-06-07 23:57 | Primary Attacker | 0x44f887cfbd667cb2042dd55ab1d8951c94bb0102 | Swapuz Depo      | 0xb6baebbf3546d72619677508d668a8a5e781531c | 10             | ETH          | $25,399     | [🔗](https://etherscan.io/tx/0xc3c985b672a2276d6cdbe8c703c5adf060391589885ff04b72d415335f97fee0) |




### Victim / Impact Wallets

- 0x8e534af51fb580c546f30d4175014af4bee921d8 - Victim? (2025-06-08)
- 0x59f3163ab39b8b90daf57508bc1faecb2f2cd374 - Victim? (2025-06-08)
- 0x06afc66ff10de97ee56b35867ee5d13e7a7b1b2d - Victim Wallet (2025-06-08)
- 0x7d7e9641a67755f7126d1cfc7f99b5bf7a0b8f45 - Victim Wallet (2025-06-08)
- 0x1496ab088ae2302e94b6b9670a9b9091de856f5c - Victim Wallet (2025-06-08)
- 0x2dec0bdf73d6521b98c4e8739edbb2e58e891e00 - Victim Wallet (2025-06-08)
- 0xd2d4c571d047db54644dc5de65af1b48cfb0e04f - Victim Wallet (2025-06-08)
- 0xc41d55bec55bd844809e13e19d9acb3a13e941e0 - Victim Wallet (2025-06-08)
- 0x52ba88e942a81b6aaaf6ceed3adc6ad9a1b71d38 - Victim Wallet (2025-06-08)
- 0xbf8fa544f40caedad29949665a58fde8c0ff090d - Victim Wallet (2025-06-08)
- 0xb92398584108af3dd8ae9cbf4e2bb7ecded30f75 - Victim Wallet (2025-06-08)
- 0xfa0dd8fc7381939a64be6f150335b072c3e3c98e - Victim Wallet (2025-06-08)
- 0x51ef507e59d66918ae09bfb606060a60399f090d - Victim Wallet (2025-06-08)
- 0xa84f9f7939e8adf5c5d3cf18664df2908d255042 - Victim Wallet (2025-06-08)
- 0xe2efc4082108da43eb8082d5c64b8744a69b292d - Victim Wallet (2025-06-08)
- 0x08e80e6c538bbb5976159317eba84b325efb16a5 - Victim Wallet (2025-06-08)
- 0x63e7bcadc5661b6abe62bff4f52cc20c70006371 - Victim Wallet (2025-06-08)
- 0x5b000d1ccb6127d8a244d35d28287419f7c1db82 - Victim Wallet (2025-06-08)
- 0xfc0b880ed947985740c1db850f37d3139bc27af8 - Victim Wallet (2025-06-08)
- 0x70eeda38dc4685c511e05de9819607d191be7a02 - Victim Wallet (2025-06-08)
- 0x98ed261bdb2da93408b4471d9e6fab6e11437295 - Victim Wallet (2025-06-08)
- 0xb75532e1061245baebcaa2e60fc0c71d7fffc66d - Victim Wallet (2025-06-08)
- 0x71a9fcf0f3fd483f1c13e6d5836b9736f66a93f7 - Victim Wallet (2025-06-08)
- 0xe7449c9111936cd1dbc15c63139fb85aa886c4cc - Victim Wallet (2025-06-08)
- 0xb98e69b59686be51046a4fa97b86a2fc92d7288e - Victim Wallet (2025-06-08)
- 0x8d40c0fabec34fd79dc3bc5b08352025785439d3 - Victim Wallet (2025-06-08)
- 0x57437f04ca7896aab747b988f97d3f01134fa02b - Victim Wallet (2025-06-08)
- 0xdf5f49455797d146d46c9d9caba116a855c267d4 - Victim Wallet (2025-06-08)
- 0x2a7cea412a00d5694485843bd53c255ed64b1371 - Victim Wallet (2025-06-08)
- 0x45326101d40226dc41202cc935062707bb9e7ea2 - Victim Wallet (2025-06-08)
- 0xec68978fc9da315af3826775d70d3ebaed76c429 - Victim Wallet (2025-06-08)
- 0x4b58c10cf4068f38a101e51d7ee3b5469c854d5c - Victim Wallet (2025-06-08)
- 0xc0ad40b17c8cd67c3e8d3da0c0d4de74d1a1cd3f - Victim Wallet (2025-06-08)
- 0x3bdebfc8d4ca345f8ee93b44c09d3b7ce7210d9d - Victim Wallet (2025-06-08)
- 0x9372ad44ef76c6c42ea08bda06961f115c5bb4f4 - Victim Wallet (2025-06-08)
- 0xfba5fe364865c1e1e39210ab1917ae1ac74efb65 - Victim Wallet (2025-06-08)
- 0xc737b3d19565431295d1c9b079ca35b862481e50 - Victim Wallet (2025-06-08)
- 0x6c108bb2a6f0a607bc35d86d989994cd716b5998 - Victim Wallet (2025-06-08)
- 0x38a1899fb0bb01d4bcb0e7a3b3f2819e4ad391c1 - Victim Wallet (2025-06-08)
- 0xb81dc3e1d623ce42a7168be0520206e8e4053f52 - Victim Wallet (2025-06-08)
- 0x7e99d19b0ac4093d8f5e9a419f311ff4dbf98f46 - Victim Wallet (2025-06-08)
- 0x2d492947538dc737626c70130b863aab0c77c115 - Victim Wallet (2025-06-08)
- 0x5bd60ffc6328801b2091fd504663f0e3c88e0934 - Victim Wallet (2025-06-08)
- 0xb9ec3f9e12fa0d39cf09e35bb8badfcfb0725a94 - Victim Wallet (2025-06-08)
- 0x83c223979048675dc582299ab1893830328366c1 - Victim Wallet (2025-06-08)
- 0xfb38ecbe9202375d9152bffe009efaf49b563f96 - Victim Wallet (2025-06-08)
- 0x8f2f2c237322db9aa76cd627221c918a2e0ec8eb - Victim Wallet (2025-06-08)
- 0x7e97fd1d3332a55b08ebab478de9f05e37dc9961 - Victim Wallet (2025-06-08)
- 0xfc178b54698eebf3c3d2eb3720ea696f757e0d0e - Victim Wallet (2025-06-08)
- 0xc9f29e8a21586f5134fae3d61797731be8c303f8 - Victim Wallet (2025-06-08)
- 0xad29f3bd54a606d6570fe92295b48a7d392dd4e2 - Victim Wallet (2025-06-08)
- 0xf9e84f452a818b383d1b9e7eb74871cbd0ef245d - Victim Wallet (2025-06-08)
- 0x0ca8dfc9229f25789217dcc4771b1d79b3f961e6 - Victim Wallet (2025-06-08)
- 0x399d40d5be83a28bb66ec205f6ff738e8a8e9397 - Victim Wallet (2025-06-08)
- 0x8f3be4c92ea38b1db5501db3838966739494de89 - Victim Wallet (2025-06-08)
- 0x553200b15ab249dd18c5b4f1f1e5a00886562898 - Victim Wallet (2025-06-08)
- 0xf9468fbd6feb138b118926cd0313d1e4a16e4f50 - Victim Wallet (2025-06-08)
- 0xc744087c95007d5061d26ec8c77774ba5e44fe06 - Victim Wallet (2025-06-08)
- 0xa0ecfafef37a769067e741c132c591744267e25d - Victim Wallet (2025-06-08)
- 0x674bdf20a0f284d710bc40872100128e2d66bd3f - Victim Wallet (2025-06-08)
- 0xebc00db31ef22da678822cbae9d54e1cc5af181b - Victim Wallet (2025-06-08)
- 0x9e8449aa1f6a5b547f26f165023c212df07e2064 - Victim Wallet (2025-06-08)


