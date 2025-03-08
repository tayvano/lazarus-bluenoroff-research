# WazirX

Date:: July 18th, 2024

Time:: 06:19 UTC – 14:48 UTC

Amount Stolen:: $230,000,000

Tags:: 👛 Trader Traitor, Keys Not Compromised

--


## Details 

*Note: mostly from [Rekt](https://rekt.news/wazirx-rekt/)*

According to a technical breakdown provided by Mudit Gupta, the attackers began laying the groundwork at least 8 days before the main event, conducting small test transactions to set the stage.

Their target? WazirX's multisig wallet, which had six signatories, five from WazirX and one from Liminal, their custody provider. This was confirmed by WazirX in their preliminary report of the exploit.

Instead of a straightforward drain, the hackers opted for a more insidious approach. They set out to upgrade the multisig wallet to a malicious version under their control.

To achieve this, they needed to overcome WazirX's security measures, which included Ledger Hardware Wallets for signatories and a whitelist policy for destination addresses.

~~The attackers likely compromised two of the four required private keys directly. For the remaining two, they employed signature phishing, tricking signers into approving what appeared to be a normal USDT transfer.~~

This deception extended to Liminal's interface, where WazirX suspects a discrepancy between the displayed data and the actual transaction contents allowed the payload to be replaced.

Minutes before the hack, a legitimate USDT transfer failed, a red flag that went unnoticed.

Two of the four signatures were actually for upgrading the safe to the malicious contract, not for the USDT transfer.

With all pieces in place, the hackers executed their exploit.

Using the two compromised keys and the two phished signatures, they successfully upgraded the multisig to their malicious contract.

Critically, one of the phished signatures came from Liminal Custody, the co-signer responsible for final checks.

This suggests a significant failure in Liminal's verification process, a vulnerability the attackers exploited to devastating effect.

(Note: The attackers used phished signatures for 3/4 and Liminal signed the 4/4 automatically upon request)





## URLs

- https://rekt.news/wazirx-rekt/
- https://liminalcustody.com/blog/update-on-wazirx-incident/
- https://twitter.com/0xVazi/status/1813865773213077752
- https://twitter.com/liminalcustody/status/1813889131338199186
- https://twitter.com/liminalcustody/status/1813889133968056660
- https://twitter.com/liminalcustody/status/181388914378266631
- https://twitter.com/liminalcustody/status/1814280472614383819
- https://twitter.com/zachxbt/status/1813896332022882686
- https://twitter.com/zachxbt/status/1813896342894465091
- https://twitter.com/zachxbt/status/1813896353296322987
- https://twitter.com/zachxbt/status/1813896362674782375
- https://twitter.com/zachxbt/status/1813896371659067620
- https://twitter.com/zachxbt/status/181389637559749017
- https://twitter.com/tayvano_/status/1813867117240021120
- https://twitter.com/moo9000/status/1814155634180526303
- https://twitter.com/tayvano_/status/1813885359174099192
- https://twitter.com/Mudit__Gupta/status/1813881385800913327
- https://twitter.com/CyversAlerts/status/1813834131165286464
- https://twitter.com/WazirXIndia/status/1813843289940058446
- https://twitter.com/ArkhamIntel/status/1813887774191231337
- https://twitter.com/CyversAlerts/status/1851239095730602136
  

## Onchain

- delegate call to malicious contract
- 0xfbffef83b1c172fe3bc86c1ccb036ab9f3efcaf2
- changed the storage of
- 0x27fd43babfbe83a81d14665b1a6fb8030a60c9b4
- so that the safe singleton for 0x27f is now
- 0xef279c2ab14960aa319008cbea384b9f8ac35fc6


### Addresses

- 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e - Tester addy
- 0x6eedf92fb92dd68a270c3205e96dccc527728066 - Exploiter
- 0xab7f74febc2e13a7636c305794e1c0ddd9e0d779 - Exploiter connected
- 0x9a638c0d1a40086d61584aa8861a4828440045c2 - Used to withdraw GALA
- 0x8F5376C6EDDC246D7E57040B1B0647FD3CBAFF89 - Used during hack, used to withdraw GALA
- 0x04b21735e93fa3f8df70e2da89e6922616891a88 - Direct Theft
- 0x35febc10112302e0d69f35f42cce85816f8745ca - Used during hack
- 0x90ca792206ed7ee9bc9da0d0df981fc5619f91fd - Used during hack
- 0x9652E54fd0fc60F198E2C0310F2EdfD508FfA1c8 - Used during hack
- 0x231e2547ca75b8f9e22be1b45845db07300cf9b4 - Used during hack
- 0xb8343bcc0256aa2d11022f12941c40c9822b6afb - Used during hack
- 0xcfbd2326234ddb5f0eaea69313b864c3dff00008 - Used during hack
- 0x62b4daa783bb22cf45b6524c63c0477ee10b215f - Used during hack
- 0xb822ae96ca67ddc4129b254d46c5cd904bc1c33e - Used during hack
- 0xc5265fb6ebe88d62626e2212234c7d3b8b7ef912 - Used during hack
- 0x313F7c62B4Ac4377eBD69FCebBB484A26faeF678 - Used during hack
- 0x0cffef1c95e280abc2ff1c44693eee19de921093 - Used during hack
- 0x252bdaaee67e3a94d80c98b22b6e85c2e4a86e56 - Used during hack
- 0x6ad4486edfbceafc170c3dd7762e8be1ddae12c2 - Used during hack
- 0x57949b506d895d9ededdd9883bc301a820fdd063 - Used during hack
- 0x2d8231e7cb5d21887f0b007878a4bdd8b1a9c0e4 - Used during hack
- 0xfae288c79c337e7f55db70abe85d39b59ed130ea - Used during hack
- 0xba19fa8e1ebab926a13ebe35ad595d2a4e2c7081 - Used during hack
- 0x6febb3debfcaea0a58fb8a648d5689e691fcf558 - Used during hack
- 0x7189c049E5b5E07EA5Bb70c90880bffdB65C6d9B - Used during hack
- 0xc63dd6d4efe063807a521ebcbff6c61cd786b2e9 - Used during hack
- 0x6ea4cd20a0930eaf5b0bc097238ceaf9008703d5 - Used during hack
- 0x1957a4c3d2edcb893c9b85833a417ea035d3aed7 - Used during hack
- 0x361384e2761150170d349924a28d965f0dd3f092 - Sitting
- 0x58D3B2fD2Ce20A7149244d7e34D18b9b55448E7a - Sitting
- 0x668399a6604c41d46c81430e4dff71443d44efe6 - Tornado Cash Depo 00
- 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 - Tornado Cash Depo 1
- 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 - Tornado Cash Depo 2
- 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b - Tornado Cash Depo 3
- 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 - Tornado Cash Depo 4
- 0xa4d155734f0b704ea5568ce89b687d2285279845 - Tornado Cash Depo 5
- 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc - Tornado Cash Depo 6
- 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a - Tornado Cash Depo 7
- 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a - Tornado Cash Depo 8
- 0xfb4f28197258a085969e8c4000090a65c9000eba - Tornado Cash Depo 9
- 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 - Tornado Cash Depo 10
- 0x06414c80e12d3c4c831acb615f98abf7d6387b4a - Tornado Cash Depo 11
- 0xa6e894326214535916bf0b7d879cccc734b6120e - Tornado Cash Depo 12
- 0x503b5d609ded2f5b9c9c50adf0b551145077ce2f - Tornado Cash Withdrawal 00
- 0xcd30a63019ab12fd617a3669e5d27af0b02a2890 - Tornado Cash Withdrawal 00
- 0xfee97845154e16d12e44cfb1b42d9a6b65725684 - Tornado Cash Withdrawal 00
- 0x4d0a5e0a94468839db9db0a61d668ea19a7ba7c7 - Tornado Cash Withdrawal 00
- 0xe93d293af6e7baa4081062a656d0b8c236c2252e - Tornado Cash Withdrawal 00
- 0xc22fb23ed9634059b66be469b845251123814069 - Tornado Cash Withdrawal 00
- 0x5ba7b216e8d1e898f56418730d6a916ce2e57198 - Tornado Cash Withdrawal 00
- 0xcd0a731a65c07b0340c055e379af96d2a704a4b8 - Tornado Cash Withdrawal 00
- 0xebba346a3788e3da5e05f2ead2f2cf0293c95563 - Tornado Cash Withdrawal 00
- 0x2c4af2b55654627df0e5cbf33cc7f2dcff6d35aa - Tornado Cash Withdrawal 00
- 0xa70f8cdbe25d4bab8d77168832c0a680f38aed40 - Tornado Cash Withdrawal 00
- 0x61e89052cfa44c160afa96f93ff41e707366bf22 - Tornado Cash Withdrawal 00
- 0xe326c1b51c338371f12d880b4a6e75295d51a204 - Tornado Cash Withdrawal 00
- 0xa71e05fb34fb79702da02e0f94e376382016d014 - Tornado Cash Withdrawal 00
- 0x2a1cf2bc9f7c5f7fb97912075aaf8a79e57d6dc4 - Tornado Cash Withdrawal 00
- 0x83c3ffe81cf6d0def25e485cfc1db5d2cf7d88c6 - Tornado Cash Withdrawal 00
- 0xfcf701753198c6870a7b2433039d66261035b926 - Tornado Cash Withdrawal 00
- 0x39ce6c2fc496e1fe2341a77c6ce946deab50955c - Tornado Cash Withdrawal 00
- 0x3e59fc3e9ab3f729be5f5a88398978a314807c55 - Tornado Cash Withdrawal 00
- 0x29c86175b1f086ecedb5f2e6f993c1ece1ebd143 - Tornado Cash Withdrawal 00
- 0xff3f62158278c53db2d1c523c867e4f7229b051b - Tornado Cash Withdrawal 00
- 0x25598a14b023d88cca4395ae61ea987447078e33 - Tornado Cash Withdrawal 00
- 0xb461ffcbe2e54b22734e0f3cc375d4d456d4a1ff - Tornado Cash Withdrawal 00
- 0x75521e328b2424e81d61c152aaf6f8dc8eeefbd1 - Tornado Cash Withdrawal 00
- 0xeaa51d76d222bb502100969c1e61fe63ec48a3e4 - Tornado Cash Withdrawal 00
- 0x5bb826f8a40a75d18f4553c5c8b68df4b18ea0ac - Tornado Cash Withdrawal 00
- 0x93745f0a2886b5363408e6ec742a1eb9753a797a - Tornado Cash Withdrawal 00
- 0x723c2ca50994f079b6cc7bca869514060505399c - Tornado Cash Withdrawal 1
- 0x03dd0a157b2e43b31c829b5ed67b4e76542b4a7e - Tornado Cash Withdrawal 1
- 0xb2e684f6aa9be5379927feecfdcf8be818c68538 - Tornado Cash Withdrawal 1
- 0x38f5322799f8a94e1940488253b45979d6e6f215 - Tornado Cash Withdrawal 1
- 0x063d068797dc951ce231802ecb816da961656851 - Tornado Cash Withdrawal 1
- 0x98e7efd0407cfce0999578a67769a50d519c2ff9 - Tornado Cash Withdrawal 1
- 0x8e08628c4cfca575bd54c73eab4741ef214814e4 - Tornado Cash Withdrawal 1
- 0x55987d456afe204cd9bbc587f4dc5e35ebbdc95a - Tornado Cash Withdrawal 1
- 0x63c2578e35fad63e97076a6d93a256fc89846f98 - Tornado Cash Withdrawal 1
- 0x7854a2bfaaa0bf9c94015bc0d692a7bcfa9ce78a - Tornado Cash Withdrawal 1
- 0x37995c401c195466c5938426d5a1797798ab4063 - Tornado Cash Withdrawal 1
- 0xd1c4bb31251eb53bf4bfc2fde2b771a8406f2583 - Tornado Cash Withdrawal 1
- 0xa481f40f5ed36c2402de99faec5ed0a850f092ee - Tornado Cash Withdrawal 1
- 0x33c2cd1d1712e9b116a40b7a27cb63048aa377cc - Tornado Cash Withdrawal 1
- 0xd17e87688bfffe5417c86c65946380b30bc4f9ea - Tornado Cash Withdrawal 1
- 0x3d262da3227882db9bc6c303fbf0de63736e3252 - Tornado Cash Withdrawal 1
- 0xeddf1e3d7f080f44f889d6edf126d6c638cb8347 - Tornado Cash Withdrawal 1
- 0x7e76f45b1586c7f0d151e162c9ebcf6209a27eb5 - Tornado Cash Withdrawal 1
- 0xb7e2e4440ff429ce0458fec248b366c04a1629a1 - Tornado Cash Withdrawal 1
- 0xc327390a51e0314f1b61b9706035731a69dd5584 - Tornado Cash Withdrawal 1
- 0x420bd3424159396c9765331aaf3867a63e4a2a13 - Tornado Cash Withdrawal 1
- 0x6ed958235ace5fd5071699a6018e47b8b03a03ad - Tornado Cash Withdrawal 1
- 0x736cb15a26b3f4c4168cfad1aac387491a96370c - Tornado Cash Withdrawal 1
- 0xabe1b839834edcbdb863673a88dc0a0ee74fc1e4 - Tornado Cash Withdrawal 1
- 0x21d368ae3f39887af65a15d3aedd4235ed402b8a - Tornado Cash Withdrawal 1
- 0x8b14b1233516da49f391ce64fac6725506a06ae7 - Tornado Cash Withdrawal 1
- 0x065188749972e424bb48fc34626b668c38f09590 - Tornado Cash Withdrawal 1
- 0x114a763450df9426e1a16a43d7e6bd7d3c355149 - Tornado Cash Withdrawal 1
- 0xc83c3a7c335b53efa4994b5700c4cb4d12e4583e - Tornado Cash Withdrawal 1
- 0x6ac8ed3b80f10352804a361354dc2637e686aff2 - Tornado Cash Withdrawal 1
- 0xf6d93e14590c1aedd62b1df54a3db7d40ab40486 - Tornado Cash Withdrawal 1
- 0x6ad463fa0b5260b71a2e1f690757bb123d4fdf50 - Tornado Cash Withdrawal 1
- 0x75d9a9b87009508a4786655d2f57b0231e69db80 - Tornado Cash Withdrawal 1
- 0x5522ff1c89aa0c98130f75b14e564a1664f781b2 - Tornado Cash Withdrawal 1
- 0xcaaab92e972a6b1ef7d8838328be86cb0fe2c9d3 - Tornado Cash Withdrawal 1
- 0xfff456cd4d1b268fae7dd90dd4fc8cf6dbacdc51 - Tornado Cash Withdrawal 1
- 0xbda2f3556951434a754d3790da00ef14fb0c09e4 - Tornado Cash Withdrawal 1
- 0xdfaf096b7e84079791639a1aba19debf6f921448 - Tornado Cash Withdrawal 1
- 0x070460959b6e715f6ee83b5cb6341816a41f7e89 - Tornado Cash Withdrawal 1
- 0x7992395e84e8b3e099f90b113331ccbd6d9e3b8f - Tornado Cash Withdrawal 1
- 0x5acd02a81f47b2342c1ee7034981a3d0c65d216c - Tornado Cash Withdrawal 1
- 0x1f5875d6724bb0688415936c482388457aa0ed31 - Tornado Cash Withdrawal 1
- 0x9bb7f2bae2e466d72050cc6c92ef197510010218 - Tornado Cash Withdrawal 1
- 0x48be2e6802ee8070f075d3ab9588b7e076330548 - Tornado Cash Withdrawal 1
- 0x4393daf80347f9934e499f55658440dfced5f0dd - Tornado Cash Withdrawal 1
- 0xa41c73c86c2a378ebc934b9a32a1535bf45e49e7 - Tornado Cash Withdrawal 1
- 0x380a4458aa5c10de720ddfa641a135d64b078473 - Tornado Cash Withdrawal 1
- 0x5723930a322db18a18486ae11d8b398d52ec00a5 - Tornado Cash Withdrawal 1
- 0x2542766b393bad6fe929409553be2a5f58937575 - Tornado Cash Withdrawal 1
- 0x5f86de8e2fade60c52a6e7a2b950d709df2514c2 - Tornado Cash Withdrawal 2
- 0xf2df936ca1f2d54c75bfd88882c28614a0479fa6 - Tornado Cash Withdrawal 2
- 0x4948733611e4ae112549511bc9e9d588ff5eed37 - Tornado Cash Withdrawal 2
- 0x53c2c50f6a2b5045c7ac5445db514102c2319392 - Tornado Cash Withdrawal 2
- 0xc77cbd8780dbbe1ae352672cd664548bda58e58e - Tornado Cash Withdrawal 2
- 0x4cf1dc4d8b43d2d49b5b44531a49401f6aed558a - Tornado Cash Withdrawal 2
- 0xec0f8e7e2adeaa57b098070dea413b5919d6280e - Tornado Cash Withdrawal 2
- 0x17be94eff0eaadbcff1b301bb8aaee759ddb0263 - Tornado Cash Withdrawal 2
- 0x563e827b2d17bdaabb4ff1b1f7c0c09e3c0faf48 - Tornado Cash Withdrawal 2
- 0x9cd09c8a39a2d586a78ef39e38179686d3478887 - Tornado Cash Withdrawal 2
- 0x43b32303d28733ea1178249857c2db16edff40e3 - Tornado Cash Withdrawal 2
- 0xb6638549b0ab6fe68c5fd456ea5b7e2a7ab4f570 - Tornado Cash Withdrawal 2
- 0xbf0639a851683ec24e03208cd808bc4f236efab3 - Tornado Cash Withdrawal 2
- 0x66e9736d032c021f282cb037c3e2dfd404767ca7 - Tornado Cash Withdrawal 2
- 0x4e759c258eed410e23fbcbf40aa3f9a773870858 - Tornado Cash Withdrawal 2
- 0x3f1a3d41090f8cf9a4289dae958b194c4bd8346d - Tornado Cash Withdrawal 2
- 0xe82c488da2118fdbb1b0aedf1cb08838ec7bf234 - Tornado Cash Withdrawal 2
- 0x0470857ebe0a4d79e8f284a9303331e5c85707c3 - Tornado Cash Withdrawal 2
- 0x61e0c434eec3a47d9f303efdc87d41cf891b4b05 - Tornado Cash Withdrawal 2
- 0x649cf70786c6253f991446608e0430619156ad92 - Tornado Cash Withdrawal 2
- 0x157be205a78f29c34b179a39f97fe9418022132e - Tornado Cash Withdrawal 2
- 0xbe21ad235b3f322f1fe023f187052f95277d1c47 - Tornado Cash Withdrawal 2
- 0xa67024438a304371e7af0b27a0d7c68acaa88cc4 - Tornado Cash Withdrawal 2
- 0xfb3fa66705e55289b4367f4e9cba45d6e8674e39 - Tornado Cash Withdrawal 2
- 0x31346d24c48088830c4d940a6645cd69e3efe6f3 - Tornado Cash Withdrawal 2
- 0xa4e7e91cdf300150f36af7a04b85e37ad2ca9110 - Tornado Cash Withdrawal 2
- 0x909b6c962611120858149015d17c4adb2395982d - Tornado Cash Withdrawal 2
- 0x32c73d97b8ce9bd156943792fdf9c6d7c6e76c27 - Tornado Cash Withdrawal 2
- 0xd82a7d08bc380aead14fd39945e564625e19cc81 - Tornado Cash Withdrawal 2
- 0xcdd501569ccde58b837f48fc9b25e1b6cf67c3f2 - Tornado Cash Withdrawal 2
- 0xf56c522fb72241961569c199f3d2c6522b303dd9 - Tornado Cash Withdrawal 2
- 0x414fd5885970ba1aad0f8632bbfc4db9e3894808 - Tornado Cash Withdrawal 2
- 0x6250b473b9c2776b268af1cb0a2e57c1ff8693e9 - Tornado Cash Withdrawal 2
- 0x2ded09d2e7a545b1658807a97cd0f83be7c0a352 - Tornado Cash Withdrawal 2
- 0xc82a0bc8a4964c32a924e9cb1df94bdd13dcc40f - Tornado Cash Withdrawal 2
- 0xe4f1e2a69b6b1fa1e0bd7496def85150c5f38a12 - Tornado Cash Withdrawal 2
- 0xf21b1c45a198f50b78104ca32cecfa304811e841 - Tornado Cash Withdrawal 2
- 0x069a8676371b88133595b1f6776255d5aa1e7957 - Tornado Cash Withdrawal 2
- 0x01bfb487b7df3432ab8f67a043c795d27d9ca7ed - Tornado Cash Withdrawal 2
- 0xb1cc333eee1bbbbab5f53392b779880b0936655d - Tornado Cash Withdrawal 2
- 0xa7b8e3e226dbb65c8b05a573b86aa78b4e8bd0db - Tornado Cash Withdrawal 2
- 0x7eb429c93e3e96f483da88f4bca700118d3a566e - Tornado Cash Withdrawal 2
- 0x66f71f829bf87c4ee4a0682e13500678a28ea5fc - Tornado Cash Withdrawal 2
- 0x134b9566c99668d1a7bc1b51218e635bb52c7eb4 - Tornado Cash Withdrawal 2
- 0x133b283321c82a1c3a746054656d9c201f1db01f - Tornado Cash Withdrawal 2
- 0x165bf391596303c4af98405f60d18986b4840dd7 - Tornado Cash Withdrawal 2
- 0x3ec7c7b09ac1ab4b84bb06d43ef89106d4e1a267 - Tornado Cash Withdrawal 2
- 0xa366d651b70a6f0f6a3b60816136fc473e63bfeb - Tornado Cash Withdrawal 2
- 0x8343ce0e60fb3a33a2ec2921794c3248ce786a9d - Tornado Cash Withdrawal 2
- 0xcb852a10e3991b89777191213802c73be45c62c8 - Tornado Cash Withdrawal 2
- 0xd311677adee212b5463c130646735f81ccc48565 - Tornado Cash Withdrawal 3
- 0x931ba5bfaf484f099773e20f1a3945cee6867cb5 - Tornado Cash Withdrawal 3
- 0xbffd28e2a22a4ee0043a68098a97e10fef2bdeb0 - Tornado Cash Withdrawal 3
- 0x4b13c0f61f533a9f6321ce8917f702e178eeb561 - Tornado Cash Withdrawal 3
- 0xd4515815ea9dcf6bb74c759fdc1a19c337c00678 - Tornado Cash Withdrawal 3
- 0x32283fe3acfdb027ccde9d614c9e6a6b775d0c67 - Tornado Cash Withdrawal 3
- 0x93f1676e9cfe9a3a64e3317ce2f69c8723b72487 - Tornado Cash Withdrawal 3
- 0xd358f1e1dec7fb7b011c7c4ca59249200c3ae737 - Tornado Cash Withdrawal 3
- 0xe8dcd7c2be9dfd1c2a6b3e9e302ac682e6326426 - Tornado Cash Withdrawal 3
- 0xf15aa5931236daa5fc0266e123c068e663cebee7 - Tornado Cash Withdrawal 3
- 0xcb3157cf14182df30a7fcd15a4908eabbc3dd468 - Tornado Cash Withdrawal 3
- 0xb8a3badbb2319df7e6b5aa9893905354d17ca80f - Tornado Cash Withdrawal 3
- 0xb6388e990d50c3c032d8019bd8a90007e9a1a36a - Tornado Cash Withdrawal 3
- 0xbef2be04e025261242480100688147c984d2e74d - Tornado Cash Withdrawal 3
- 0x96693a48fcee6379007d3e1729c41e9f7117c690 - Tornado Cash Withdrawal 3
- 0x408aa9ee85f95c02bbb331a312d83cdefb00b9a1 - Tornado Cash Withdrawal 3
- 0x758f61d47c0da622f459f0d5b1ac365a9e8fa4ee - Tornado Cash Withdrawal 3
- 0x1553928f7b560d9387c125a4f926cd33783472d2 - Tornado Cash Withdrawal 3
- 0x90129d4d9113e479c11097c487a5f06e07374ba6 - Tornado Cash Withdrawal 3
- 0x4e7c398e241a1f60ec8d0258cdfa128335b6b2bc - Tornado Cash Withdrawal 3
- 0x9bbc58c80c06bd343d939ea62a60e1f479353abe - Tornado Cash Withdrawal 3
- 0x02a361d4e034d8b53312c2f0eb13fbf358f228eb - Tornado Cash Withdrawal 3
- 0xf00fe1bc2b2a0eb740d2becf9afe3b7c4699841c - Tornado Cash Withdrawal 3
- 0x864842becd6a98e01e02f848a063794b25d25ab8 - Tornado Cash Withdrawal 3
- 0x3272eb3446b9a8984aa8239c4b483a45741e32e6 - Tornado Cash Withdrawal 3
- 0x83f704875716ca84e5e395cd93eaef7fdd2661ec - Tornado Cash Withdrawal 3
- 0x04e5094ede06dc3476fb923c67969b9e3e18596e - Tornado Cash Withdrawal 3
- 0x8bc37ed3d8dcc016fc5950dc17e4589ada2b2e18 - Tornado Cash Withdrawal 3
- 0xfa1474ef330fe904502b896d30d22518f6b2b2a5 - Tornado Cash Withdrawal 3
- 0x9d9651cdd1356186f6b2972a50651f7b4fabdcbe - Tornado Cash Withdrawal 3
- 0x98361be002ec04d1427d9a96e5e7bd0d7524308c - Tornado Cash Withdrawal 3
- 0x5c95e7ea22d4abc75f583ba7dc1242145622e627 - Tornado Cash Withdrawal 3
- 0xc523978a0e55a996c86b6e5b7f517cf65dbecbab - Tornado Cash Withdrawal 3
- 0xfe3670c38a03be5b1c37a2c7025626311162e75b - Tornado Cash Withdrawal 3
- 0xb26d02c22317e564e1f6f8e1812c85671ac2d001 - Tornado Cash Withdrawal 3
- 0x450f630ac36182134de522c53ae939b4f1c4b944 - Tornado Cash Withdrawal 3
- 0xaded2074ab127161788a1462840a3c2b01197d82 - Tornado Cash Withdrawal 3
- 0x498ea5d733f7b90e7f3e7c4a48962a6ca552155f - Tornado Cash Withdrawal 3
- 0xdf23d1894f2a7060e7e7c55f46854c363f77e7f8 - Tornado Cash Withdrawal 3
- 0x931ead27ef05d66974053d805ed273bdc63028e2 - Tornado Cash Withdrawal 3
- 0x8157d31fd7381494da1497af4621b9ff8160cbd1 - Tornado Cash Withdrawal 3
- 0x98feb989a8f4f9aa1a3ad1907dae9097304d3196 - Tornado Cash Withdrawal 3
- 0xebfe3c5c6cc4167d85b56f155bc62b1ebd5951a7 - Tornado Cash Withdrawal 3
- 0x6611075126ccfd00904b3559e6bd371baaf5e649 - Tornado Cash Withdrawal 3
- 0x90970edfbc1e69261d9fdc22e57d1f522319cf78 - Tornado Cash Withdrawal 3
- 0xf916c0d2db4a71c71417d36a9c6b543d7a3a44ee - Tornado Cash Withdrawal 3
- 0x94ad34a0ae6cd4f9b84358b675e761398063c29d - Tornado Cash Withdrawal 3
- 0x00e653d217ef6fd11e7a17176ec755f8936ebc6c - Tornado Cash Withdrawal 3
- 0x879ecd03ae2859779c18ab5e6d7321542f14262f - Tornado Cash Withdrawal 3
- 0x91d07f4883708f109e6090729a1026d9d76f5d25 - Tornado Cash Withdrawal 3
- 0x7d89644f66c3afa7093045c84720141b0c997ec0 - Tornado Cash Withdrawal 4
- 0x1d4514c55683dcef92f5d876054b86a9a9782004 - Tornado Cash Withdrawal 4
- 0x4e379c0c094887c363c31cd98d427368bc667e40 - Tornado Cash Withdrawal 4
- 0x61af6e4169b31bd2702463cbdc9b3dcea8bc6b4e - Tornado Cash Withdrawal 4
- 0xfb3c5afed463534d25c7d6e08c72f7ad808a00b9 - Tornado Cash Withdrawal 4
- 0xcf26ab4cd9458a46e9d0c4b4267a61485ecfe6e8 - Tornado Cash Withdrawal 4
- 0x57e809d2e613afe36484f049721d8bdda23f045b - Tornado Cash Withdrawal 4
- 0x308b4996b14c79de23f70a1d26cd7c3bfa54c478 - Tornado Cash Withdrawal 4
- 0xef3c4fc0b0036090c75acd5be94176d002c1ef52 - Tornado Cash Withdrawal 4
- 0x585aef5668bfb37e2a38d3d2fed0efeefcdb8ebe - Tornado Cash Withdrawal 4
- 0x0a77efe1cd8923bbb01349974d3d7072c08a3142 - Tornado Cash Withdrawal 4
- 0x8449cf36c28c7bfc82f05e471c0c472505752025 - Tornado Cash Withdrawal 4
- 0x38fb97f8049cf178262febb0c116291e262fa55b - Tornado Cash Withdrawal 4
- 0x7b6837fa6bd52fb8502ab84765bfc38e2b53e2e2 - Tornado Cash Withdrawal 4
- 0x04fc58dade16f459a79da6095e37970c708c3ecb - Tornado Cash Withdrawal 4
- 0xe17a6287f8c04734ed8fc3f504300c44168f11ab - Tornado Cash Withdrawal 4
- 0x9f027cfc838cf895a5ec9c91fcb90930910db613 - Tornado Cash Withdrawal 4
- 0xc34c05b0847291536b78cf4905d38b82d08be4d0 - Tornado Cash Withdrawal 4
- 0xaff59f83ac1a70d68ff4f0b5e92a3b1d7d6c341b - Tornado Cash Withdrawal 4
- 0x045f9b38337c102163712d128a444a0d11363bf2 - Tornado Cash Withdrawal 4
- 0xf3bd33da885892ee67b0af4a80f59286b48a5ee6 - Tornado Cash Withdrawal 4
- 0x1efd569bd88b083f144e0f02333e18ded2d9950e - Tornado Cash Withdrawal 4
- 0x8d5be3f6d41f56e6c2e39c9420f1736de9ca91d6 - Tornado Cash Withdrawal 4
- 0x801c44fb116c4ee476c5d6a7f041dcdd581dbc0f - Tornado Cash Withdrawal 4
- 0xa8a83da7852195b933f89570a4ac8e4726ba8255 - Tornado Cash Withdrawal 4
- 0x9067dfbd5641ff48cbec2ff7f95bc521ba214d55 - Tornado Cash Withdrawal 4
- 0x22bc4428c3437babdf0c4cdd60b5ed6a161c4f0e - Tornado Cash Withdrawal 4
- 0x3607fb35f46adc43119eb7ef94681d0cdb07c4cc - Tornado Cash Withdrawal 4
- 0xb942750bc00aa9266812a1582321017f45d033b2 - Tornado Cash Withdrawal 4
- 0x8b1970558a1d7970e69eb5fbcfb977e9b6c0944f - Tornado Cash Withdrawal 4
- 0x81eb54d4526f4eeedd96899a0f88e16bcaa6d037 - Tornado Cash Withdrawal 4
- 0x08af33a05596ea07763cd358cb51b99e54baeaf3 - Tornado Cash Withdrawal 4
- 0x820b6f9130576491bf88256bc141b759294c5fba - Tornado Cash Withdrawal 4
- 0xc42b10b808a25f002bba1dd385bb3430b53aa2c0 - Tornado Cash Withdrawal 4
- 0x8fc5c8147b8db102c4063484ff85e19b5c0cb90b - Tornado Cash Withdrawal 4
- 0x496a2c91dcd2ab1222b0fffc65886595e579ea25 - Tornado Cash Withdrawal 4
- 0x5e7acd7b878383ef6bd17c17a776e5e6ccf625c7 - Tornado Cash Withdrawal 4
- 0xed0dc7eb3e9ff019bf18a5edfbafd4a832a73c53 - Tornado Cash Withdrawal 4
- 0x81c568ccb3d9ef50c2d297e4c5fde77b4893508b - Tornado Cash Withdrawal 4
- 0xfc9d1072c1f7108084a8a9b19176e316166f38da - Tornado Cash Withdrawal 4
- 0xdb5c146441f08603ac3a15b5021b3bc6af32cea6 - Tornado Cash Withdrawal 4
- 0xe106243e6b6c611e3b3f7a83065ecb8614b09349 - Tornado Cash Withdrawal 4
- 0x04f859e6a721ef55170617532158d6db2f2d07a5 - Tornado Cash Withdrawal 4
- 0xe844b155758bdaf18bf7d55118a4326c44da27d3 - Tornado Cash Withdrawal 4
- 0xce94da88537c8120a43eab2836ce45a14642a298 - Tornado Cash Withdrawal 4
- 0xd5dfb12a0bf09f745cc7d7df59516bf45b3f594b - Tornado Cash Withdrawal 4
- 0xcb887e43ac29036e4ff25027dac01d26ea9549e8 - Tornado Cash Withdrawal 4
- 0x65dc7e985d1db21a24fdca13e61253b8f12a5b9f - Tornado Cash Withdrawal 4
- 0xabd720fd844120cc7be804947a0b427e09f658c4 - Tornado Cash Withdrawal 4
- 0x92c627005058e67b5c84e17f4566dc9118edb689 - Tornado Cash Withdrawal 4
- 0x373a81edeac09d8347474f8b4a874865760ddbf8 - Tornado Cash Withdrawal 5
- 0x393be1c8e7a78cdd8b4ffd755d86ca515a00982f - Tornado Cash Withdrawal 5
- 0x4594651bd2180a63b04174748f83870f56401b88 - Tornado Cash Withdrawal 5
- 0xd80e62a5e9bd58777a7c8b841e5bfc40ee8a4ff9 - Tornado Cash Withdrawal 5
- 0xc09a15894123249ec0af1e43509cfe61b13b368d - Tornado Cash Withdrawal 5
- 0xfa7011e60f6cfb30ac048e2b261c0b9125e2bd10 - Tornado Cash Withdrawal 5
- 0x342b47ab0c5b3544ddf1e735a401165b25263b6f - Tornado Cash Withdrawal 5
- 0x91356bfc9d08471f356891f23143707cf32343f5 - Tornado Cash Withdrawal 5
- 0xee5343f52af4858e527c9a9ad85577c17f3836cb - Tornado Cash Withdrawal 5
- 0x507e0e33fe23b7aae348a1f89bb08709062a5b41 - Tornado Cash Withdrawal 5
- 0xcff1760c7b9be9ecddb1248578257a7b01efda28 - Tornado Cash Withdrawal 5
- 0xe05ebaeb153d8cacc68631f05adee863fc9666f9 - Tornado Cash Withdrawal 5
- 0xa4aa0734701fb1b5933bc2fceb72b98b23e235f0 - Tornado Cash Withdrawal 5
- 0xb02de56c50ecd3278c4c79d1b67bb4292a22f4b9 - Tornado Cash Withdrawal 5
- 0x51832b7b9e67ba5e2c8b39a71bd20e5d02e651d8 - Tornado Cash Withdrawal 5
- 0x075da34c1d1ef8b5f96a93ddb3af57e7308173ae - Tornado Cash Withdrawal 5
- 0xa5e31f435b60867fcdbce0d408eacee712229d00 - Tornado Cash Withdrawal 5
- 0x7c6fe09dd97014e0eed923ea843474b6cc6b9257 - Tornado Cash Withdrawal 5
- 0x66270c3aa1fcfaca8f033d3650c6255ac57c27a4 - Tornado Cash Withdrawal 5
- 0x9de9a3d51793ffc4f7c8d5adf5a82ec178dc439e - Tornado Cash Withdrawal 5
- 0x24b96753285e10883ae9b535b7fe71c59e7e8432 - Tornado Cash Withdrawal 5
- 0x9810698b1df6fee775bafcc41933b929b12f5c9d - Tornado Cash Withdrawal 5
- 0x5a80391059227f2bae6b4d3f1b37b6c399365646 - Tornado Cash Withdrawal 5
- 0x326742755592c8f16f37a8d0c65f91b208cd4082 - Tornado Cash Withdrawal 5
- 0x55a58d2ad3ace022659112c3abe3cb7ddde494cb - Tornado Cash Withdrawal 5
- 0x61e1b1d5af712a6a0b49ad56d873b0d6423c9c3b - Tornado Cash Withdrawal 5
- 0x147067734eb5f7d22692e5bd89111f4a9f8283d0 - Tornado Cash Withdrawal 5
- 0x8ae40b93515a30c701dce8ad40f314564612beb6 - Tornado Cash Withdrawal 5
- 0xeb003fba831b2bc58d5cbbb8255e968b9f4a04b1 - Tornado Cash Withdrawal 5
- 0x4dc94da4aa71e7f18e277da064c53ded4dd3a45a - Tornado Cash Withdrawal 5
- 0x53cd07a23ea9d20d3f08f00629a21d4be105e29f - Tornado Cash Withdrawal 5
- 0x38323914d2fcbe39bcf4ed6ecfe78dd7a7292f47 - Tornado Cash Withdrawal 5
- 0xd43e7a3b044120099b8f6a56080c2357530d5ef6 - Tornado Cash Withdrawal 5
- 0x6c76af0c792836cc403d3112c177f02555b7ac7f - Tornado Cash Withdrawal 5
- 0xb252d1ff818d44fa8ccd2c0351ab01486c6aaaa9 - Tornado Cash Withdrawal 5
- 0xd077b17656ff8a9abcb75ba0968fb8e68ddc277c - Tornado Cash Withdrawal 5
- 0x277a53f0184aee437c335e0e0464b971c1dcc4b0 - Tornado Cash Withdrawal 5
- 0xebf9b55a95e9062572d79e273cc6adfc417279d0 - Tornado Cash Withdrawal 5
- 0xca011ac352065e289814475984ae50f6e7ede448 - Tornado Cash Withdrawal 5
- 0x05c549ea65dedb7985fd6e57c6ede20d7a18a038 - Tornado Cash Withdrawal 5
- 0xf66541f80835a066be142541fcc02e22700d16f6 - Tornado Cash Withdrawal 5
- 0xe571382adbd879ebe7949a0c0b8825a77c878ea3 - Tornado Cash Withdrawal 5
- 0xe54d59fd8281188c1f2d8ab2fa32356c5f761647 - Tornado Cash Withdrawal 5
- 0x6f99078979cc76dd46688ecf2cae997229556270 - Tornado Cash Withdrawal 5
- 0x6f8bf5dfe70aab0517d3eabab2837959c01bd9ab - Tornado Cash Withdrawal 5
- 0x8ea83b39c0417b8df95eafd450328787c946e45c - Tornado Cash Withdrawal 5
- 0xf0ec5da5dbfccaa70f6038bbedcb8659fdac064e - Tornado Cash Withdrawal 5
- 0x93d08b5b460a4b1c5d93a398f2ddf7c49fa4c48a - Tornado Cash Withdrawal 5
- 0x74416176c40889843545c6b420806ad4a4630768 - Tornado Cash Withdrawal 5
- 0x4a8c5e0c0b5246f7b1a2cc631c1b9aa2f1803a92 - Tornado Cash Withdrawal 5
- 0xfcba540b44d2046fd93b52ba95df0254d831bcf3 - Tornado Cash Withdrawal 6
- 0x8f40ebb782ac0af5c14ee550f276f5d10c637a02 - Tornado Cash Withdrawal 6
- 0xb1e3f0548ca5e7ae479d244e90aa6bdf25bdcd7f - Tornado Cash Withdrawal 6
- 0x330945b6e906bcd745e43ef9566064f2a7b2b0a2 - Tornado Cash Withdrawal 6
- 0x3c08442f3934e4081e5a0f747e9cc5a0ecd99641 - Tornado Cash Withdrawal 6
- 0xdbc7f26b2cf2cc66fe5936b93f1a262b15b8b56d - Tornado Cash Withdrawal 6
- 0xe26d6144dddf5d3194d250c89e179b8645bc9bf3 - Tornado Cash Withdrawal 6
- 0xb774b05040c8550abecb0aa851581ae2e8ebf33d - Tornado Cash Withdrawal 6
- 0x0591a528c173330c2a63a895c6118d6427cfccd5 - Tornado Cash Withdrawal 6
- 0xba9fc7c5b027331c6b8ffec7a2175a174789a585 - Tornado Cash Withdrawal 6
- 0xacb5f58d31686acc720641038f0668ef54665f0f - Tornado Cash Withdrawal 6
- 0x49ad6478d3be0670679048d74e311e0edf9a96c8 - Tornado Cash Withdrawal 6
- 0x5aa975bb69133aa9a9757c84147718ed99d40c1e - Tornado Cash Withdrawal 6
- 0x2500fe47c0202bdd8ecb798fe075044c1869c358 - Tornado Cash Withdrawal 6
- 0xc52648f44610cfd2c3fefe0750479fb2d0ff7a6f - Tornado Cash Withdrawal 6
- 0x480ed3ad5055d63c2e67a8d5781901e01699d191 - Tornado Cash Withdrawal 6
- 0xc6f9fb51a425ab972b6f8eaaa49c35020e0d8f1a - Tornado Cash Withdrawal 6
- 0x13964b844edd0a8babcfc1db58c499bb9b11350b - Tornado Cash Withdrawal 6
- 0x632cd7c3aa127771881390e7ac907dd1de6b1b53 - Tornado Cash Withdrawal 6
- 0x0e019e1e3f6069d432b6fb0d4778c609fd4e824a - Tornado Cash Withdrawal 6
- 0x39c46a88a354de38e0015400dcd6ba5ef94231f5 - Tornado Cash Withdrawal 6
- 0x69b993d0c0ed2df55115fce77f5a55334a85c57f - Tornado Cash Withdrawal 6
- 0x0e19186c8a83e7d41f94d78f2057c264f23d46e4 - Tornado Cash Withdrawal 6
- 0x3f382d9c8421868135ca9c3e92aedcd337da21b1 - Tornado Cash Withdrawal 6
- 0xda39eaa3f2f51dcefa8978c9f5253ea5abe9aa4c - Tornado Cash Withdrawal 6
- 0xa3a6442eb2ecb3f921549a0879217652dd60189d - Tornado Cash Withdrawal 6
- 0x86c15f08c791374e951a3cba190bcafe4ae49c20 - Tornado Cash Withdrawal 6
- 0x7974b5749f0d7f8a8053f92ab95c47ca1ab34855 - Tornado Cash Withdrawal 6
- 0xa608a96ccc3164ddcbcbdcdb9a2d200a6a231711 - Tornado Cash Withdrawal 6
- 0x5dbc522ef80dbb7d4014d9b0c90fa80ed23223ba - Tornado Cash Withdrawal 6
- 0xdf105accecd919c74e57d53295731c661470b5e8 - Tornado Cash Withdrawal 6
- 0xbe7caef1c93b8fe91d73e1322c719fb8e47024df - Tornado Cash Withdrawal 6
- 0xf51328f279cd262d22ebc1ae267079f33f492635 - Tornado Cash Withdrawal 6
- 0x0a01cdd11659190d611b12e52ea3c31adf95e282 - Tornado Cash Withdrawal 6
- 0x305ecee08e168d082bd981d7638d689ea0784e78 - Tornado Cash Withdrawal 6
- 0xb522f4fe7c839a602b83c86336e521fae13765c8 - Tornado Cash Withdrawal 6
- 0x192cb0ea2b29c8e0a380eab3774fbfe96580b570 - Tornado Cash Withdrawal 6
- 0x8a6f2865f578ae4417251ebce17931acf6e7afc2 - Tornado Cash Withdrawal 6
- 0x8382f8e81295a45d513a40ecb628279dd822334c - Tornado Cash Withdrawal 6
- 0x201916690b8731ca39e7ad364690b18103d2ab87 - Tornado Cash Withdrawal 6
- 0x20649266a6370ab0a29cf04a561c9f739a8da37c - Tornado Cash Withdrawal 6
- 0xd9a561317c3a9934c72773c8164a297c995ae35d - Tornado Cash Withdrawal 6
- 0xe080aa8bd639e00b9fb8653db52867699b4780a0 - Tornado Cash Withdrawal 6
- 0x97326e4e9dc051d66c25759f4bc343bb8e1e2be4 - Tornado Cash Withdrawal 6
- 0x582803f2dde7459283352a48224ea6f11f07b4d4 - Tornado Cash Withdrawal 6
- 0x79ed1cdac2e340dd624de0ad1b9235fc7103dcbd - Tornado Cash Withdrawal 6
- 0x06810c99cdbcd0d3cc69d9bbfb84cf950e733514 - Tornado Cash Withdrawal 6
- 0xc84da11908e63e4f3a48227928374eff6eb8552d - Tornado Cash Withdrawal 6
- 0xb6394c3422fbc703a7c4f2bcb315d53d21228692 - Tornado Cash Withdrawal 6
- 0xcf571d132227c25d8afd6c887aa06fd730f39ebc - Tornado Cash Withdrawal 6
- 0xe5925eaec89d1574750ce5e7aa2dac4559bb2864 - Tornado Cash Withdrawal 7
- 0x052194f17aad2a46155b7b7f83354b94fe892339 - Tornado Cash Withdrawal 7
- 0x198d7e11ba4967144d509b8ab19026e3a79c452a - Tornado Cash Withdrawal 7
- 0xed36d96f5c4895ba0b013e3d1d5ec9c31a410db7 - Tornado Cash Withdrawal 7
- 0x9bfd4c868fee7ee982554079cf1d12de917e5425 - Tornado Cash Withdrawal 7
- 0xfd0986e106a1ef39c33e5c295c3d9a1234e4f653 - Tornado Cash Withdrawal 7
- 0xd89187f929a4e8081d23a71a25f3848c33340886 - Tornado Cash Withdrawal 7
- 0xee8b3d4fefb1b37e39af50c4cf036c1a8eecd45e - Tornado Cash Withdrawal 7
- 0x2692eb0b4b4a7d4f7df2e322819bbf5ca1ea0859 - Tornado Cash Withdrawal 7
- 0x81c288f2b53c26cf67249f2116df5187b1cb6b8e - Tornado Cash Withdrawal 7
- 0x4337d577f7a84ba51fc4ab7ca22327ef711d866d - Tornado Cash Withdrawal 7
- 0xe80fed7113af98390c5719e60009bfda40ee1566 - Tornado Cash Withdrawal 7
- 0xb93f02ce87168457893e4654ffce31f6d3247d87 - Tornado Cash Withdrawal 7
- 0x55aef76900daa727f45789bcfcab0504965dd28d - Tornado Cash Withdrawal 7
- 0x7f78d6d8a57fb3e9ae839b5010fa87e260fa759f - Tornado Cash Withdrawal 7
- 0xf3b14da38c165915bd4add9fcd206a7f07385744 - Tornado Cash Withdrawal 7
- 0x3177af4edd3c939f381cc29b4dea6ba73a99b73f - Tornado Cash Withdrawal 7
- 0xbb469e1d0e92bfe08aea69a1a5d54ba30e03276e - Tornado Cash Withdrawal 7
- 0x09de4ef5fe71f07ca2d7d570f29008a223ecd598 - Tornado Cash Withdrawal 7
- 0xd9f14535c9f27f98b9b988002df8e62d5d59ccd3 - Tornado Cash Withdrawal 7
- 0x5d62f617ff1418b9756eb736548771ed8b7a3516 - Tornado Cash Withdrawal 7
- 0x755f3b53346f81e5391467295ef4aa322e02cda4 - Tornado Cash Withdrawal 7
- 0x8ed2058166e3cb65131b2aeff889b641450b4f01 - Tornado Cash Withdrawal 7
- 0x60a152c0f0c2dd6068d588f42027352bee593ee8 - Tornado Cash Withdrawal 7
- 0x24601cc4295a5b0118426da0a2c3f5b5337e8d01 - Tornado Cash Withdrawal 7
- 0x98e3883eb455894eeddd29131765fded523aaa9d - Tornado Cash Withdrawal 7
- 0x6f3331f755575d7bece19dde014856bcdd6a9d3e - Tornado Cash Withdrawal 7
- 0x23455954f3728f9eb248891ed11f6d42e4f9cfc5 - Tornado Cash Withdrawal 7
- 0x7e80caaf9d8d2a0ad82e532184fdac0467d72eb1 - Tornado Cash Withdrawal 7
- 0x7dee98d6b875aab9f660797bef3cdcb620b0199f - Tornado Cash Withdrawal 7
- 0x1d98e0ffb6fb73e2d7952892d685ce440b53722c - Tornado Cash Withdrawal 7
- 0x7dcc98a165e34baee566c31127309711320e9211 - Tornado Cash Withdrawal 7
- 0x9b531a7fb45f6db89e17e025a33fa13a2965138b - Tornado Cash Withdrawal 7
- 0x1f6793b7cca4e057266259336443e8560f108540 - Tornado Cash Withdrawal 7
- 0x7cee5c109f93236109d0095325736ee8ddf675a0 - Tornado Cash Withdrawal 7
- 0xddc015433f64b35da01b411c452701894c469357 - Tornado Cash Withdrawal 7
- 0xd11612ecfd734713f150073b8f4313a6473feb7a - Tornado Cash Withdrawal 7
- 0x33de13ef77d603349ebd5c6ed7a41530ca5caf9b - Tornado Cash Withdrawal 7
- 0x2b404660164343b6a3e2cd94e6ebe112be06af2e - Tornado Cash Withdrawal 7
- 0xca85e50558e4319fc861a6a0c3220f5015f2789c - Tornado Cash Withdrawal 7
- 0x9698f51bc5e96f2a8e05422388555aeade76c845 - Tornado Cash Withdrawal 7
- 0xb6a580f1cc72ec9ef1c104211092e086940e934f - Tornado Cash Withdrawal 7
- 0xac4d1ef28faaca846eb078fc3b59a73a624a67d6 - Tornado Cash Withdrawal 7
- 0x01a9111cc503b9977ef2c888d956beb48a249a20 - Tornado Cash Withdrawal 7
- 0xfe0ce8d939e510eaed46366671920221c71771a2 - Tornado Cash Withdrawal 7
- 0xc2738e31660c9a9b6ac456659a20f86ea77d2058 - Tornado Cash Withdrawal 7
- 0x7b5fdbbf731f3cd80a1ef0327a203dbbd4d6e0ef - Tornado Cash Withdrawal 7
- 0xc1ac5d46ef4fb6cf926ce1590f9a8f537f9c8943 - Tornado Cash Withdrawal 7
- 0xb218dbb8287900fa819490fb8952a1f742271cfe - Tornado Cash Withdrawal 7
- 0x804e31705491770ebc476d4b0599df255d5eb15e - Tornado Cash Withdrawal 7
- 0x3caf269caf892d0b81d560443f4192e7710dfbfd - Tornado Cash Withdrawal 8
- 0x140621b4079aa885439d3066a1defc833820566a - Tornado Cash Withdrawal 8
- 0x3bfd2395d08094fd9e3d87d0c2578599dfd3e8d1 - Tornado Cash Withdrawal 8
- 0x1e54c84e5a12de8815f5307eeec63f68b0a66350 - Tornado Cash Withdrawal 8
- 0x093dc10027ec09c32f7f5f623bbd3c9d26d27db8 - Tornado Cash Withdrawal 8
- 0x2cd8d674db9c2b5ca2adbdb64bf9c765de052b6c - Tornado Cash Withdrawal 8
- 0x21c30e720e38bd59610c19ed3f481be01b69fa9e - Tornado Cash Withdrawal 8
- 0x809177fcea7c594ed4861b7e4d9c6cc07e38ddff - Tornado Cash Withdrawal 8
- 0x5b275de98b075a08dbeb09dd41040f52708709be - Tornado Cash Withdrawal 8
- 0xb55ed1f3387f6316891bcefee38cd60ba213a8cd - Tornado Cash Withdrawal 8
- 0x1a6454cc345371d834bb8142dbb2a026241f912b - Tornado Cash Withdrawal 8
- 0xbb41814c0d922cb7f12231ede83c0d4db0168494 - Tornado Cash Withdrawal 8
- 0x63b38190b4803df5e579ae5b1b5e1f7189cc104e - Tornado Cash Withdrawal 8
- 0xf19eb318b7dd12d3f6fc0ac4a11429c618435159 - Tornado Cash Withdrawal 8
- 0xf67448b7d0aa69e147d8b2b4c690cbade513d8cf - Tornado Cash Withdrawal 8
- 0x371561f6f7b80a41f83d7c84dad3fc16520cdece - Tornado Cash Withdrawal 8
- 0x57ba188567258f1eec8144e570588adfbe7bc5ad - Tornado Cash Withdrawal 8
- 0xdfb64afa632fae3392d81951f1a603c78630c379 - Tornado Cash Withdrawal 8
- 0xcea1ae20785a063d80112dccea50b80ebef55a28 - Tornado Cash Withdrawal 8
- 0x64e52498ed84e03b1c1963df9a40ec3ddb44fd8f - Tornado Cash Withdrawal 8
- 0xd531bad2230ba08bd2e323d9c1c50a5bdc5f8d38 - Tornado Cash Withdrawal 8
- 0xd5d886b595f7cfc22fb13590a8455b338a21e43c - Tornado Cash Withdrawal 8
- 0xd9fde6f6dfb17e8b91cdffbfe650e6708b86e2ed - Tornado Cash Withdrawal 8
- 0x5081ff1818f6465ec9c735a8df9bee6d25dd76a4 - Tornado Cash Withdrawal 8
- 0x528ddc867c07dbc2be7300b9980a8a8cc72f9891 - Tornado Cash Withdrawal 8
- 0x48bbef7bab92fcba7dc37c6be4241e2eeafffcae - Tornado Cash Withdrawal 8
- 0xf0321d6a59629966c09ac928e21fd47dd5ae02f2 - Tornado Cash Withdrawal 8
- 0x9109e567c2086905e0cd1f90b52110ba61966466 - Tornado Cash Withdrawal 8
- 0xa3cf6ed0fac70d5677dae39c8ded07d07f88092c - Tornado Cash Withdrawal 8
- 0x7bbdd090c86852345677966febe3d02897a816ef - Tornado Cash Withdrawal 8
- 0x0bae9ff6d2d5561ea6a996b28171e5d41217c079 - Tornado Cash Withdrawal 8
- 0x3f536024012c43aed4434f58a0ef02f54a32c630 - Tornado Cash Withdrawal 8
- 0x299d9d57da813ed506e51369652682bcc4d02010 - Tornado Cash Withdrawal 8
- 0xc8186f97d54e4235401a5a515ef2b6be770ea8a7 - Tornado Cash Withdrawal 8
- 0x475dc1adf826bff32f2b98bf872bfc753e005da8 - Tornado Cash Withdrawal 8
- 0x9b738e7df48cfb3ea663bdc4af764929092e4b6b - Tornado Cash Withdrawal 8
- 0x5840cd76591a7f70c5b6530a8f288dbe094f6fb5 - Tornado Cash Withdrawal 8
- 0x49c41326f8d58cb86ca2dc867c2ee734c29c3419 - Tornado Cash Withdrawal 8
- 0x3874e1502c70c854b376f1b717a047c9b45dba33 - Tornado Cash Withdrawal 8
- 0x5e9e1992293db05cd808d6bcb28f5113bec23cc9 - Tornado Cash Withdrawal 8
- 0xf4622847e1248a6c8d756a6d90cea6dbaf69e16c - Tornado Cash Withdrawal 8
- 0x188a7c5438173eb590671030c234654cdbcc977e - Tornado Cash Withdrawal 8
- 0xe7bebe50df652c90473972494dad4c96d0a1677d - Tornado Cash Withdrawal 8
- 0x77b3ccc6890f6b0709ee6c5e19c929c24482bde9 - Tornado Cash Withdrawal 8
- 0x49cdf54a304029407b33a74f9206b4abc55f77d3 - Tornado Cash Withdrawal 8
- 0xae550ad745f4058b33a95421e69fcb6d24d8c611 - Tornado Cash Withdrawal 8
- 0x7135492489ea081b6cbd1b273c8a1d949d337817 - Tornado Cash Withdrawal 8
- 0xa4f643040c4f757d83be3f27dc0ddf14c9898db2 - Tornado Cash Withdrawal 8
- 0xae7524e04516e3b0900060db1cccecf76d85fdb4 - Tornado Cash Withdrawal 8
- 0x213ec646d47c0151458ae50b0895ebdc1558a864 - Tornado Cash Withdrawal 8
- 0xbd9956ecd8c100a629c04ab6534eb810f2adf2a6 - Tornado Cash Withdrawal 9
- 0x36fde9ef1a086200bb4c7669c51a872e2570c94e - Tornado Cash Withdrawal 9
- 0x7311c79eae80fff2b55a506e75f8eff5a9657f70 - Tornado Cash Withdrawal 9
- 0x4cf9fb0f68c9876f0cf511c7910c2f341adef3d8 - Tornado Cash Withdrawal 9
- 0x8e25394b0432c601a8331dee3652baf010087a85 - Tornado Cash Withdrawal 9
- 0x60adf001e3822b716ff7730b7f0bb0b9c603ec0b - Tornado Cash Withdrawal 9
- 0x262f3cbd538d8049ffa883288fc8c2fc389ab9c0 - Tornado Cash Withdrawal 9
- 0xf2418f690295f037c02bf8494e7f7d727f281351 - Tornado Cash Withdrawal 9
- 0x2f0590feece9c54a93e426fa44ac44a4315252c7 - Tornado Cash Withdrawal 9
- 0x189df6bf06c7aef516d8adba4d768b065ceae975 - Tornado Cash Withdrawal 9
- 0x1dbf60490fd92c5c8e0927699ab2f1dcbf239a35 - Tornado Cash Withdrawal 9
- 0x87ca81866e5e1fbe05539d8ae90c0c97ad41bd7d - Tornado Cash Withdrawal 9
- 0xf23ba00ab73911d0eb23af6573fdb5242ea2ed41 - Tornado Cash Withdrawal 9
- 0x3c8f00f786b590b8b7f5fa11e5832580664e7e71 - Tornado Cash Withdrawal 9
- 0xff0e869e2898162cd4b62a925ecec519ceb33a25 - Tornado Cash Withdrawal 9
- 0xc3ef0f9b14da0d482c19d5c1812f6584312e5d37 - Tornado Cash Withdrawal 9
- 0x2dbb4b05c3185b37822f498778c4abf56408352a - Tornado Cash Withdrawal 9
- 0x8ac194df73369e6162e51333407f0772d85a5b38 - Tornado Cash Withdrawal 9
- 0x05add1149adec8fc69c4cbc759b7e18b467f99b4 - Tornado Cash Withdrawal 9
- 0xa56647bb211ba3700c1ad3c904deff606f538bb7 - Tornado Cash Withdrawal 9
- 0xa9fa667753ed39cf79fa1faba3cc80d282fc1a14 - Tornado Cash Withdrawal 9
- 0x89a026676cae9bd60783cab2f47a0f9a5d9abfd6 - Tornado Cash Withdrawal 9
- 0x920857caee0a46a32788a95510786a35904998b9 - Tornado Cash Withdrawal 9
- 0x2448593024a07db74d35268f0089e8e61308a2d8 - Tornado Cash Withdrawal 9
- 0x1d724024c1028b63f2a45eab549473d7adfef3e5 - Tornado Cash Withdrawal 9
- 0xaae94af8d265a94daa12c6c320953a0cff45619b - Tornado Cash Withdrawal 9
- 0x6b5026f6970525de2d1e085b6fdf876f90810eff - Tornado Cash Withdrawal 9
- 0xc5f7506ea9f278b1c6b30572840128ab8bc6a71c - Tornado Cash Withdrawal 9
- 0x3d24cb1850ec031c441dbf827b2d2277d25ca0b6 - Tornado Cash Withdrawal 9
- 0xed2148c2df469b82272486bea90ccbd9011999de - Tornado Cash Withdrawal 9
- 0xd64b98a4fe51eff365327677489ed02a26174e9a - Tornado Cash Withdrawal 9
- 0x6639f5a45219213aa07d1a0c53de146c89a4a665 - Tornado Cash Withdrawal 9
- 0xb79a9a764c91556c09747c0c921065789e13be30 - Tornado Cash Withdrawal 9
- 0x0a8fe8a70084a4fa9d79864e280782bdee747b6e - Tornado Cash Withdrawal 9
- 0x41d45bc8ecee219a311bbfada151936a2d7c42ad - Tornado Cash Withdrawal 9
- 0xc874d0dfcf49681b59f6354eb03cba0efe80ada0 - Tornado Cash Withdrawal 9
- 0x20910d3fb697c38d239b0c40b9f97b71abaf8168 - Tornado Cash Withdrawal 9
- 0x28ae8eac20a64812a37c2aae676ac4f2b515ebf0 - Tornado Cash Withdrawal 9
- 0x8cd57fdd589d5f69f846dabcbd3dd3e83c95a9eb - Tornado Cash Withdrawal 9
- 0x3fa4028eb2b652054a33f2aaaa00d69869df5a22 - Tornado Cash Withdrawal 9
- 0x29d410d53e175571fe2b44ca982c5fca1bf53bbb - Tornado Cash Withdrawal 9
- 0x808983a6053430264cb021e8c61d1936ac217dca - Tornado Cash Withdrawal 9
- 0xf061e98aa21e09b2a6897fbb038d7944c44f91b9 - Tornado Cash Withdrawal 9
- 0xb1e676ea71dbcf24ad55ed6033cd0ed4763da6e9 - Tornado Cash Withdrawal 9
- 0x0f308a6ec7cfefaaa2d580b356b10a42073510be - Tornado Cash Withdrawal 9
- 0xb05835dd07d6102d4ef9df394565913b430a0036 - Tornado Cash Withdrawal 9
- 0x24ace3669d0e80ff6dd285fdf0607c7826afa080 - Tornado Cash Withdrawal 9
- 0x433df4642b2b70a71e38c7b0192c5084fb7b9146 - Tornado Cash Withdrawal 9
- 0x6588a50d2cd3e85493fda84bdaeda8392bf4bbdd - Tornado Cash Withdrawal 9
- 0xad0649a1a261af5c563eb60177ccc35abd5aa7a7 - Tornado Cash Withdrawal 9
- 0xe800ff8c971445ef4b5663fa61896c38b9517a43 - Tornado Cash Withdrawal 10
- 0xede0848696562031276d8bb06c50ba93099ef9eb - Tornado Cash Withdrawal 10
- 0x7c490b9fa060794e72eb28a641e6b28f6b0833e7 - Tornado Cash Withdrawal 10
- 0x582bee47f206dd40c0b2bec7692a8298c984292b - Tornado Cash Withdrawal 10
- 0x510e4e37b3157ea21ba66716df9a8e58e5322506 - Tornado Cash Withdrawal 10
- 0x36a021d8070e8e9c3e7871e9b41c9401ff09e0fb - Tornado Cash Withdrawal 10
- 0xf0fa6d87b11af18e4271f0351930c650cb2553b1 - Tornado Cash Withdrawal 10
- 0x22706c466a5affe2567b271af8911589743da3f8 - Tornado Cash Withdrawal 10
- 0x0ca475ab67aec2aed2815ac8ec5f9df0156b5ebf - Tornado Cash Withdrawal 10
- 0x2312104c95a7766dde5f16c7ca770ce26dd676a5 - Tornado Cash Withdrawal 10
- 0x9db64d79710bfb249e60c805cdc9db694caaa1ff - Tornado Cash Withdrawal 10
- 0x2efad3a39b6a0ca3fe381ab4b96cf5201d26446d - Tornado Cash Withdrawal 10
- 0x3d9896da34ddc36ce6cccff511c73ab409d18684 - Tornado Cash Withdrawal 10
- 0xe0961d49d95921885e4b0346fa805281f81c21e9 - Tornado Cash Withdrawal 10
- 0x12459e10b62213e6b64a56711aeca886d76205ac - Tornado Cash Withdrawal 10
- 0xa2c8594275d867c1c06438afe8504067426819ee - Tornado Cash Withdrawal 10
- 0x5117acf41f16ab23ba2e5d35c1da4169589aaee9 - Tornado Cash Withdrawal 10
- 0xd3b589b60d7c15b23b4f97985027100a0777ac40 - Tornado Cash Withdrawal 10
- 0xf8690551a5b0e698f1535038e4455b6e94068496 - Tornado Cash Withdrawal 10
- 0x3c39da0453d490f9403ffe1899527af904a07b1e - Tornado Cash Withdrawal 10
- 0xd378fc5de3c23032b0c353145e888ab80cf2316e - Tornado Cash Withdrawal 10
- 0x7a1aca1ebcb35f430172cc6d0e8b1755195e95e5 - Tornado Cash Withdrawal 10
- 0x5ded64f62b1e8ddc96ff8ebefeb179cb97738ff9 - Tornado Cash Withdrawal 10
- 0xb4cfed28714ee1f45ebafabaff6c4fbff447bc45 - Tornado Cash Withdrawal 10
- 0xcefa3cf1b578a04625d55e6534cb196392e1e115 - Tornado Cash Withdrawal 10
- 0x48f0de984f129d471c4537733654f0b63a7866b2 - Tornado Cash Withdrawal 10
- 0x3c552fda4043cfe6b650da2ab87cf1cadcfcaf25 - Tornado Cash Withdrawal 10
- 0xdee87eb4bcf6ddbb7dc220ecabaad8a174141779 - Tornado Cash Withdrawal 10
- 0x06dc27afdf50f2e0f0c3eff401fc3f92c75b76c2 - Tornado Cash Withdrawal 10
- 0x14205149859f7bc79b63ef6a7d9d686ca2c7f4f4 - Tornado Cash Withdrawal 10
- 0x02d8bf47c3672a0295959e8001370d405383bf9d - Tornado Cash Withdrawal 10
- 0x12f26d82e4df3b13e1296ad7ac937cfa127e15e3 - Tornado Cash Withdrawal 10
- 0x8fbb5cea0372c67b95170ebc600aa64b61238b48 - Tornado Cash Withdrawal 10
- 0x49500d2a43a9d4b617f31686b1adb474af36c084 - Tornado Cash Withdrawal 10
- 0xb9c18c6361a7e547fddbf3f6ddddfbdef92b24dc - Tornado Cash Withdrawal 10
- 0x9cdad13015d904be748eee5124f4efbfd8f80434 - Tornado Cash Withdrawal 10
- 0x7a315d08db044d168e5e497693508c25e7703dd5 - Tornado Cash Withdrawal 10
- 0x8787801655d756e964823ed25373a0b83970599d - Tornado Cash Withdrawal 10
- 0xaa7f4b46b6c1d715dd14c4ac38d4d52a309620e4 - Tornado Cash Withdrawal 10
- 0x24c5e04228303ea246aa894745b30a90cf99bb35 - Tornado Cash Withdrawal 10
- 0x287f76bc7d9ba622a4b591fd84996a40f0bfb680 - Tornado Cash Withdrawal 10
- 0xc67565e798996d2973acee042314d0d436b84ebe - Tornado Cash Withdrawal 10
- 0xe4a7d2a1c7db94b59c59a9f913d89152a0cc2c54 - Tornado Cash Withdrawal 10
- 0x724eee940a4e428681b22e3468c5c1b9eb69f5b3 - Tornado Cash Withdrawal 10
- 0x0b456989f0bc29ff2ae3dd9af034832e2af6f94d - Tornado Cash Withdrawal 10
- 0x74335834bfa93d349448456c61526f7a1dc3659c - Tornado Cash Withdrawal 10
- 0x5526cc24c96ac3886e825b975058bcbaefb3729a - Tornado Cash Withdrawal 10
- 0xb77e94e2eaf04a5031f7a2973d464c641142a36f - Tornado Cash Withdrawal 10
- 0x460ead15e7312068ddd3440017b0e5b6fcc9d2f0 - Tornado Cash Withdrawal 10
- 0xeb278aab90169dca373b2daaad5d9efaf68e295c - Tornado Cash Withdrawal 10
- 0x65c2ac2f177206c77f66865adfb0c8b456bb97d1 - Tornado Cash Withdrawal 11
- 0x3ef060fecac4114d50fecd35ae3523bdc1b3a42f - Tornado Cash Withdrawal 11
- 0x2aaf509194dd1ad0df98fda25564a6fb7f01beb6 - Tornado Cash Withdrawal 12
- 0x8ac97d0f70c2b05cc03b617ec7fbb8b7dfd3c942 - Tornado Cash Withdrawal 12
- 0xf9d9aa61c2d571d7719445f8dabb4c5396ede553 - Tornado Cash Withdrawal 11
- 0xd797b5899247adc43aeb1dcad7cd0537eca98e1e - Tornado Cash Withdrawal 11
- 0xe9a5d423336e40799d0a71bbf13b21350d2096f2 - Tornado Cash Withdrawal 11
- 0x464c008378d6aa59fc3bb91548f2a752ac655c9a - Tornado Cash Withdrawal 11
- 0x694db03e67483126ec02121611d011d1779cb86a - Tornado Cash Withdrawal 11
- 0x1e2e521ba1b3b6da43db1e9fd5422b65a58719e8 - Tornado Cash Withdrawal 11
- 0x47bbe128eaa1888b6c07d3e48962b84a71b0fbc6 - Tornado Cash Withdrawal 11
- 0x73a846c95d1be7d4df9e13043daf0d8bd4a4ae38 - Tornado Cash Withdrawal 11
- 0x66d146526db1825e2016e22b31f7251c78913186 - Tornado Cash Withdrawal 11
- 0x8c66a9809ff827f03f21bf1ea1224a519c712637 - Tornado Cash Withdrawal 11
- 0xa5d9fa0af2c5b1d30e40b8f2b15c7724dcf85e36 - Tornado Cash Withdrawal 11
- 0xff53661023fa4ba911936ea279359930dd30d706 - Tornado Cash Withdrawal 11
- 0xaf19922993f99554a794b459d6330646791ae47b - Tornado Cash Withdrawal 11
- 0x411f248995067668d51612178d59cc00f41b1279 - Tornado Cash Withdrawal 11
- 0x859abdedad55e5f3b5d0dc07e8383980c441adbc - Tornado Cash Withdrawal 11
- 0xb332f02e3387f0a7183bc99adc1af6eda2a15074 - Tornado Cash Withdrawal 11
- 0x83c71854d4e30a509562e09b3a08a00594426a2b - Tornado Cash Withdrawal 11
- 0x246eaa3a7b1bcf1cff5b9110775a75ab6034de82 - Tornado Cash Withdrawal 11
- 0xf123327bd6e44b0ab1f40f9199a9add4f0359a2c - Tornado Cash Withdrawal 11
- 0xf88cebfd97e9e14e434bb7ec35392b9b0d73de32 - Tornado Cash Withdrawal 11
- 0x01754991bb720282bd688e44f345da9e3df343c4 - Tornado Cash Withdrawal 11
- 0x9cca339f5b1655719128c47aa9cfd14b559d66ad - Tornado Cash Withdrawal 11
- 0x02e65d7ea7a1289d7506afb07d841da1d24983a8 - Tornado Cash Withdrawal 11
- 0xbd7f1a74a5a75c3cbcf62e522e318e81a3ceb0ab - Tornado Cash Withdrawal 11
- 0x415b9321cb864b6a018dcc746351827a2b1f4bda - Tornado Cash Withdrawal 11
- 0x59ac86395d1e0d44fd5a3e3d5eb76c3aa60ae01b - Tornado Cash Withdrawal 11
- 0x9af89040fbf01d64f2730877101297c8a37eeb14 - Tornado Cash Withdrawal 11
- 0x2d3390eda5436e95ceafd7dbff054f8a42481ef7 - Tornado Cash Withdrawal 11
- 0x05ffdea77f63865e960e5ced45178a616eeecfb6 - Tornado Cash Withdrawal 11
- 0x81142408bffc9f53bdc6b32c692db2612b6be477 - Tornado Cash Withdrawal 11
- 0x01edea2c477d054c2cc98addd3d30a06a49996cc - Tornado Cash Withdrawal 11
- 0x95843ee8b0b005ce83bd1fa1b9bc340a6b96a9c1 - Tornado Cash Withdrawal 11
- 0x605f47134f963018e72b43a055bb106a81e757a0 - Tornado Cash Withdrawal 11
- 0x77eddab8635e7f6d8add523793596df5cacf4944 - Tornado Cash Withdrawal 11
- 0x43f27f6de3d18a69cbee3f4bd1d5d0f1d0e53511 - Tornado Cash Withdrawal 11
- 0xfadf12f623deb0488b598479f33c1b768300e599 - Tornado Cash Withdrawal 11
- 0xfb14ada116ea07daaa134dbbd7dfbde33b1b8efa - Tornado Cash Withdrawal 11
- 0x6030e77eaec645cd96c2074e01aa8ae5c68abcdf - Tornado Cash Withdrawal 11
- 0xd057480a9f6abbaff0d7aa4335dbc65ae98df541 - Tornado Cash Withdrawal 11
- 0x5d267475586edfeeb81bef1ad3152c3b53512818 - Tornado Cash Withdrawal 11
- 0x221ae6a659e98d1253e7d693a8927a31f7c86bdd - Tornado Cash Withdrawal 11
- 0xe8c40f1cd3d3bc77f795945f8afeca62ddb076ff - Tornado Cash Withdrawal 11
- 0x006fdf9941ee8bdcaa1020ba83737b200dc083d2 - Tornado Cash Withdrawal 11
- 0x019fdc1e08172e332704599f5ed9f8c412047076 - Tornado Cash Withdrawal 11
- 0x910165b84f5062fbb3276e1aa0af501fd4657991 - Tornado Cash Withdrawal 11
- 0x32810b4551ff7bac9bb54469214fc57246af6e12 - Tornado Cash Withdrawal 11
- 0x493df6ff837a19215740139c7255a0ad5d006f7f - Tornado Cash Withdrawal 11
- 0x2d868a20da8b5e07f79184eccfe1aead35132dac - Tornado Cash Withdrawal 12
- 0x297ebb0d16928af1f80f9f0a5c0326ab3cfd509e - Tornado Cash Withdrawal 12
- 0xde46b18b295a783b010436cc8e2ba8bb3feea875 - Tornado Cash Withdrawal 12
- 0x472bb4e25ad8304345a12139866ed566e2c3e48f - Tornado Cash Withdrawal 12
- 0xdd1e1fb176e3aa266ec0cd73f1289a77ff642544 - Tornado Cash Withdrawal 12
- 0x3034723fd7151aee449e8166bbf61a7b1a62c3fd - Tornado Cash Withdrawal 12
- 0xaab5f9042d89ed0d9896ba89b9dc6cda3de3a27b - Tornado Cash Withdrawal 12
- 0xbd61efb21f9bc6c3b7b267ad5b39dcc4f9c2a823 - Tornado Cash Withdrawal 12
- 0xa4244f2f9e486f20d925336867cd95973152ecff - Tornado Cash Withdrawal 12
- 0xa917ddc3458964088f99dee861e43da7ed72584f - Tornado Cash Withdrawal 12
- 0xdf7af4e6c8e381780fdeb6e0cf70b4babe9be28d - Tornado Cash Withdrawal 12
- 0x93ca1dea6a6969fdb26d7611e674dec9ccdfe5a7 - Tornado Cash Withdrawal 12
- 0x38277a71e67a74898ef21306dc84390cfdfa8a45 - Tornado Cash Withdrawal 12
- 0xc41793bfc82ba230bae10ce9e4a8d13fc3272122 - Tornado Cash Withdrawal 12
- 0xecf637b2c5cb141e55c2ed63c51c20767664f4b3 - Tornado Cash Withdrawal 12
- 0x71eb2ef4a2916a442072177f91b7ef0bcf1b7f38 - Tornado Cash Withdrawal 12
- 0x18b431580b7a12a9cb898d9fa2fb5e76370a7e72 - Tornado Cash Withdrawal 12
- 0x2313b42888eddfffdf84e4bb38c647e466b7e4b6 - Tornado Cash Withdrawal 12
- 0xd6dde4491bf614d282d71fc7bdcefa7cee97e3f4 - Tornado Cash Withdrawal 12
- 0xbba5456403279295e7dea5e3683ea434997c5c21 - Tornado Cash Withdrawal 12
- 0x46a5f010497435ccfb5f0e0de5a3fbefa435630e - Tornado Cash Withdrawal 12
- 0xd7619b8e2538b0aae7e8d3b2a9087ea256801d0d - Tornado Cash Withdrawal 12
- 0x85e2f944349190a15af8eadc4f975406d1dc6a4b - Tornado Cash Withdrawal 12
- 0xe233de0c3b076bc463e1b19a4ee88666c87ac2f1 - Tornado Cash Withdrawal 12
- 0x96e5f679e8c324c8e2b710d2524bd5104ea75e06 - Tornado Cash Withdrawal 12
- 0x8920c2c8c1b4b97840fb3f7e5f2225c4fff28451 - Tornado Cash Withdrawal 12
- 0x42ac9dbf33d29506e84697a1092a8a9ec767e31c - Tornado Cash Withdrawal 12
- 0x10149d5d89d0d78d4b5b1bbfb8817b9e8e4067a0 - Tornado Cash Withdrawal 12
- 0xf25004359443c93465f9f1a6601151bfd7af6adf - Tornado Cash Withdrawal 12
- 0x16ee72d6e7c34d9e1644b3273416a96fac87c6bb - Tornado Cash Withdrawal 12
- 0x8d1fecebb93c735eee9fc06b0cd227c7508bf797 - Tornado Cash Withdrawal 12
- 0x993e97026b39ae1e1f7d297cd1160d6cfbe390d0 - Tornado Cash Withdrawal 12
- 0xc697e4a47b8368fae14f7a2566e038c41518d14c - Tornado Cash Withdrawal 12
- 0x8dc81ed6508b714db2e60e4ea04219b5358937bf - Tornado Cash Withdrawal 12
- 0x79a815975c8c4c7adc1dd0d13549681cc87b4ca6 - Tornado Cash Withdrawal 12
- 0xc82c9287cb6cb69c1e3092af5709be3377c7ba98 - Tornado Cash Withdrawal 12
- 0x8aa57238c1503bab045bc7a81bb34f7454d1802e - Tornado Cash Withdrawal 12
- 0x73300fb6169972f11acda1bc128f8460bfade0cc - Tornado Cash Withdrawal 12
- 0xa2a465e9c96fa703e3298996d194dff561a1ec22 - Tornado Cash Withdrawal 12
- 0xf4d162231c426c9111951803c5c155e77759c16e - Tornado Cash Withdrawal 12
- 0xda63e2cc9f541ee5af64927ffcb0c512fb18338e - Tornado Cash Withdrawal 12
- bc1qxarm80qyvj6t6duzltdr7eectu467mg4rxaup4 - 502.23 BTC - 2024-10-14 1:33
- bc1q7ryfhqgy8fdjyuj3kjdsj4c92yhgr6s8raxehk - 503.18 BTC - 2024-10-14 0:36
- bc1qxxk4x2mjde9n379k0s8zvsf8hjyld7ehn0feaa - 115.36 BTC - 2024-10-12 2:34
- bc1pqss46x36d6mavd00m0s8m0dnhnhdqjeu7lghdlq8f5xl6w0drsfse5ktt4 - 40.26 BTC - 2024-10-09 1:23
- bc1pldggfwn9hag2uldm99g2jxk8lq33gj96cznwrcnnt426f48khk6qq4hdmd - 44.25 BTC - 2024-10-09 1:23
- bc1pdant9edksnt9llw54wjvuju2hq3sc4qqhrp7lrg6fmqgpunczf0q9s5460 - 43.98 BTC - 2024-10-09 1:23
- bc1p7wt4zv5l869qvc3snlddk446am7x8j7vhzvr34wv3dmyxt7hl7fshqx2t9 - 42.75 BTC - 2024-10-09 1:23
- bc1p7y2sn43nukck0l6c94kz784nner07sah9k3jh8lthlfaqlljpvuslqtx0y - 40.03 BTC - 2024-10-09 1:23
- bc1q2y5xkmx97g67egd24rx4em7lmeu2npfny2dlad - 143.05 BTC - 2024-10-11 7:07
- bc1qgmmfwgeu2570ym8xadpy0lfxqpnhjs55yd6etg - 606.35 BTC - 2024-10-10 0:47
- bc1qtr5adjvfvt2e7l3n0hkvypdcfglt5st43y6ylu - 26.410703 BTC - 2024-10-14 9:09
- bc1qp25qmkf683mdpwva7lpv7fyehwgkzlj9tnp5wv - 23.17 BTC - Oct 15, 2024 5:02:00 AM


### Victim Addresses
- 0x27fD43BABfbe83a81d14665b1a6fB8030A60C9b4 - Victim Hot Wallet
- 0xd83b89e261d02b0f2f9e384b44907f8d380e9af0 - Wazirx Team Member Address (Ledger)
- 0x9af78003cecc2383d9d576a49c0c6b17fc34ae34 - Wazirx Team Member Address (Ledger)
- 0xfa54b4085811aef6acf47d51b05fda188deae28b - Wazirx Team Member Address (Ledger)
- 0xd967113224C354600B3151E27Aaba53e3034f372 - Liminal's Signing Key


### Contracts

Exploiter Helper Contract:
- 0xfbfFEF83b1C172fE3BC86C1CCB036AB9F3efCAF2 - Contract
- 0x6eedf92fb92dd68a270c3205e96dccc527728066 - Deployer
- 0x0d352bc03b8cd42378d0bc71381a6a7f1c618c7824854bad5218d194bd8d7e9b - Txn

Exploiter: Contract
- 0xEf279c2aB14960Aa319008cbEa384b9f8aC35fC6 - Contract
- 0x6eedf92fb92dd68a270c3205e96dccc527728066 - Deployer
- 0x44afe9bcf348ddd163ff4309987e3e50d5973992463e0f422613bafc0f42f642 - Txn



## Hacker's Test Multisig Transactions

Contract: 0x3b5f13799f71c10e6b06844a842aa953e7494f69

see: https://safe-transaction-mainnet.safe.global/api/v1/safes/0x3B5f13799f71c10E6b06844A842Aa953e7494F69/multisig-transactions/

successful eth transfer:

- 2024-Jul-09 14:44
- txn hash: 0x655f8bee055161881c13997df3a805ad2a8efd5bbd6ec25b375fdfea4f69dfd9
- 0xB20eAAc8053a8CCF0e6F57E6Bf831249A15Df26F
- 0x6C9Ca04775ED2862043456Ed12851F4b592d77bd
- 0x47CEEe151E5042b84ec2846B6219f4A8541D870b
- 0x3470163Ab39262A0EB935904E47F83C8C3F461a1

failed txn:

- 2024-Jul-09 15:07
- txn hash: 0x397b80fa4a57fd22b17ba498a060aa1cab89d1c0de6ba15e87e1cc9e18e4582c
- 0x28B5C75C030CbD640D0f396bF35dE71ba766b574
- 0x6C9Ca04775ED2862043456Ed12851F4b592d77bd

test delegate txn:

- 2024-Jul-09 15:07
- txn hash: 0xfecfee98519dcaeecb839ffaf33225f732ef02f1d0ea0a9a32fed37be08aba13
- 0x6C9Ca04775ED2862043456Ed12851F4b592d77bd
- 0xB20eAAc8053a8CCF0e6F57E6Bf831249A15Df26F
- 0x47CEEe151E5042b84ec2846B6219f4A8541D870b
- 0x3470163Ab39262A0EB935904E47F83C8C3F461a1



## Exploit Multisig Transactions

- **Note: READ THIS for everything txns, signatures, safes: https://paragraph.xyz/@ayc/recover-safe-wallet-signers**

- https://safe-transaction-mainnet.safe.global/api/v1/safes/0x27fD43BABfbe83a81d14665b1a6fB8030A60C9b4/multisig-transactions/

- https://safe-transaction-mainnet.safe.global/api/v1/multisig-transactions/0x4e82121a3bc2fb62c0b06ab5fff5ca965ceab4f51cc949c6e50d85ed63e6aa70/confirmations/

### Example of a good / legit transaction from Jul 15 2024

- txn hash: 0xfa377a00729d54d167ebbc37a42f040c9237c56ade00843f1cc24421e2bf2d81
- 0xfA54B4085811aef6ACf47D51B05FdA188DEAe28b - Wazirx Team Member 1/4
- 0xD83b89E261D02B0f2f9E384B44907f8d380E9AF0 - Wazirx Team Member 2/4
- 0x9AF78003CecC2383d9D576A49c0C6b17fc34Ae34 - Wazirx Team Member 3/4
- 0xd967113224C354600B3151E27Aaba53e3034f372 - Liminal 4/4


### Partially Signed GALA Txn

- safe txn hash: 0x79ded740c0521bebc7449312de37cf7f9de27e2d95b7e6e57e9ecb620360b7cb
- 2024-Jul-18 05:15
- 0xD83b89E261D02B0f2f9E384B44907f8d380E9AF0 - Wazirx Team Member 1/4
- 0x9AF78003CecC2383d9D576A49c0C6b17fc34Ae34 - Wazirx Team Member 2/4


### Partially Signed USDT Txn
- safe txn hash: 0xfe1d20734698cb8f8fc21e70a797db518063bc5d059cba41d1f220cec1e4529a
- 2024-Jul-18 05:15
- 0xD83b89E261D02B0f2f9E384B44907f8d380E9AF0 - Wazirx Team Member 1/4
- 0x9AF78003CecC2383d9D576A49c0C6b17fc34Ae34 - Wazirx Team Member 2/4


### Failed Onchain USDT Txn

txn hash: 0x8b99ae634e1e7180b3fcc66e8fe5d076351477077051a7bbf5ec626a9d0588ef
msg hash: 0x50a9ff81d06bd812f55d3447c4c48c291f2386f57341a4f21c4e584d07f5943f

- r: 0bd7f89c2b11160cfed25509da814414ebfee66f002badb387847384fa4bde0d
- s: d5f08e55840e29bb7e6be5eb1d1400ea418fd89c03ed223c5864443a98c43c477
- v: 32
- a: 0x9af78003cecc2383d9d576a49c0c6b17fc34ae34 - Wazirx Team Member 1/4

- r: e70f0edc837bbad235931e9025c310a874b4e58cd0f4d62e0e4624ea0ab6372f
- s: f6ec8d5c7196c3404ca325fa6e41a93e8caa6b2d07e6b71c9e8855f2261c553fc
- v: 31
- a: 0xd83b89e261d02b0f2f9e384b44907f8d380e9af0 - Wazirx Team Member 2/4

- r: 40082eba0f71627a3451d47132b8f4c266bc9be2bebe4424848757d10f13e769
- s: 963af0b543a2357765d9f290410e919301ad065f0f2efa1233eb8634c93111f0e
- v: 32
- a: ~~0x7843965f0c2be09c9a8a04af093165175cd91e5a~~ - Wazirx Team Member 3/4
- The address here is wrong due to how ecrecover works. Ecrecover goes from message hash + signature -> public key -> Ethereum address. Because the tooling assumes that the message being signed is the same for all signers (even though it's not in this case) it thus runs ecrecover on  the wrong message and thus derives a wrong Ethereum address ultimately. However, the signature IS still valid—it's just not valid *for that message.* See [this post](https://medium.com/patronum-labs/nicks-method-ethereum-keyless-execution-168a6659479c) for more information on ecrecover and [Nick's Trick](https://weka.medium.com/how-to-send-ether-to-11-440-people-187e332566b7) from 2016 on how this works IRL.

- 0xd967113224C354600B3151E27Aaba53e3034f372 - Liminal 4/4

### Malicious Upgrade Transaction

- txn hash: 0x48164d3adbab78c2cb9876f6e17f88e321097fcd14cadd57556866e4ef3e185d
- msg hash: 0x44496341c76e2f244f0d92cf0ff7f3947788e75dd198a5a7cf4ad9020ddc8346

- r: 8e64a89386af2f223b8433a1df65db8f0ff60544b2f02c56ec02b640d6fb15a1
- s: 1f7dffda5b99b0292b5e02d0cc44508d7d8f994515358e9da3016d8098b22588
- v: 32
- a: 0xd83b89e261d02b0f2f9e384b44907f8d380e9af0  - Wazirx Team Member 1/4

- r: 3da7c6bd7c130430cf662de3d9af067c4a0629f849e29003c40ad3979cd67072
- s: 0c3ceb3a61e38fb7166353e3262eb6554c3f6571807cf22f9bdc4a83a5644166
- v: 31
- a: 0x9af78003cecc2383d9d576a49c0c6b17fc34ae34  - Wazirx Team Member 2/4

- r: 40082eba0f71627a3451d47132b8f4c266bc9be2bebe4424848757d10f13e769
- s: 63af0b543a2357765d9f290410e919301ad065f0f2efa1233eb8634c93111f0e
- v: 32
- a: 0xfa54b4085811aef6acf47d51b05fda188deae28b  - Wazirx Team Member 3/4

- 0xd967113224C354600B3151E27Aaba53e3034f372 - Liminal 4/4



### Tornado Cash - Pre-Hack

- W 2024-07-08 15:03 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0xe3b4cf64e0fc25fafb10d226984b18addc038879ed77f730abbed4737db6a5fc
- D 2024-07-09 15:48 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x6a18de11965770a233e57c7dac4e302b1800c42747c3edb57a7be9f361e672ca
- D 2024-07-09 15:50 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x9efbd685f7debb74846bf87742717dc75d72f4308bc26cc904d2e6f3147c10df
- D 2024-07-09 15:51 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x71cab94a24798265f0768495cc459e79e2969bb01621f65778f95ca80e665c1b
- D 2024-07-09 15:54 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x0524c9715e2065c27a32ae2eba33bbe54906259ed0aab746e48737c40d00204e
- D 2024-07-09 16:29 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x065d8253e5bcd2c5540283c985239bf78a4447d5273cfff81fd00fe31733e3eb
- D 2024-07-09 16:30 0xc6873ce725229099caf5ac6078f30f48ec6c7e2e 0x4956f50b21404877e492e068876945472ae6308a734ded7ebce0121120a3629a
- W 2024-07-10 06:28 0x6eedf92fb92dd68a270c3205e96dccc527728066 0x4d3cf025d6d0351c06cd0b795b113aae463570c49bcdbd2bf0e186beb0de71f1
- W 2024-07-10 06:33 0x6eedf92fb92dd68a270c3205e96dccc527728066 0xaef336f8c4cd2c5812f340b7880913c9923122e19d493c590498a7df45490cc3
- W 2024-07-10 06:36 0x6eedf92fb92dd68a270c3205e96dccc527728066 0x09c3343191c8f570f1309f7c16dda39d8d31fd1ba9c3f45f547c9d7c3bba0cf3
- W 2024-07-10 06:38 0x6eedf92fb92dd68a270c3205e96dccc527728066 0xedadeabb73a2b8b4e3508e0ebf3a85717d6246b21f94b7109cb0b8bac858348e
- W 2024-07-10 06:41 0x6eedf92fb92dd68a270c3205e96dccc527728066 0x90057766b23ec0b37427402bb28b80d352cce1ff56fc802e3d237f0e1f95375e
- W 2024-07-10 06:44 0xab7f74febc2e13a7636c305794e1c0ddd9e0d779 0x6ec7cd672fd056b07b3cd111cb6ccea827c924076d9adad1d12dfc13d3c1b8da



### GALA Transfers

Prior to the hack, the attackers withdrew GALA for nearly 2 hours straight until the hot wallet had no more GALA. Presumably this was to prompt the team to sign a transaction so that the hackers could inject the signatures and payloads and ultimately execute the hack.


| Date               | Withdrawer Address                         | Amount       | Gala Balance | Amount USD | Asset                                             | Txn Hash                                                           |
| ------------------ | ------------------------------------------ | ------------ | ------------ | ---------- | ------------------------------------------------- | ------------------------------------------------------------------ |
| 2024-07-18 2:44:35 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78488       | 1,799,820.37 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x951f35b2d7920490420f782eca83f3203f9673408e617d967ae5f787dc8444f8 |
| 2024-07-18 2:45:11 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78488       | 1,721,332.37 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xfb229af686280b90e7ed32689c6b9161429d70b3a2f97b3433cbacd41d29a9a2 |
| 2024-07-18 2:45:59 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78488       | 1,642,844.37 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x67d8d4ee6a6afe7bfa5ac076b0e75c1408d1ced085d7abf73df81bec9c8ff19e |
| 2024-07-18 2:46:35 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78488       | 1,564,356.37 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x33c2cf0067b0712495def3d75384708345507947c4b74be40f750ebed1ae65f4 |
| 2024-07-18 2:48:35 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -22575       | 1,541,781.37 | $573       | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xf48361e0fac47cc324c93deab41739aa11e957bb86fe2ad8938aca919aceed83 |
| 2024-07-18 3:14:23 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 1,463,264.37 | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xa34fd5d221222c2ad560de860ed7d4ca38e3964fbda3d9acf14e55818c8a408b |
| 2024-07-18 3:31:35 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 1,384,747.37 | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xb90e00dc30ec927a365ee97557c44232f004cf85be48be0ddbe907112d56c8ef |
| 2024-07-18 3:31:47 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 1,287,887.30 | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xd7384f6f869cebab51d1546c3ce01e584be8f977438f8ed430913d3b27048623 |
| 2024-07-18 3:31:47 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -18343.07778 | 1,366,404.30 | $465       | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x0659a7c4ab31f4c3633a3e6c7311fb69b83ae0dd69e6bbe8992deabf249535ca |
| 2024-07-18 3:37:35 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78516       | 1,052,355.30 | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xc748603118e731bbca356ba6a2987f703b577d338dc1eb4da34c5fabc4247d65 |
| 2024-07-18 3:37:35 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78508       | 1,209,379.30 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x9904103d973e13431d6eb9ead34d0ac27c9fae712e6eb10362876669264e65c7 |
| 2024-07-18 3:37:35 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78508       | 1,130,871.30 | $1,991     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xdb57d9cd788c869b2b61d243baea036cd6cd9c4a0650d8e386375c685d76431c |
| 2024-07-18 3:37:47 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78517       | 816,805.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x46a5c58e30d71519724ca6a975b9041afabe193bc5e030c8181691ec30a0dcc8 |
| 2024-07-18 3:37:47 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78517       | 895,322.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x2b040622f142650de35b071175f703d3393cb5f27b9fbeed69166d1ed9825859 |
| 2024-07-18 3:37:47 | 0x8f5376c6eddc246d7e57040b1b0647fd3cbaff89 | -78516       | 973,839.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xdf8ba9bb7286dc496f885ea8eafad6db832b359d3e97b4e7152c7ce57d19cc5b |
| 2024-07-18 3:56:59 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 738,288.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x59d36ddd5b631920c639eb186c906b4f180e9b5654fe58e30e77bbd0475725d2 |
| 2024-07-18 3:57:35 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 659,771.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x72f3968c5b1538112c37771855b08dedc2c5583bf51bd5fec4541b196b9604d1 |
| 2024-07-18 3:58:11 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 581,254.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x71ea3d00dbfaf70b8daf667588b60f9784cb5a77ed624c9962968309aa84a509 |
| 2024-07-18 4:05:47 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 502,737.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x2b51ccf0d26c0b895edefd67bb8c39343730eb9bc9104bf3a729979c01e1f7c9 |
| 2024-07-18 4:06:23 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 424,220.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xfce587965931a1587769f145abff958c6100dc8339859499a57fd22db48160ea |
| 2024-07-18 4:06:47 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 345,703.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x6057edf87428e49f4098e4182248cb3ea48a7f3a53a1c9da197fbd844bfde177 |
| 2024-07-18 4:07:23 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 267,186.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xe89db05cf8ca49f723a5133ae1264818fa687cf0cf8cddba35d34db4355591da |
| 2024-07-18 4:07:47 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 188,669.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0x9f0dc1e4cfc65fbe3d65a32787d37ab788e616373bde4ed85346e77f6df6d1a6 |
| 2024-07-18 4:08:23 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 110,152.30   | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xc26efc9151e09938135b9b04147c9dce93ec35d52b8e4b0493e360e4022b8b08 |
| 2024-07-18 4:19:59 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -78517       | 31,635.30    | $1,992     | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xc8f80fa828360c4adc238094630d7afb469c4e2700acc23708dbeff05fac97bd |
| 2024-07-18 4:22:11 | 0x9a638c0d1a40086d61584aa8861a4828440045c2 | -30000       | 1,635.30     | $761       | GALA (0xd1d2eb1b1e90b638588728b4130137d262c87cae) | 0xb1acdd66083f4cd132c5c5be6b60c341d926751c1fb8eb0e794f9be77bfee57e |



## Tornado Cash Demix


| Name                 | Date             | Amt  | Balance | Address                                    | Txn Hash                                                           |
| -------------------- | ---------------- | ---- | ------- | ------------------------------------------ | ------------------------------------------------------------------ |
| Tornado Cash Depo 00 | 2024-09-02 15:08 | 0.1  | 0.1     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x7d2fd4c3494a725b4bcaa78941aec66beb081eb79e0faaf46f0814d5295897cc |
| Tornado Cash WD 00   | 2024-09-02 15:57 | -0.1 | 0       | 0xeaa51d76d222bb502100969c1e61fe63ec48a3e4 | 0x8cf6956cd03159d91396ff9cf588757815d49532c5413960492f761618d12620 |
| Tornado Cash Depo 00 | 2024-09-02 16:03 | 100  | 100     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x7a9fc4392c39ae83e2e74c5d4682526047dbb727b50c9daefa79cc23adf7395e |
| Tornado Cash Depo 00 | 2024-09-02 16:05 | 100  | 200     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x2065281f4e19de405111ada7e6cabd85d34a6423df6a4acdbb3e3d29f08db1f9 |
| Tornado Cash Depo 00 | 2024-09-02 16:06 | 100  | 300     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x89a7e99b6ff0b5ce6f7b60a4d307cf3a4d5f92342d6e2f65c68dd46908f8ec2b |
| Tornado Cash Depo 00 | 2024-09-02 16:08 | 100  | 400     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xc624e00ee46dddb4e4cd4804be844cdcb4313bb57f5f594a3692e2f557d6b2bd |
| Tornado Cash Depo 00 | 2024-09-02 16:10 | 100  | 500     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xe9f522153656b2e9be3b0ee30b37cb47dc07b6f8a5c45b02d5919b2e458e1864 |
| Tornado Cash Depo 00 | 2024-09-02 16:13 | 100  | 600     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xa6fd258d54d5bc4110e661479209a491513cc2ef55b3f5fc26ca3190ea552f97 |
| Tornado Cash Depo 00 | 2024-09-02 16:15 | 100  | 700     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x0107afae1b2be6f16ff65c1d38e46fd05ac42901fa7ced5baa4088fbf3d5058c |
| Tornado Cash Depo 00 | 2024-09-02 16:17 | 100  | 800     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x0fa72d77c43c2a76a9ed7efad247a864a264c103d2dd45ff3bc29ed9c0b0f690 |
| Tornado Cash Depo 00 | 2024-09-02 16:18 | 100  | 900     | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x630fae5c1797e7737985adef5b2ff99d5315048eff65a173dc8b112628399ae6 |
| Tornado Cash Depo 00 | 2024-09-02 16:20 | 100  | 1000    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x90549ec1a354103016c127661c76e4bfe23221f4f877aee8a079c696e33d9247 |
| Tornado Cash Depo 00 | 2024-09-02 16:22 | 100  | 1100    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x1a7cece0d1e0f32158cf36416550dd67261d141b03c3b091732a622db75e117a |
| Tornado Cash Depo 00 | 2024-09-02 16:24 | 100  | 1200    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xdf59fd406d1457f233e2b92dd02616b9e746df534046db4d6129eae7f4fa3f6e |
| Tornado Cash Depo 00 | 2024-09-02 16:25 | 100  | 1300    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x1074e90a125a990f53b6a103b4794eb2ecdae841a061cbddeb84f00534987813 |
| Tornado Cash Depo 00 | 2024-09-02 16:27 | 100  | 1400    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x93c6db6ba2c986504f07a3ea0bfaad47d3d4a58cb3db1d65bac94b5876cda775 |
| Tornado Cash Depo 00 | 2024-09-02 16:29 | 100  | 1500    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xf07af86fbeef2c274dcedf38a93853a768dfef7b137ea8cb420b1b527e7c49a2 |
| Tornado Cash Depo 00 | 2024-09-02 16:31 | 100  | 1600    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x9866b4386311f172eb13dc9ff622ccf37bae445644d408d0d2ca0f36283531ee |
| Tornado Cash Depo 00 | 2024-09-02 16:34 | 100  | 1700    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xd68d8af8ab333271393cbb98c14b6556b073558e294d0053068effbb7c7d7c97 |
| Tornado Cash Depo 00 | 2024-09-02 16:37 | 100  | 1800    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x5ce6273315fea064edbf7f7da5c40f06136a5e4308f17319034c19006fb21472 |
| Tornado Cash Depo 00 | 2024-09-02 16:40 | 100  | 1900    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xa65d9d5eab676c7b686d997e3a0dd7996d2ed52ed95f4ceb043303d2d4a547df |
| Tornado Cash Depo 00 | 2024-09-02 16:42 | 100  | 2000    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x75cef96f3f4053a65411b4fb87c5bc212eb2b2ce2b18ce1a6bf9408f19a6896b |
| Tornado Cash Depo 00 | 2024-09-02 16:44 | 100  | 2100    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xba443b7274000588258678fc263b4d3f08f8b8ec6454bcdf6a2d537daf46b2f2 |
| Tornado Cash Depo 00 | 2024-09-02 16:46 | 100  | 2200    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x1c9af39c8771679f77e13270ceb30813e11d2eba376857d5ff1ad7442f8b43e4 |
| Tornado Cash Depo 00 | 2024-09-02 16:48 | 100  | 2300    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x831ebed7392533d5aa8f7fa192ef34f213f54782bf97e49b04bc62abe2f3a6d6 |
| Tornado Cash Depo 00 | 2024-09-02 16:50 | 100  | 2400    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x5e4f275332ecd4bb4753ae4fa9b2ed0046def2c440f8c1459ac63c307e686894 |
| Tornado Cash Depo 00 | 2024-09-02 16:52 | 100  | 2500    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0x154708719cd45eb19693506af8ea4478d688998627fce5421d8d4511b1b59a21 |
| Tornado Cash Depo 00 | 2024-09-02 16:55 | 100  | 2600    | 0x668399a6604c41d46c81430e4dff71443d44efe6 | 0xb9a80e38e342b4c953f84fea9884a6ccf0e147fcbde4ab528b15536c8fa388f6 |
| Tornado Cash WD 00   | 2024-09-03 6:51  | -100 | 2500    | 0x503b5d609ded2f5b9c9c50adf0b551145077ce2f | 0x01ed276b30a6f118113b61ac4da6ef09904947e4d445f0720ee5f43eeac77334 |
| Tornado Cash WD 00   | 2024-09-03 9:17  | -100 | 2400    | 0x25598a14b023d88cca4395ae61ea987447078e33 | 0x44e6ccd2bae7378b48b3abfb22bdf539010e1c7b9af8a6f36ae64db5c26c01cb |
| Tornado Cash WD 00   | 2024-09-03 9:44  | -100 | 2300    | 0x93745f0a2886b5363408e6ec742a1eb9753a797a | 0x2b60eb74e678a2d0e51385b4879c31b95ac44d9b0e6185082d22ece24e04ae96 |
| Tornado Cash WD 00   | 2024-09-03 10:15 | -100 | 2200    | 0x5ba7b216e8d1e898f56418730d6a916ce2e57198 | 0x020c954eac7a6a5b144f977404f9529878c54000339e3ba81c1f9e32b0743bbe |
| Tornado Cash WD 00   | 2024-09-03 10:30 | -100 | 2100    | 0x5bb826f8a40a75d18f4553c5c8b68df4b18ea0ac | 0xa3c479f00ad4081e17b7123c9e8a17dd12c398d4fb8ff7428f7ce4ffc9ff0a2f |
| Tornado Cash WD 00   | 2024-09-04 13:16 | -100 | 2000    | 0xe93d293af6e7baa4081062a656d0b8c236c2252e | 0x07a9d181b072539a4cfb296d1961ccea78206ab0d106111e8e205370556f2968 |
| Tornado Cash WD 00   | 2024-09-04 13:47 | -100 | 1900    | 0x61e89052cfa44c160afa96f93ff41e707366bf22 | 0x307b06092d17999cd55bedae17332f60ff8474f2f5436fb71f5fd6ca44cf1295 |
| Tornado Cash WD 00   | 2024-09-04 14:21 | -100 | 1800    | 0xc22fb23ed9634059b66be469b845251123814069 | 0xff355fd0b053f2ef482e54b19ec7808881ac29340507edd713b8c33c4b6d6342 |
| Tornado Cash WD 00   | 2024-09-04 14:38 | -100 | 1700    | 0xcd0a731a65c07b0340c055e379af96d2a704a4b8 | 0x4538bdc4206aaf72a58c74e40b6ac783f1553cd686cad2d06b93af4f294b7d45 |
| Tornado Cash WD 00   | 2024-09-04 15:01 | -100 | 1600    | 0x2c4af2b55654627df0e5cbf33cc7f2dcff6d35aa | 0x88f77cdc4322b8ed768a6526da13b6c0030a868911483705f792c006807fe88d |
| Tornado Cash WD 00   | 2024-09-04 15:15 | -100 | 1500    | 0x83c3ffe81cf6d0def25e485cfc1db5d2cf7d88c6 | 0xcecf72cc2da0d667fa0b55fe8fd021e6d6712b0568978655216d66d31749f543 |
| Tornado Cash WD 00   | 2024-09-04 15:50 | -100 | 1400    | 0xa71e05fb34fb79702da02e0f94e376382016d014 | 0xda49753bf97dbbb50d08c802ef980f71e4b2dd6b1ec761ea3fd23fb12bdad36b |
| Tornado Cash WD 00   | 2024-09-04 16:50 | -100 | 1300    | 0xfcf701753198c6870a7b2433039d66261035b926 | 0x9bf9f074f9d7c40d1c942a199b3c11df10254318b45f2f6b3eaf70a613924e02 |
| Tornado Cash WD 00   | 2024-09-04 18:00 | -100 | 1200    | 0xb461ffcbe2e54b22734e0f3cc375d4d456d4a1ff | 0x738c1a42e5b63da25e1f3288616a66b71e09b08e572f760306944bf684c1ab00 |
| Tornado Cash WD 00   | 2024-09-04 19:13 | -100 | 1100    | 0x75521e328b2424e81d61c152aaf6f8dc8eeefbd1 | 0x25a260a3b0bb006ec6e1be7397cc2678efa4bce4670f02bde5c4a8737b6efa2d |
| Tornado Cash WD 00   | 2024-09-04 20:20 | -100 | 1000    | 0x3e59fc3e9ab3f729be5f5a88398978a314807c55 | 0x6c5965670ad88efa6249ce285b71c8c69afabd95d4b0b1a012143f1f5a40ae8d |
| Tornado Cash WD 00   | 2024-09-04 21:25 | -100 | 900     | 0x29c86175b1f086ecedb5f2e6f993c1ece1ebd143 | 0x34c4f1d3051c80563e17e7131ba5af5a12469968cb617c4d896785dfbc6adb36 |
| Tornado Cash WD 00   | 2024-09-04 22:46 | -100 | 800     | 0xa70f8cdbe25d4bab8d77168832c0a680f38aed40 | 0x0b654afa7e691b63505b9a2cb2a659670d430b11350c727e596d746a98a624a6 |
| Tornado Cash WD 00   | 2024-09-05 0:01  | -100 | 700     | 0xe326c1b51c338371f12d880b4a6e75295d51a204 | 0x6bcdadf84f800bf30e352c2b2e87a97786f97b6645440bf15ef49f0e9871955e |
| Tornado Cash Depo 1  | 2024-09-05 7:57  | 100  | 800     | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x1699d0ceaf3326fdb73492ff54091d839a776374997f06f40dedea11a5771c85 |
| Tornado Cash Depo 1  | 2024-09-05 7:59  | 100  | 900     | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xf06bb7b1c0e327d6bc58598afdc39b241eb3c27f2aa152a6cd634f661236745c |
| Tornado Cash Depo 1  | 2024-09-05 8:00  | 100  | 1000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x911c6df194e903e5aa2495a440641b6de7e57c4b0d094f331b02fb9c2cfb4277 |
| Tornado Cash Depo 1  | 2024-09-05 8:01  | 100  | 1100    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x2bfa4d11e6201b722f59465f7388a98353a45e24fc9dfa5ad8e848f4bb5e7024 |
| Tornado Cash Depo 1  | 2024-09-05 8:02  | 100  | 1200    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x510dc9952ef0d8dc7a1db137206fa8592a20cfb61332e6cbb9564afa6cc5fcc3 |
| Tornado Cash Depo 1  | 2024-09-05 8:04  | 100  | 1300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xb6a5554b07bf753d69398dcae77b3bf9a2685b939537b8c678cdae1a7357579c |
| Tornado Cash Depo 1  | 2024-09-05 8:05  | 100  | 1400    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xf7ccb5ee2df6315017e08277935d4d5d0e8f230603dd541d6b8ef7fbe696dd12 |
| Tornado Cash Depo 1  | 2024-09-05 8:05  | 100  | 1500    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x59f996466a4ce7b760ed12127eba5f69ea2a1dbc095630eb141c2b0d94889c74 |
| Tornado Cash Depo 1  | 2024-09-05 8:07  | 100  | 1600    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x5dc22f81c8f44603d6e030a26d0767ecc607cf8ef8d5a9912f92896c0652c957 |
| Tornado Cash Depo 1  | 2024-09-05 8:09  | 100  | 1700    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x76677b5e2b218af4308571a27d566ff942c0c4df0c5500bf50e97cfcb1c8a437 |
| Tornado Cash Depo 1  | 2024-09-05 8:10  | 100  | 1800    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x9d4ab8b53d73708a7ffcb012014a85651ad41cefc2a09bb65615c9be57100498 |
| Tornado Cash Depo 1  | 2024-09-05 8:12  | 100  | 1900    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x7e6add9a3b1a88e4f297d754a8fd34b6a41235c2f2ae6afb2e0ad1905f15cc3b |
| Tornado Cash Depo 1  | 2024-09-05 8:13  | 100  | 2000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x8818c04ce9cc9946fd4bacfe302191e13f330d318a2e8e8bd9ce062f1ff5a670 |
| Tornado Cash Depo 1  | 2024-09-05 8:15  | 100  | 2100    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xdb3d0484f1f6165c69ce25acb683a4cfe1cfc33a609468802c4e094dbe302abc |
| Tornado Cash Depo 1  | 2024-09-05 8:15  | 100  | 2200    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x642d834855e82d36e24badde5e4c911c3d74c2ab613acd624f42383e5a6d2823 |
| Tornado Cash Depo 1  | 2024-09-05 8:16  | 100  | 2300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xe123d9dcd66d802d16cdc787f62426fe4d9bf87cb86f88b58aaf3807b0ea3bdb |
| Tornado Cash WD 00   | 2024-09-05 8:56  | -100 | 2200    | 0x39ce6c2fc496e1fe2341a77c6ce946deab50955c | 0xce483fd7ce8f0a595d605150388d1975e5fece1a245184e536ab685c6c909f68 |
| Tornado Cash WD 00   | 2024-09-05 9:49  | -100 | 2100    | 0x4d0a5e0a94468839db9db0a61d668ea19a7ba7c7 | 0x580c52b50b95792a5044937bf20c0d17d7f76d3cf4303bba783523c5db974789 |
| Tornado Cash WD 00   | 2024-09-05 11:01 | -100 | 2000    | 0xff3f62158278c53db2d1c523c867e4f7229b051b | 0x7c9e066173f663c9efc40bed55267627f5f4b6924545b39fb2b69ecabcf5c304 |
| Tornado Cash WD 00   | 2024-09-05 11:04 | -100 | 1900    | 0x2a1cf2bc9f7c5f7fb97912075aaf8a79e57d6dc4 | 0xe6eaae479fb3bce6c177184663a29ba4977dc0a2c9330495befb1f6642a06d6c |
| Tornado Cash WD 00   | 2024-09-05 11:16 | -100 | 1800    | 0xebba346a3788e3da5e05f2ead2f2cf0293c95563 | 0x4c1d9997dba727e0152757df80c814741f3ad7fd9f1e8d6160d82c26207ebcb8 |
| Tornado Cash WD 00   | 2024-09-05 11:21 | -100 | 1700    | 0xcd30a63019ab12fd617a3669e5d27af0b02a2890 | 0xe5b8326cb43fe396d53f8dae14b71c11c592783f00939fc75c1d8c4fff357ec6 |
| Tornado Cash WD 00   | 2024-09-05 11:26 | -100 | 1600    | 0xfee97845154e16d12e44cfb1b42d9a6b65725684 | 0x580a2c9965c0d81634ac939ffd99d26ca95daf4fcafaef35bed9fe47f34a636e |
| Tornado Cash WD 1    | 2024-09-05 11:36 | -100 | 1500    | 0x5522ff1c89aa0c98130f75b14e564a1664f781b2 | 0xf0524e6b80efd624a2d0386372102d889bb67a5c0b4c8ba0a620e800b54cfb6b |
| Tornado Cash WD 1    | 2024-09-05 12:46 | -100 | 1400    | 0xcaaab92e972a6b1ef7d8838328be86cb0fe2c9d3 | 0x81239cc02c8c61aae053136c6b7c9ea154f6769c721889d3a366675fead90395 |
| Tornado Cash Depo 1  | 2024-09-05 13:36 | 100  | 1500    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xe5962610cd73413128726de1ee22b5f1a9b327fedc9c0ffda378d6b4768810f9 |
| Tornado Cash Depo 1  | 2024-09-05 13:41 | 100  | 1600    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x61530a544f7e0610ad302919959c65ff731652c619ea0d7dce599eb38523e5f8 |
| Tornado Cash Depo 1  | 2024-09-05 13:46 | 100  | 1700    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x620193b4165e7a36c57d09a5c1726a76383ad1e5c8dad2329262bc5d06f990e9 |
| Tornado Cash WD 1    | 2024-09-05 13:48 | -100 | 1600    | 0xbda2f3556951434a754d3790da00ef14fb0c09e4 | 0x7d8767b860f0b34b83e8952a78046c393da0655069c1625339e868ec03bc3245 |
| Tornado Cash Depo 1  | 2024-09-05 13:50 | 100  | 1700    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x3e92adb8f4954796a8797f34f6c57f2670fb79f12da8ca19ca6879bcf12a1d42 |
| Tornado Cash Depo 1  | 2024-09-05 13:55 | 100  | 1800    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xaa2a6916572293e5bf558a65b0cfe5def7e1268cf5903714beaff6b12441ef5b |
| Tornado Cash Depo 1  | 2024-09-05 13:59 | 100  | 1900    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x6fc7dc3bf9171f314b6c89474656b879ba4471506c90edeb938793043f2b4005 |
| Tornado Cash Depo 1  | 2024-09-05 14:03 | 100  | 2000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x7037c2068ae3e1fb29700deefc959afc27cb9f6b4a80fbd4ebcf51dfaae772fa |
| Tornado Cash Depo 1  | 2024-09-05 14:08 | 100  | 2100    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xce6b0bc46e4b325a9b1c88824ac9611783332a5780b0a59530f3a0ae8e267dc1 |
| Tornado Cash Depo 1  | 2024-09-05 14:12 | 100  | 2200    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x5429abc428e610f36a2d6491028d3bea7bf9448cffd9dc211c7603d2c730a809 |
| Tornado Cash Depo 1  | 2024-09-05 14:16 | 100  | 2300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xcd239608ef7e44514cbb019f39ae9ddadf2178f61997d715ff5be7c63cc901e8 |
| Tornado Cash Depo 1  | 2024-09-05 14:22 | 100  | 2400    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xe056a4181b2ec85fc4bdd334ffb9e886fd3cb6aedd3f5952484a983e495f8828 |
| Tornado Cash Depo 1  | 2024-09-05 14:26 | 100  | 2500    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x8506acf94cd18f9aaf8e294bd0e8b3a7f16e3897689e6079cf6698b45a2599cb |
| Tornado Cash Depo 1  | 2024-09-05 14:31 | 100  | 2600    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x8dd6b7789834022f74b25c09360b5fe20ddf95c55f47dd4a287eaf0459ac2d7e |
| Tornado Cash Depo 1  | 2024-09-05 14:49 | 100  | 2700    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xf1ae0872b1988d29c5a73d60820370cf6979b18bb3a22262c5c0785a3412afb4 |
| Tornado Cash Depo 1  | 2024-09-05 14:53 | 100  | 2800    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x89e6aee33c1a9904c19c6c31b3d7a7b89a62ae729ed01bc6a51b37a43cdb9f37 |
| Tornado Cash Depo 1  | 2024-09-05 14:58 | 100  | 2900    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x51a48c26fd3fb689b7a2c781d8785fcfe30fd5d06e9fa041835313f603e84665 |
| Tornado Cash WD 1    | 2024-09-05 15:01 | -100 | 2800    | 0xd17e87688bfffe5417c86c65946380b30bc4f9ea | 0xc77dad1053e1bace403a80069f88d9b9358f5ea0a6ad40275e8ea88dcd288ad9 |
| Tornado Cash Depo 1  | 2024-09-05 15:02 | 100  | 2900    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xcb6fb426e5ee903812cca12545dabc303ae90ea063790db58d255dbd47f71b30 |
| Tornado Cash Depo 1  | 2024-09-05 15:07 | 100  | 3000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x6cbec6e62f92d5cdb68fb02ee309fe0e3a2e3a17abe4d130034106ca48cdb481 |
| Tornado Cash Depo 1  | 2024-09-05 15:12 | 100  | 3100    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x60a3cf0d7c7c0e8c0afa809adda972c927d4706ba017e5f9d8851d0e6cd1c2d1 |
| Tornado Cash Depo 1  | 2024-09-05 15:17 | 100  | 3200    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xa2c9e1678afd277c7b9e065226b6916ca4ba5265d1b02176d4247de66e28aa2e |
| Tornado Cash Depo 1  | 2024-09-05 15:20 | 100  | 3300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x1304e7eeafab3b3f21e9cc912ab3d476152c7cdfc298f0c078317116dfa6d768 |
| Tornado Cash WD 1    | 2024-09-05 15:48 | -100 | 3200    | 0x6ed958235ace5fd5071699a6018e47b8b03a03ad | 0x556355c53563f4e39fcbcd0b2bb497e2444461c9b9dd1b64e7988c2c89171d46 |
| Tornado Cash Depo 1  | 2024-09-05 15:51 | 100  | 3300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xd8606dd584f6e3346cb68040496d43166e3517c96e7dbceca4c4ad702860eeeb |
| Tornado Cash WD 1    | 2024-09-05 17:00 | -100 | 3200    | 0x9afeedfc18fdc85bd13f179be2cc404dc0e7f35f | 0xd82e22d7c73d814626f9ea6a04568fd98dc45ae3871271434faa3e2f32317bf4 |
| Tornado Cash Depo 1  | 2024-09-05 17:02 | 100  | 3300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x427bd44bd4d1439e84185688aba22ab00a60250ef97d53d7ead0d34773ddfbd3 |
| Tornado Cash WD 1    | 2024-09-05 18:12 | -100 | 3200    | 0xf6d93e14590c1aedd62b1df54a3db7d40ab40486 | 0x6bc560c12711333d53c7164d2a5c8a0520d6621410c2cfcaecab4177da6e0cd8 |
| Tornado Cash Depo 1  | 2024-09-05 18:16 | 100  | 3300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x50480c9ff479775d98a2133187496091243229f5da4dbfbb2093b40e82c13f0d |
| Tornado Cash WD 1    | 2024-09-05 19:29 | -100 | 3200    | 0xfff456cd4d1b268fae7dd90dd4fc8cf6dbacdc51 | 0x32667c5e23742e075fb688729c8a529f01a310fce5b71e16097a859b9eab1697 |
| Tornado Cash WD 1    | 2024-09-05 20:19 | -100 | 3100    | 0x8b14b1233516da49f391ce64fac6725506a06ae7 | 0x8062c06e134cd4a0102ea52e8fbd61d38a8bf7200c0dbba0f6b891e98114db06 |
| Tornado Cash WD 1    | 2024-09-05 21:39 | -100 | 3000    | 0x21d368ae3f39887af65a15d3aedd4235ed402b8a | 0xfdc9219e2ac31e8bca69ee186985761e0cbec9a92f2673b769f447a90622af5d |
| Tornado Cash WD 1    | 2024-09-05 22:43 | -100 | 2900    | 0x6ac8ed3b80f10352804a361354dc2637e686aff2 | 0x13add8e5d2a66f3ff79a63526ca18ccd5baad54b8976b2efe748631540a4b39b |
| Tornado Cash WD 1    | 2024-09-05 23:33 | -100 | 2800    | 0xb7e2e4440ff429ce0458fec248b366c04a1629a1 | 0x92719e794f4058bfb3033241a8784d32283b6d236ede162a3fd109bdbfc9cdac |
| Tornado Cash Depo 1  | 2024-09-06 0:20  | 100  | 2900    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x475450799255956593c97f5ad8b7f62657e5867d72716c75700b640f9cb2b9c0 |
| Tornado Cash Depo 1  | 2024-09-06 0:25  | 100  | 3000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x948d0d8674660c2804ec8c2968cf3606d521df3d2af7ab3bd70d8943694fa0f8 |
| Tornado Cash WD 1    | 2024-09-06 0:26  | -100 | 2900    | 0xb2e684f6aa9be5379927feecfdcf8be818c68538 | 0xf05efc2b088e9b7bfa7b12bbbdd0fc9cd04b55655ebcbfc9178f23c26d683031 |
| Tornado Cash Depo 1  | 2024-09-06 0:30  | 100  | 3000    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x89513dedef2cdf9f17052b17be507eea3eb6362968251a4d058ebd5d7e2bf24f |
| Tornado Cash Depo 1  | 2024-09-06 0:35  | 100  | 3100    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x7ab6ac15328b0b175cc45dad1e236fa5735fa33bc01287521953b1d917ff223e |
| Tornado Cash Depo 1  | 2024-09-06 0:41  | 100  | 3200    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x9e05dea53c2816bf19b8a31c1897a08be36d2abb77e3956332c408bfff394fc7 |
| Tornado Cash Depo 1  | 2024-09-06 0:44  | 100  | 3300    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xd60d09c0b6aaabb05ac426e1eac2756b447951134c5a0f27e538dafc50bbd768 |
| Tornado Cash WD 1    | 2024-09-06 1:10  | -100 | 3200    | 0x7e76f45b1586c7f0d151e162c9ebcf6209a27eb5 | 0x57c45235403aa394ad0c0d994ee6e08c716c56246b895fa8a599026892585575 |
| Tornado Cash WD 1    | 2024-09-06 2:09  | -100 | 3100    | 0x063d068797dc951ce231802ecb816da961656851 | 0xc68d069b65b7d1b149132806c8e9400cf00d63e1e4c9eec148e9c322f9a7b2ec |
| Tornado Cash WD 1    | 2024-09-06 4:15  | -100 | 3000    | 0xc83c3a7c335b53efa4994b5700c4cb4d12e4583e | 0xc588e3e57ff7ac198e5cc259783a0ae59dbfe30a9ba90f759799d4d45f1c48d6 |
| Tornado Cash WD 1    | 2024-09-06 4:47  | -100 | 2900    | 0x736cb15a26b3f4c4168cfad1aac387491a96370c | 0xb527e5916bfae5bc3a94b02dfa7ba75148c423fce12ee3281e44b5a01dfd9190 |
| Tornado Cash WD 1    | 2024-09-06 5:31  | -100 | 2800    | 0x420bd3424159396c9765331aaf3867a63e4a2a13 | 0x7c869241a6f68d0049db78d33613c47ed13a8cb57c16c8d155cc6bb1e370595f |
| Tornado Cash WD 1    | 2024-09-06 6:15  | -100 | 2700    | 0x75d9a9b87009508a4786655d2f57b0231e69db80 | 0xace97a6e1ac6c4ba83d84259ce31acf3aadac8fd634e816f2b8e5403fd3831ac |
| Tornado Cash WD 1    | 2024-09-06 7:02  | -100 | 2600    | 0xeddf1e3d7f080f44f889d6edf126d6c638cb8347 | 0xa37f36ab05ef283def1fd8e2cad4aeafc65e5f21cffcf3ab956c1ee3bdff2e85 |
| Tornado Cash WD 1    | 2024-09-06 7:46  | -100 | 2500    | 0x8e08628c4cfca575bd54c73eab4741ef214814e4 | 0xd4aca7ce4e4292ea2f908e8cf92cf6730e37f40b3506a77e32a83ca9afd908d5 |
| Tornado Cash WD 1    | 2024-09-06 8:06  | -100 | 2400    | 0x98e7efd0407cfce0999578a67769a50d519c2ff9 | 0x666f3f53e606d25da0c5e8518b7ee6f57cb48cc40ba24ac9212753bee383099c |
| Tornado Cash WD 1    | 2024-09-06 8:24  | -100 | 2300    | 0x723c2ca50994f079b6cc7bca869514060505399c | 0x4163a93a27981a3718bcb28e12ea54293cd919a3912f9b98cfc1108e873d20d5 |
| Tornado Cash WD 1    | 2024-09-06 8:46  | -100 | 2200    | 0x7854a2bfaaa0bf9c94015bc0d692a7bcfa9ce78a | 0x80ac50306840eba4841fe431f8d744aba4cf708c904672cc10fe907b2bf6d1a0 |
| Tornado Cash WD 1    | 2024-09-06 9:09  | -100 | 2100    | 0x37995c401c195466c5938426d5a1797798ab4063 | 0xec100e5495eaef9d9a0d3201f0c43825202c1fbbb5e86010010f20595869c9e2 |
| Tornado Cash WD 1    | 2024-09-06 9:22  | -100 | 2000    | 0x065188749972e424bb48fc34626b668c38f09590 | 0xf85de1fa0e52825d0f2fcb0d16bac60c39a334f6d77b0b6bb5c4d55ce8217310 |
| Tornado Cash WD 1    | 2024-09-06 10:02 | -100 | 1900    | 0xabe1b839834edcbdb863673a88dc0a0ee74fc1e4 | 0xee5bd682c9a5dcd5f2c734a2e91bc6fb9877fa580c27cf83896535aa15e24c93 |
| Tornado Cash WD 1    | 2024-09-06 10:20 | -100 | 1800    | 0xa481f40f5ed36c2402de99faec5ed0a850f092ee | 0x37a305c5e9e33a140c375f485630cacf3d747e4b55f982bb4bf5c67a75d314bf |
| Tornado Cash WD 1    | 2024-09-06 11:22 | -100 | 1700    | 0x63c2578e35fad63e97076a6d93a256fc89846f98 | 0xecf06a47bf8607d2abe72998a3c1ca77f7347da8beb0011fe8c979733f63a19f |
| Tornado Cash WD 1    | 2024-09-06 11:48 | -100 | 1600    | 0x38f5322799f8a94e1940488253b45979d6e6f215 | 0x9858a7c1c888113bd4de7250274d523a2dd5cf9341e62bde3263c38ce4358c83 |
| Tornado Cash WD 1    | 2024-09-06 12:37 | -100 | 1500    | 0x03dd0a157b2e43b31c829b5ed67b4e76542b4a7e | 0x09ac954cbd6fc1939223ae55ea08e6da96a8e2e7356ab72428842f0681268603 |
| Tornado Cash WD 1    | 2024-09-06 13:32 | -100 | 1400    | 0x33c2cd1d1712e9b116a40b7a27cb63048aa377cc | 0x57b0f7f0f8025729c5c1d1e0496722219088c054ca61256f904c056b343f8cb7 |
| Tornado Cash Depo 1  | 2024-09-06 13:35 | 100  | 1500    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x0a62258a31cd72c38f07edff1dbed929571ac873211d4c247e562237172dc378 |
| Tornado Cash Depo 1  | 2024-09-06 13:43 | 100  | 1600    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xba0873308d50482c809af4d0a8e8dba627da905aa5486b84b3ee9878b6fe0a4d |
| Tornado Cash Depo 1  | 2024-09-06 13:48 | 100  | 1700    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0x9087afefc5d334ec3a84d1c77586174b5db626d508c2a6c15d2420e22f622249 |
| Tornado Cash Depo 1  | 2024-09-06 13:51 | 100  | 1800    | 0x2d2906f7c8da32e87064d9e71c98f39b2ceba968 | 0xb4e512ce2e53f56420e050babd48e9e43dd4ddb068005dce65b2709ebe4c5d92 |
| Tornado Cash WD 1    | 2024-09-09 6:40  | -100 | 1700    | 0x6ad463fa0b5260b71a2e1f690757bb123d4fdf50 | 0x552a9b4d874b47896b0921b66d2e92115d20a8903bcfb8c58da7d81b515dc7e5 |
| Tornado Cash Depo 2  | 2024-09-09 7:44  | 100  | 1800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x45546f58e7350bfc1f46dfb4dfa08eefbda6dbfd4f5c0289d7a5d387d7f182c8 |
| Tornado Cash WD 1    | 2024-09-09 7:46  | -100 | 1700    | 0xd1c4bb31251eb53bf4bfc2fde2b771a8406f2583 | 0x256619d1f5053c8f15380cba72a0f96b63701cf7314cef156a3500ebac24e5fa |
| Tornado Cash Depo 2  | 2024-09-09 7:50  | 100  | 1800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x2c1ae0cefbb14a97e642561dc177d8db34879a901c5fd7aeb915697650f372f1 |
| Tornado Cash Depo 2  | 2024-09-09 7:53  | 100  | 1900    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x262a842a0832b6d582f2ab7f66379a14f2c4ca1c17c052c33612f2111b0cfb33 |
| Tornado Cash Depo 2  | 2024-09-09 7:58  | 100  | 2000    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x71af0fe927a62437ad37801a4fc7e4114ad470e95409bfbdb85b5b61879addb8 |
| Tornado Cash Depo 2  | 2024-09-09 8:03  | 100  | 2100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x88186e76251798d60191a5deef41b22140f2ed6c31d09a1308204302f9c9093c |
| Tornado Cash WD 1    | 2024-09-09 8:06  | -100 | 2000    | 0xc327390a51e0314f1b61b9706035731a69dd5584 | 0xa63343f148ab0f32e55bda370091db6fd6cb9e4b932096d4c2ee4e5f65264a1f |
| Tornado Cash WD 1    | 2024-09-09 8:25  | -100 | 1900    | 0x114a763450df9426e1a16a43d7e6bd7d3c355149 | 0x838e2138e755559bc199fb0857db51b99784fa1324da045ca54a8fb641f54656 |
| Tornado Cash WD 1    | 2024-09-09 8:30  | -100 | 1800    | 0x3d262da3227882db9bc6c303fbf0de63736e3252 | 0xa7ef1c1cef6945038eef11e4956714498ff147c102450418defb61b38bd3b6ce |
| Tornado Cash WD 1    | 2024-09-09 8:53  | -100 | 1700    | 0x55987d456afe204cd9bbc587f4dc5e35ebbdc95a | 0x7ee176be0e882531bab9fd4cf84424557f693c68c6f84103d463baf71aee84b8 |
| Tornado Cash WD 1    | 2024-09-09 9:14  | -100 | 1600    | 0x48be2e6802ee8070f075d3ab9588b7e076330548 | 0x8af77909d6fab6591c71697568bf6b8b82e8970b4a95f28a45d94c7022ced754 |
| Tornado Cash Depo 2  | 2024-09-09 9:21  | 100  | 1700    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x698d403930c43614a998700243dc32ce8a286c156a11e909b2e7e3ebb3a1a8cf |
| Tornado Cash Depo 2  | 2024-09-09 9:26  | 100  | 1800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xece8c267db1c889ea86abfa93751669ce93e28844415424c00b79550019c6408 |
| Tornado Cash WD 1    | 2024-09-09 9:27  | -100 | 1700    | 0x070460959b6e715f6ee83b5cb6341816a41f7e89 | 0x3e4f640e59dbaf774c604a4be82203a03ed3c6d4f94a2ae7e2383e662a5beda6 |
| Tornado Cash Depo 2  | 2024-09-09 9:30  | 100  | 1800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x5982f07da70cfa4882f5603f5790702fd9c1c8438f4262851ecf321380e0154c |
| Tornado Cash Depo 2  | 2024-09-09 9:34  | 100  | 1900    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x9377c57b46b56a8a45c823d90143164977cd02c594df987eb2912907c1f492ec |
| Tornado Cash Depo 2  | 2024-09-09 9:40  | 100  | 2000    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xaef210cfd4ef626379fa9ff82bdc90666a4e157f72268e012c391c1f6c40686b |
| Tornado Cash Depo 2  | 2024-09-09 9:44  | 100  | 2100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xf92cf5921443bbcc6eecc170a2f2151af97e84b1a6709bd2cba0f0f35bf800a6 |
| Tornado Cash Depo 2  | 2024-09-09 9:48  | 100  | 2200    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xac599de4143f83c48aab42d9cb2696d7675e9861e52e97d07b37935bfcc19c00 |
| Tornado Cash Depo 2  | 2024-09-09 9:52  | 100  | 2300    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x3f81c22c0d2402abcbe56ae630faa17c4adde9a1f66b277c81ddc6ead9258293 |
| Tornado Cash Depo 2  | 2024-09-09 9:57  | 100  | 2400    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x7ec4649bac41cf38e81df3334db44fec53b1e290121c00d9b9a965b530f58ef9 |
| Tornado Cash Depo 2  | 2024-09-09 10:02 | 100  | 2500    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x55b28257803f728c6e31c83dbefff8126ea033db01faa20f600b7c7569fb916f |
| Tornado Cash WD 1    | 2024-09-09 10:04 | -100 | 2400    | 0x380a4458aa5c10de720ddfa641a135d64b078473 | 0x7347af88793774da6b8ecdb505f76b9fa2af38df37342974b1b7a68ee388f30e |
| Tornado Cash Depo 2  | 2024-09-09 10:07 | 100  | 2500    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x0de31c90518f2b88f1c864a657e6353b8602c8db66086d6aadb32dea88c15a54 |
| Tornado Cash WD 1    | 2024-09-09 10:09 | -100 | 2400    | 0x1f5875d6724bb0688415936c482388457aa0ed31 | 0x828714decb648a2742087772f233ecb5958d765f805af3dab1afc09cdf3a0b87 |
| Tornado Cash Depo 2  | 2024-09-09 10:12 | 100  | 2500    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xdc846bf92a1a992fdf43a803641385231443e7b3f38435ceb3c76d3f056d0c31 |
| Tornado Cash Depo 2  | 2024-09-09 10:15 | 100  | 2600    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x7d3545f4024ece8550c5453d8b4b0bd27588f9b6f7581243bbe84096b0b84da7 |
| Tornado Cash Depo 2  | 2024-09-09 10:20 | 100  | 2700    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x280f67599b3d491cb31341d60602ebd5cd956a5a77b06efb364597eadc578842 |
| Tornado Cash Depo 2  | 2024-09-09 10:26 | 100  | 2800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xbe515606ca1a49a3ef3bc1880f702c1e3a022e36a78afb64963ab92b9c961a23 |
| Tornado Cash WD 1    | 2024-09-09 10:32 | -100 | 2700    | 0x5acd02a81f47b2342c1ee7034981a3d0c65d216c | 0x9c24cf138b69d2727ff80300601c174200ab14b222b312957c0bb9c5d9be2adb |
| Tornado Cash Depo 2  | 2024-09-09 10:32 | 100  | 2800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xb7f31aabbfd379e1e56c91f31ff0be00761f7ebf67e7851746c879c8725b6aeb |
| Tornado Cash Depo 2  | 2024-09-09 10:37 | 100  | 2900    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xde71b428b0310716c49c5bf262a685afdecc02fcd8c1d44a7f5a4a3d344b8da0 |
| Tornado Cash Depo 2  | 2024-09-09 10:42 | 100  | 3000    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x99e36fee2359294962f6851361e78efb77865345344e7d7c09c20d73885f43db |
| Tornado Cash Depo 2  | 2024-09-09 10:47 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x5879514b467fe804136d8b6ba69257e681784a4401fc04f8f11bda6057942eb2 |
| Tornado Cash WD 1    | 2024-09-09 10:51 | -100 | 3000    | 0xa41c73c86c2a378ebc934b9a32a1535bf45e49e7 | 0x5b69b5705f24f604bc19139f7a254e48c93edebc774717e1eef867db68c8c89f |
| Tornado Cash Depo 2  | 2024-09-09 10:54 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x86e7f8d92b94743afaea25128a5b65046e41543dd53ff7cdd76fc35d4d311a96 |
| Tornado Cash WD 1    | 2024-09-09 11:16 | -100 | 3000    | 0x2542766b393bad6fe929409553be2a5f58937575 | 0x43cfb1aa59b7387c78f2b929d540213d93860bf84f432a34a112fcdb72f04fe6 |
| Tornado Cash Depo 2  | 2024-09-09 11:18 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x07d9ad9111e3b8a017cf6e16f6f7505116c5ded8ad4bcbf8d097d335efa31210 |
| Tornado Cash WD 1    | 2024-09-09 11:46 | -100 | 3000    | 0xdfaf096b7e84079791639a1aba19debf6f921448 | 0xe218921d157849b3476e3b43d75c7e665183f8fcbbba772bce719b9f85ecc47c |
| Tornado Cash Depo 2  | 2024-09-09 11:49 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x16d08d8631743a423046eaa7d3189202e23e50622742a4189b3aacd1992eb153 |
| Tornado Cash WD 1    | 2024-09-09 12:26 | -100 | 3000    | 0x5723930a322db18a18486ae11d8b398d52ec00a5 | 0xbf4abb8d9de4350f0b4a45397df515cd8bc5bcf0a7cda4c3af03ed105d21e002 |
| Tornado Cash Depo 2  | 2024-09-09 13:15 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x425b0cc795ee43c313da038cf2a08ded05db76b29fb2f437e3076c0859368add |
| Tornado Cash WD 1    | 2024-09-09 13:16 | -100 | 3000    | 0x4393daf80347f9934e499f55658440dfced5f0dd | 0x81a182c035ee7bfc7bda46aba9622507f97a384ba7f99994291c71cc7d9c596c |
| Tornado Cash Depo 2  | 2024-09-09 13:22 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xb81c33b99f856522c6f03f0e8601fa733dfc46f04a75fb54e44bba48615bcd8e |
| Tornado Cash WD 1    | 2024-09-09 13:53 | -100 | 3000    | 0x7992395e84e8b3e099f90b113331ccbd6d9e3b8f | 0xee1a98afb00e5653a3c0ed65a9970967f7a289d34638b36b5da5323eb60f0426 |
| Tornado Cash Depo 2  | 2024-09-09 13:57 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x0d09f26bd11b47ae0c8d9d2b83c22d6bdde460c187e8ef6a0aa6d0b703b4fe09 |
| Tornado Cash WD 1    | 2024-09-09 14:26 | -100 | 3000    | 0x9bb7f2bae2e466d72050cc6c92ef197510010218 | 0xc161d4f94e60ce69ef43fb18296c1da050161d69fb7c2f5ec480bc69e949b0cf |
| Tornado Cash Depo 2  | 2024-09-09 14:28 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x5e49f742196c5bfe3e6674a7035f610dff794e494d4d0be62f06d01de46e2193 |
| Tornado Cash WD 2    | 2024-09-09 14:50 | -100 | 3000    | 0x563e827b2d17bdaabb4ff1b1f7c0c09e3c0faf48 | 0xaae43401a2b5147f563b0af6a1791048ad008c7d725ccf900416c0bc9a329287 |
| Tornado Cash Depo 2  | 2024-09-09 14:52 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x7e98a5f0b2722e30b1f05412e867ba7e1fac76401b5508daffe694c7ac8473d4 |
| Tornado Cash WD 2    | 2024-09-09 15:04 | -100 | 3000    | 0x4948733611e4ae112549511bc9e9d588ff5eed37 | 0x33333a48beec28427b301ad04e22300293be49831e512854407180782b1af9e4 |
| Tornado Cash Depo 2  | 2024-09-09 15:07 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xb911848c5c44e5d0f4e15d460d47f672fdce9fabd02fc2cfc0384c1650cd38a6 |
| Tornado Cash WD 2    | 2024-09-09 15:33 | -100 | 3000    | 0x32c73d97b8ce9bd156943792fdf9c6d7c6e76c27 | 0xd7034f37499e56eb4d250c57038d2099f7ee79baba1ba4859736ebc705b19dcc |
| Tornado Cash Depo 2  | 2024-09-09 15:47 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x98133fd4dd53597f6d4c55553878b1901301cddcb8e2e5ade17e07188b0ec169 |
| Tornado Cash WD 2    | 2024-09-09 16:19 | -100 | 3000    | 0xa67024438a304371e7af0b27a0d7c68acaa88cc4 | 0x036bf5eb26e88cf37a260df84403191eeece2e90dc2ccf02fb76560c9d3a662e |
| Tornado Cash Depo 2  | 2024-09-09 16:21 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xe793788278bf60e236cbe9f4261c87cddc4e4bb59fa5ad4dc7ac8c8a898036db |
| Tornado Cash WD 2    | 2024-09-09 16:39 | -100 | 3000    | 0x31346d24c48088830c4d940a6645cd69e3efe6f3 | 0xa927bdb1a7b7069dfaeec13e57717c72ad8232cfcc88e81d7315c449f9215e17 |
| Tornado Cash Depo 2  | 2024-09-09 16:43 | 100  | 3100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xd76ddd47b65f53721fafe9cc8fc0ea5a160b17628d2367d48de0ee42a9f3ad78 |
| Tornado Cash WD 2    | 2024-09-09 16:54 | -100 | 3000    | 0xf56c522fb72241961569c199f3d2c6522b303dd9 | 0xc2a1cf44a1ac2554e47a263429b5196cfeb6a71b5193362638861c8656a59aab |
| Tornado Cash WD 2    | 2024-09-09 17:30 | -100 | 2900    | 0x0470857ebe0a4d79e8f284a9303331e5c85707c3 | 0x93d21998f6eeb6f0b06024697de12f390b91b1b82e5999f23fccdc12b26a35b9 |
| Tornado Cash WD 2    | 2024-09-09 17:35 | -100 | 2800    | 0x9cd09c8a39a2d586a78ef39e38179686d3478887 | 0x3177e18bca27d81e0f1e6507e7ea0d4ae0b5bdff20d671f08838232b6309e231 |
| Tornado Cash WD 2    | 2024-09-09 17:59 | -100 | 2700    | 0xb6638549b0ab6fe68c5fd456ea5b7e2a7ab4f570 | 0xa789af9792e011b497bf714eb759363eef2bc50a45b64af7e0ff311552278efa |
| Tornado Cash WD 2    | 2024-09-09 18:33 | -100 | 2600    | 0x069a8676371b88133595b1f6776255d5aa1e7957 | 0xda47680c5563a3d191d388880c83d75117a0cfda851203cbc2cdf249df0592b9 |
| Tornado Cash WD 2    | 2024-09-09 19:10 | -100 | 2500    | 0xcdd501569ccde58b837f48fc9b25e1b6cf67c3f2 | 0x146e4d2f3342f085083f97dbf8277ce922cb4fb4053516106184d7be1f9cec00 |
| Tornado Cash WD 2    | 2024-09-09 19:47 | -100 | 2400    | 0x649cf70786c6253f991446608e0430619156ad92 | 0x3a1f9a2f6d5657d8995a634abe7b2defeda1f3e9159292c4132c84d557df90f1 |
| Tornado Cash WD 2    | 2024-09-10 0:21  | -100 | 2300    | 0xc82a0bc8a4964c32a924e9cb1df94bdd13dcc40f | 0x6d07299d762c91e2c84af957d9c5a708988e64138c24e7e9398eda444b1d4db7 |
| Tornado Cash WD 2    | 2024-09-10 0:51  | -100 | 2200    | 0x4e759c258eed410e23fbcbf40aa3f9a773870858 | 0x85062ab4530027df19c60900f1827b4b5cf5a007f3c986bbe11880e01f29a1e9 |
| Tornado Cash WD 2    | 2024-09-10 1:02  | -100 | 2100    | 0xf2df936ca1f2d54c75bfd88882c28614a0479fa6 | 0xf62082c7a10e0e90dcc3137d460215b767382574c8388dd244bc561865b325c7 |
| Tornado Cash WD 2    | 2024-09-10 1:35  | -100 | 2000    | 0xf21b1c45a198f50b78104ca32cecfa304811e841 | 0xde83dea957e3e1574daf744ee7a7725b6fb1e4851531486a47d52d05f5bfcc14 |
| Tornado Cash WD 2    | 2024-09-10 2:08  | -100 | 1900    | 0x17be94eff0eaadbcff1b301bb8aaee759ddb0263 | 0x228a47579933c01030c61e16509743e9435cbbaeae3e0a27303ccc839b4ce197 |
| Tornado Cash Depo 2  | 2024-09-10 2:21  | 100  | 2000    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x526bf4ad7803615ff9788ee1dac87f04e17a32eff7df5ee143d63eac41cc129a |
| Tornado Cash Depo 2  | 2024-09-10 2:26  | 100  | 2100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x23078eaf28a2fc0cdfbe8400e57ff9b77a01f35bb37ae4602e62cb3163eece4c |
| Tornado Cash WD 2    | 2024-09-10 2:28  | -100 | 2000    | 0x53c2c50f6a2b5045c7ac5445db514102c2319392 | 0x7ac6dbf390ebf2d64307e5294d2b8bdf68300e230c63054ff4dc78d488451d53 |
| Tornado Cash Depo 2  | 2024-09-10 2:31  | 100  | 2100    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x6537b97a334304437395e8cf019018fb6f3b25172f5098b7ca24d9bfe707d6d6 |
| Tornado Cash Depo 2  | 2024-09-10 2:35  | 100  | 2200    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xf8e5c3f06a6882192806df05374c7b2af8d4e64d3a92140de600b370c0e342ef |
| Tornado Cash Depo 2  | 2024-09-10 2:40  | 100  | 2300    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xdfa6d434429f1ce5aa7d53a006e37cb2cb01db00aec4c7419e4c0843b6cef9a7 |
| Tornado Cash WD 2    | 2024-09-10 2:42  | -100 | 2200    | 0xc77cbd8780dbbe1ae352672cd664548bda58e58e | 0x0919101280aaf5150a13d1db87a7a529480a82f8b4e078dfaead84cd1266712b |
| Tornado Cash Depo 2  | 2024-09-10 2:45  | 100  | 2300    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x2cd3194023611a2e40d177b8b075b1a738f2e169f8d93ba1eec27ccd5d908d35 |
| Tornado Cash Depo 2  | 2024-09-10 2:50  | 100  | 2400    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xee4a8128462a684c4032c6fb4cfa95756010e72b931861d693c051b181562608 |
| Tornado Cash Depo 2  | 2024-09-10 2:55  | 100  | 2500    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xcdce27fecef20f47ff43ddc382b402da1e89dea3a59f74265e02d2f6398e3775 |
| Tornado Cash WD 2    | 2024-09-10 2:56  | -100 | 2400    | 0xbe21ad235b3f322f1fe023f187052f95277d1c47 | 0x1ecb144ba787a154b0dc722a4a75f7915ed5d150e9d0bc2ad5129af57d414295 |
| Tornado Cash Depo 2  | 2024-09-10 2:59  | 100  | 2500    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x0f9d94442f59c2b52ada938d31e7ea7eb20f7f041284dd0377c2b18c1966c1f0 |
| Tornado Cash Depo 2  | 2024-09-10 3:03  | 100  | 2600    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xe43d1625f55b2ff22bb8927ca4da63d73b24e7a9b024d4ed914c5c095c94cfd8 |
| Tornado Cash Depo 2  | 2024-09-10 3:07  | 100  | 2700    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x87536952f76cd8cd2589c1a12f2b16851710c18dec583ba1aa04fb1acb8d45bd |
| Tornado Cash Depo 2  | 2024-09-10 3:13  | 100  | 2800    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xb86f65a7d8c89c3241a7a4135ec4948492d11019b85f57748ad48b2fc8d00c39 |
| Tornado Cash Depo 2  | 2024-09-10 3:17  | 100  | 2900    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0x896963dd5f1620bd06230622a9822e2548d0a0cbf907a2e5f9f718d6ce2fdb9b |
| Tornado Cash WD 2    | 2024-09-10 3:17  | -100 | 2800    | 0x3f1a3d41090f8cf9a4289dae958b194c4bd8346d | 0x4e25f704ecd9fb6fd2f07c59b698dd0db86a87479d240674a0a4a7543811a40c |
| Tornado Cash Depo 2  | 2024-09-10 3:20  | 100  | 2900    | 0x93097b0a0ace8fcd0b2337ae5dc7f638c48234c2 | 0xae971c8030d72aacf612f3a809d98745db0acced4f5c7bb8165cac7ea18f8c79 |
| Tornado Cash WD 2    | 2024-09-10 3:29  | -100 | 2800    | 0x909b6c962611120858149015d17c4adb2395982d | 0x45e076d749dc1b4507b6ca722300199706ba2e4647c5577ed22f253f1d53dd0f |
| Tornado Cash WD 2    | 2024-09-10 3:42  | -100 | 2700    | 0x414fd5885970ba1aad0f8632bbfc4db9e3894808 | 0xd8cfacad8a2e48be7645cae6a1dab973a1ec3839cf8eee7bdd3b2ae616d3149d |
| Tornado Cash WD 2    | 2024-09-10 3:55  | -100 | 2600    | 0x157be205a78f29c34b179a39f97fe9418022132e | 0x7d84454e7f05d3ebcc80299ff719ba4b923cdb6164113aa6da68ff2aafe068e0 |
| Tornado Cash WD 2    | 2024-09-10 4:14  | -100 | 2500    | 0x43b32303d28733ea1178249857c2db16edff40e3 | 0x567b941c21a6e29ec178c65424ce52257457723686399ec8cb49f5d42f333418 |
| Tornado Cash WD 2    | 2024-09-10 4:41  | -100 | 2400    | 0xe82c488da2118fdbb1b0aedf1cb08838ec7bf234 | 0xab814587ded2506b4ff103e3461366b75084dd4958fb706378d0b71ac818a5d9 |
| Tornado Cash WD 2    | 2024-09-10 4:56  | -100 | 2300    | 0x66e9736d032c021f282cb037c3e2dfd404767ca7 | 0x3cd8ab84df870cedbcfcd98372d6274aed2c4caf3fdef2c1d35943b3f30667e9 |
| Tornado Cash WD 2    | 2024-09-10 6:25  | -100 | 2200    | 0x4cf1dc4d8b43d2d49b5b44531a49401f6aed558a | 0x04e651a152bc612a22f36cfe6f0d35e79bfc9e6a32faeb52e51fa3c9a3ccd3fe |
| Tornado Cash WD 2    | 2024-09-10 6:27  | -100 | 2100    | 0x5f86de8e2fade60c52a6e7a2b950d709df2514c2 | 0xea00b07f4f0736a2900ba0418d20aa2baac74773167957af9fe164233efc5b4c |
| Tornado Cash WD 2    | 2024-09-10 6:31  | -100 | 2000    | 0xec0f8e7e2adeaa57b098070dea413b5919d6280e | 0xcffe7726ab8eb1cddb90cec29fc502a75ad0a178c6d5447641091681fdd90957 |
| Tornado Cash WD 2    | 2024-09-10 6:38  | -100 | 1900    | 0x2ded09d2e7a545b1658807a97cd0f83be7c0a352 | 0x2f31f1fd59a102099550ded00bc1dc16c1b03a7b3fe7e9cc34be261b3c99f332 |
| Tornado Cash WD 2    | 2024-09-10 6:42  | -100 | 1800    | 0xfb3fa66705e55289b4367f4e9cba45d6e8674e39 | 0x258fb3217a5b54e4bce688f9a0db82bdde5da3490b0c2148addda1e1040c3ffd |
| Tornado Cash WD 2    | 2024-09-10 7:14  | -100 | 1700    | 0x6250b473b9c2776b268af1cb0a2e57c1ff8693e9 | 0xee58a7ca99b6b5b82213f5d8ac7606dd4fc7145f28a633956496d2e918e606ce |
| Tornado Cash Depo 3  | 2024-09-10 7:27  | 100  | 1800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x95029aaabbf6a5b2e0616314d1cdb49c5077404b9e45985161ba0e9ae89fc9df |
| Tornado Cash WD 2    | 2024-09-10 7:40  | -100 | 1700    | 0x61e0c434eec3a47d9f303efdc87d41cf891b4b05 | 0xaf5cfcd46a381cf635ded1638cea1e0755e9ab38be7272fbe81f99f25ea7d223 |
| Tornado Cash WD 2    | 2024-09-10 8:14  | -100 | 1600    | 0xe4f1e2a69b6b1fa1e0bd7496def85150c5f38a12 | 0x813b378a01cf04a8d315f6fe87425954a9740993da5513af55b9c5b94ad99468 |
| Tornado Cash Depo 3  | 2024-09-10 8:30  | 100  | 1700    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x076214254ea9c44fe950aedcfc70482286cb2b8ca96d7693614e07d345c7b56d |
| Tornado Cash Depo 3  | 2024-09-10 8:34  | 100  | 1800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x5b5c37fccbe4119d70b8cccaabdb9c490a40125e0b4a62b0d73c725f48c6ee7f |
| Tornado Cash Depo 3  | 2024-09-10 8:38  | 100  | 1900    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xe842f9dc3929fda0d4b810f89d82069a646f9dd39d23736c5b0cdc767c1add68 |
| Tornado Cash Depo 3  | 2024-09-10 8:42  | 100  | 2000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x470ed3022d1c74ddcdaefab48f146bf02f62688d121781dcca5c8322930b96bc |
| Tornado Cash WD 2    | 2024-09-10 8:44  | -100 | 1900    | 0xd82a7d08bc380aead14fd39945e564625e19cc81 | 0x4f571e556366bd8d603f543aa3758e202e3977573880c231d330400ba7fa09eb |
| Tornado Cash Depo 3  | 2024-09-10 8:46  | 100  | 2000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x8adacf1d4aec79b1c2d5c2fa04d03995d5b5bad205f0c953c6185dc5b683e6e3 |
| Tornado Cash Depo 3  | 2024-09-10 8:49  | 100  | 2100    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xd13a8af4bccec04955193716ce45e0fff3291fe4160e43fd93151e29efa29af7 |
| Tornado Cash Depo 3  | 2024-09-10 8:53  | 100  | 2200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xf74b3c9340e2ec321af20966bbc2c7c3074d397db3aea10aae34cc9728f36774 |
| Tornado Cash Depo 3  | 2024-09-10 8:56  | 100  | 2300    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x193d5be06c53148bc8edbb4234e057c07fd373f915d959a8d7f04793c5762ac0 |
| Tornado Cash Depo 3  | 2024-09-10 9:00  | 100  | 2400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x822a37cb65424cc491cd4d895fd583dbeb870338107a34a7641e7289c6725bad |
| Tornado Cash Depo 3  | 2024-09-10 9:06  | 100  | 2500    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xb3bd55ab456bd13917fd091a4927040736ff67fa773fa0056c83f00a311c0aaa |
| Tornado Cash Depo 3  | 2024-09-10 9:10  | 100  | 2600    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x4f396b4be1d07d2f63a309952c4bcc64fc16a0dfc42aaa95f69a9983fb7bf2a2 |
| Tornado Cash Depo 3  | 2024-09-10 9:16  | 100  | 2700    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xae0a534f56ea5d6395d6b9072482438aaa8b5504f2efad6ce9f8d6299410f1da |
| Tornado Cash Depo 3  | 2024-09-10 9:20  | 100  | 2800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xc229a4fee9b091fe074b7d87cfb7d1312845faac2536a0329eb5aec1f347c0e9 |
| Tornado Cash Depo 3  | 2024-09-10 9:25  | 100  | 2900    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xf31472d585cfc27550f790f40abadc17dd0fdb8f864de2ea839cce812392e8be |
| Tornado Cash Depo 3  | 2024-09-10 9:30  | 100  | 3000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x7c967def716c0f0774e5837fc3d5fc70063e098798d2f7ee17970b8a6bed0cf5 |
| Tornado Cash Depo 3  | 2024-09-10 9:36  | 100  | 3100    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x272c2bff1f32c73b62a840e7cb367f24aa089d52654f032c7773b14191abb815 |
| Tornado Cash Depo 3  | 2024-09-10 9:40  | 100  | 3200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x27446ff477b88828da1fcc79fbd9665fd7f66f3ec21e7bae108a82e3f3378fe0 |
| Tornado Cash WD 2    | 2024-09-10 9:46  | -100 | 3100    | 0xa4e7e91cdf300150f36af7a04b85e37ad2ca9110 | 0x4ea437dbe680129834c5486ede09ca1f568e13f6fd9dda3feb4db54a22b37d90 |
| Tornado Cash Depo 3  | 2024-09-10 9:46  | 100  | 3200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xa8a74cef819e36076d1431c9a74fff9fdf1ea9d53a818e460f7f72231f2f9215 |
| Tornado Cash Depo 3  | 2024-09-10 9:52  | 100  | 3300    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x9445fc6d710e3bbbde1812c47ae615f201c5445a1a16c1f6996670526aba5497 |
| Tornado Cash Depo 3  | 2024-09-10 9:58  | 100  | 3400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x0aac0416888f2266b85aab8eccf867beb612b1a2eb2f679e09b698d2443c06e5 |
| Tornado Cash WD 2    | 2024-09-10 10:04 | -100 | 3300    | 0xbf0639a851683ec24e03208cd808bc4f236efab3 | 0xbe19b0f100b2547401e277641d5570ad06fa98e1bf61ce1e18bb67fa5c6c8c97 |
| Tornado Cash Depo 3  | 2024-09-10 10:33 | 100  | 3400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x291a20900043e9c22d16b85c8fb1af92f31341deab5619c97162c90c8db0d5b9 |
| Tornado Cash WD 2    | 2024-09-10 10:36 | -100 | 3300    | 0x01bfb487b7df3432ab8f67a043c795d27d9ca7ed | 0x70a211fbbc4204e2164ea0dbd5fb2865dfd8fd7a6637842b538438160730c108 |
| Tornado Cash Depo 3  | 2024-09-10 10:39 | 100  | 3400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xd21d146760f58d634d777aa8d5d787f1c349d50f22bbf393e440f5775025641a |
| Tornado Cash Depo 3  | 2024-09-10 10:54 | 100  | 3500    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x62c65061ddd10a70991fa125aa58205764cad7a66645ec6d0fd86efcb9bf6238 |
| Tornado Cash Depo 3  | 2024-09-10 10:58 | 100  | 3600    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x22b8739ddd3196c54fe15bb342e7d62ca462245e67af931bf3a6c95ca5cd1601 |
| Tornado Cash Depo 3  | 2024-09-10 11:03 | 100  | 3700    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xd6293ab13ec3c4e50cb1e33bd95e8eb51567be52db4acb07e93fae1a7edf1c87 |
| Tornado Cash Depo 3  | 2024-09-10 11:07 | 100  | 3800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x0505a4f9d1526327b6e47b962a785d90121e26e5f2f65f32946e7929bc1f7d8a |
| Tornado Cash WD 2    | 2024-09-10 11:12 | -100 | 3700    | 0xa7b8e3e226dbb65c8b05a573b86aa78b4e8bd0db | 0x3090b07a73e649223bf8c44dccd60b792a04264ce222e38a83afff395a7770c2 |
| Tornado Cash Depo 3  | 2024-09-10 11:12 | 100  | 3800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x1f6f2555ea14799e7924ac2c4ef44cf4c44e84429b8cb5aca10a6e72bfbc840d |
| Tornado Cash Depo 3  | 2024-09-10 11:17 | 100  | 3900    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x7e506f115e25a225dc71ff2c16768863e6067be5f074173b16792a3a0ded9149 |
| Tornado Cash Depo 3  | 2024-09-10 11:22 | 100  | 4000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x847223a4c4846914789353f24405dfa8026c34accf2e9805f79addb95e5583a1 |
| Tornado Cash Depo 3  | 2024-09-10 11:27 | 100  | 4100    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xb1d5fae1c089c1d0726f83316d4e32b164a048f09d404eabe7115d65234457f7 |
| Tornado Cash Depo 3  | 2024-09-10 11:32 | 100  | 4200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x332028bf2ff025b36cc9597d0829f89968dd2fd40fa3c3ef924bfe61f62872b5 |
| Tornado Cash Depo 3  | 2024-09-10 11:37 | 100  | 4300    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xf8c85996d85a12699e30be6a85a736ef2719be0c8ea13a11ce5dc1f4e84ec09b |
| Tornado Cash Depo 3  | 2024-09-10 11:41 | 100  | 4400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x8b0fab8e8a113f7bb0fcd6d6dbc43b27a3b1be1ac92ffe83c927545baeace438 |
| Tornado Cash Depo 3  | 2024-09-10 11:45 | 100  | 4500    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xc66753a6f75cad7dd3931a84e83d00f5101af5eed38de1c60ff7e91bfa821e25 |
| Tornado Cash Depo 3  | 2024-09-10 11:50 | 100  | 4600    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x6412e378e382c7e941beef8d1bf30f440f66603039aa3a20e3f7bc99d0c3b3d8 |
| Tornado Cash WD 2    | 2024-09-10 11:52 | -100 | 4500    | 0x133b283321c82a1c3a746054656d9c201f1db01f | 0xc4293b038270c6dedb28cb253750fbc159111f04d745de6596a2fa0b000b1243 |
| Tornado Cash Depo 3  | 2024-09-10 11:55 | 100  | 4600    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xe892bafae3d3eefe8cd5d71a9287c28df11a7e79b132f4ffdfbab14256cce35e |
| Tornado Cash Depo 3  | 2024-09-10 12:00 | 100  | 4700    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xfa00a5f84367c2249a90ea19057afa553eedc0817e799b3fcda90ebfdeb7b4b0 |
| Tornado Cash Depo 3  | 2024-09-10 12:05 | 100  | 4800    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x3932d91de05e7074b5d9207de7374d19a64dad5f018289eb938899f60214d281 |
| Tornado Cash Depo 3  | 2024-09-10 12:09 | 100  | 4900    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x6fd222108174d691d74d27a579081ac7de63ff0828cb6da6c8ec447a295e6736 |
| Tornado Cash Depo 3  | 2024-09-10 12:14 | 100  | 5000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x388662cc18519212fa13af773fd2e794fd367959f9d020990c8acd96db070582 |
| Tornado Cash Depo 3  | 2024-09-10 12:18 | 100  | 5100    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xfd36971404354ca10335be2218c903414f4dc2ba39a687a94c621dfda645d22b |
| Tornado Cash Depo 3  | 2024-09-10 12:22 | 100  | 5200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x71f58817aee7895ccf772a8371cbee815c9ee9cd985b587352d33e7196661923 |
| Tornado Cash WD 2    | 2024-09-10 12:25 | -100 | 5100    | 0x165bf391596303c4af98405f60d18986b4840dd7 | 0x6dc1e3966139c90085e4897a5bb4a53a774c4b3660ec2ba0151909057397ffeb |
| Tornado Cash Depo 3  | 2024-09-10 12:26 | 100  | 5200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xbb9bb3d61ce6f8a462dcdbdfc8a6396b4c1f7e1088ef505069fee7060e3073db |
| Tornado Cash Depo 3  | 2024-09-10 12:30 | 100  | 5300    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xb22ee592d2398ea325440e86578c0d31fb1af4d66102d8fb81f2720518d3490d |
| Tornado Cash Depo 3  | 2024-09-10 12:35 | 100  | 5400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xd40251531236f4d6f8fe9486ae2ae0e14d80eade352e2bc853b50c3834f89f83 |
| Tornado Cash WD 2    | 2024-09-10 12:52 | -100 | 5300    | 0xcb852a10e3991b89777191213802c73be45c62c8 | 0x42167115aebbc313a72d21e2344bb664cb7cbc9db469f6bdf3db01051ca4772a |
| Tornado Cash Depo 3  | 2024-09-10 12:54 | 100  | 5400    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0xcf4f38cc8668e2836a1c23cb4d15667abde9d30b4b77655b4a25367d9b750134 |
| Tornado Cash WD 2    | 2024-09-10 13:26 | -100 | 5300    | 0x7eb429c93e3e96f483da88f4bca700118d3a566e | 0x27c93456179e0e2f8f9c1963a7cf38015bdf58006e8960a81fbf5bac1eb1ad08 |
| Tornado Cash WD 2    | 2024-09-10 15:58 | -100 | 5200    | 0x66f71f829bf87c4ee4a0682e13500678a28ea5fc | 0xbd2d3abccb8733b9c8d1f185e4c385729886434a78b1f8f28c736c571df39ee1 |
| Tornado Cash WD 2    | 2024-09-10 16:26 | -100 | 5100    | 0x3ec7c7b09ac1ab4b84bb06d43ef89106d4e1a267 | 0x47acfe14de8a3ae5b1ef6b753406f94d8c0a73f5944f57fa3695043d67897227 |
| Tornado Cash WD 2    | 2024-09-10 16:51 | -100 | 5000    | 0x8343ce0e60fb3a33a2ec2921794c3248ce786a9d | 0x057a02a0303fe0add8c5b9ce16b9a684880a93dd28a01343ef5ab476aa6c5eb2 |
| Tornado Cash WD 2    | 2024-09-10 17:05 | -100 | 4900    | 0xa366d651b70a6f0f6a3b60816136fc473e63bfeb | 0xdcb69be4a14adb43aa8b754ffc4de8e9a3b8045f1c4a546498773d07bc68e418 |
| Tornado Cash WD 2    | 2024-09-10 17:28 | -100 | 4800    | 0xb1cc333eee1bbbbab5f53392b779880b0936655d | 0x8d4bc981c40da1a642eeb075c4b25884b3df9109de6d75f76b71862a77b2b668 |
| Tornado Cash WD 2    | 2024-09-10 17:54 | -100 | 4700    | 0x134b9566c99668d1a7bc1b51218e635bb52c7eb4 | 0x3aa816b41b74f2ff08789b92e2903de1a77200702800b8dcb29f90d6929daa2b |
| Tornado Cash WD 3    | 2024-09-11 0:30  | -100 | 4600    | 0x98361be002ec04d1427d9a96e5e7bd0d7524308c | 0xb14fdf718e3101f5914b0ac4401555edab12e31d3a13f80b62a368a2d3d08a01 |
| Tornado Cash WD 3    | 2024-09-11 0:46  | -100 | 4500    | 0x02a361d4e034d8b53312c2f0eb13fbf358f228eb | 0xe6532e5ac211a355c137db168963fe7cf839aff80aa3939defb9db2e5f659564 |
| Tornado Cash WD 3    | 2024-09-11 1:04  | -100 | 4400    | 0xf00fe1bc2b2a0eb740d2becf9afe3b7c4699841c | 0x60e0695fa6d794534db178372da1f372a11c484dce888ba934e05c33af7e3807 |
| Tornado Cash WD 3    | 2024-09-11 1:17  | -100 | 4300    | 0xfe3670c38a03be5b1c37a2c7025626311162e75b | 0xdb617cc5cf51dd5ef0a5ef6912f712d4f0adb41f56c36f1c379b088669032522 |
| Tornado Cash WD 3    | 2024-09-11 1:31  | -100 | 4200    | 0xaded2074ab127161788a1462840a3c2b01197d82 | 0x680bc5e61489d3010c01319c688f69b0d1fb48cfc38328e5970578ab64958ddb |
| Tornado Cash WD 3    | 2024-09-11 2:01  | -100 | 4100    | 0x450f630ac36182134de522c53ae939b4f1c4b944 | 0xb8b70f67664ebff421eac96efc8acafe00879c788cccd0563be1f62ace202373 |
| Tornado Cash WD 3    | 2024-09-11 2:24  | -100 | 4000    | 0x9bbc58c80c06bd343d939ea62a60e1f479353abe | 0xca229e34d6c0d3553d0826f9915f722306e770b58a318456f875d343300bf6f9 |
| Tornado Cash WD 3    | 2024-09-11 2:44  | -100 | 3900    | 0x5c95e7ea22d4abc75f583ba7dc1242145622e627 | 0x82145ffdf8384be8bc26b4173403601cd227a11ae4531b547075a9a059588cbe |
| Tornado Cash WD 3    | 2024-09-11 2:58  | -100 | 3800    | 0xbef2be04e025261242480100688147c984d2e74d | 0x9dd8eda712f6fb1686f995965b3385a668ce205de2585f5a15d9a03854a0917a |
| Tornado Cash WD 3    | 2024-09-11 3:22  | -100 | 3700    | 0x4e7c398e241a1f60ec8d0258cdfa128335b6b2bc | 0xd37729ca977390812e2bd8cf88cf2eb9593381dda334dc664fe07081af402e0a |
| Tornado Cash WD 3    | 2024-09-11 3:39  | -100 | 3600    | 0xd358f1e1dec7fb7b011c7c4ca59249200c3ae737 | 0x258ca0755ac5343c681cca5235c6456997f01f4fa534ba5ebd1c064cf87b9077 |
| Tornado Cash WD 3    | 2024-09-11 3:54  | -100 | 3500    | 0x93f1676e9cfe9a3a64e3317ce2f69c8723b72487 | 0x72b5e98bbcfc6008abb15271fafca6dc84858dcce62079e52513157363d6ea52 |
| Tornado Cash WD 3    | 2024-09-11 4:19  | -100 | 3400    | 0x96693a48fcee6379007d3e1729c41e9f7117c690 | 0x9724e6bec6493e0536b88dcdb14802768d0b4b930a83c2c01ff72c2883b46969 |
| Tornado Cash WD 3    | 2024-09-11 4:34  | -100 | 3300    | 0x864842becd6a98e01e02f848a063794b25d25ab8 | 0xcbda323f7f664844de6937665e2c9e8744b0d571e31325da3feb23c123ff97d6 |
| Tornado Cash WD 3    | 2024-09-11 6:38  | -100 | 3200    | 0x8bc37ed3d8dcc016fc5950dc17e4589ada2b2e18 | 0xf6c2b07ba4d054659be997fcf0ad18caaeae6487c880bde8c1c78f72b1213851 |
| Tornado Cash WD 3    | 2024-09-11 6:53  | -100 | 3100    | 0x408aa9ee85f95c02bbb331a312d83cdefb00b9a1 | 0x591ecb6affa98a5effd4cd012e942991c014631d66b20768e6b723e56bc7c3b7 |
| Tornado Cash WD 3    | 2024-09-11 7:07  | -100 | 3000    | 0xb6388e990d50c3c032d8019bd8a90007e9a1a36a | 0xf5d67a28132aa9b67373c0c11f139d8b942afdbbe3d68d8ef443afe3bd22cc0f |
| Tornado Cash WD 3    | 2024-09-11 7:25  | -100 | 2900    | 0xe8dcd7c2be9dfd1c2a6b3e9e302ac682e6326426 | 0xc33a03ffce1932fd83563e162097a121c418c1ce3c9f39d5ab95a3713c96e6fe |
| Tornado Cash WD 3    | 2024-09-11 7:46  | -100 | 2800    | 0xd311677adee212b5463c130646735f81ccc48565 | 0x1f1a6589d06a9f90d7906c7f4cc52df99a95e40bf0c815bef87649be56ac963c |
| Tornado Cash WD 3    | 2024-09-11 8:05  | -100 | 2700    | 0x498ea5d733f7b90e7f3e7c4a48962a6ca552155f | 0xbcba3b808affb3eb331d0bed8e7b9e3f22d3ed8897424cef3c4de887904ac649 |
| Tornado Cash WD 3    | 2024-09-11 8:20  | -100 | 2600    | 0x9d9651cdd1356186f6b2972a50651f7b4fabdcbe | 0x257dc0101c4ac7c7ce749ebe91a9ab11bbbb7d547cd09fa600ccc26f01fb4ca1 |
| Tornado Cash WD 3    | 2024-09-11 11:29 | -100 | 2500    | 0x931ba5bfaf484f099773e20f1a3945cee6867cb5 | 0xe25ea5e1e99d95c8542cfd563895b4338196e0e63b872a3c42ca97a4d80d72d6 |
| Tornado Cash WD 3    | 2024-09-11 11:38 | -100 | 2400    | 0x3272eb3446b9a8984aa8239c4b483a45741e32e6 | 0x57fd1c2bbe6def7ce633a5a1a9ee88662d142fb6a50b88a295433845c4faa9e4 |
| Tornado Cash WD 3    | 2024-09-11 11:58 | -100 | 2300    | 0x4b13c0f61f533a9f6321ce8917f702e178eeb561 | 0xdb160bb0a3427b3af171e55c45e26948d33d8c48ae4b79e58f2271074cb57a7a |
| Tornado Cash WD 3    | 2024-09-11 12:19 | -100 | 2200    | 0xb8a3badbb2319df7e6b5aa9893905354d17ca80f | 0xb39cc5d3758fff74a77f6d407e228f852fc72e3df7ea9ee6e67a495c956831b8 |
| Tornado Cash WD 3    | 2024-09-11 12:30 | -100 | 2100    | 0x1553928f7b560d9387c125a4f926cd33783472d2 | 0xc454300f66b8df61fb91a4bea3c35eff8552d8b87c9e22bd46058280162ce215 |
| Tornado Cash WD 3    | 2024-09-11 12:49 | -100 | 2000    | 0xf15aa5931236daa5fc0266e123c068e663cebee7 | 0x194cbb0fbf78ee007d35cd62d93172f872824acb2cda66ef5d55c3630342434e |
| Tornado Cash WD 3    | 2024-09-11 13:06 | -100 | 1900    | 0xd4515815ea9dcf6bb74c759fdc1a19c337c00678 | 0xe8b9dc00c858e69ae909b3f4edaf562cdc7354eab6002da8121d858fc885298b |
| Tornado Cash Depo 3  | 2024-09-11 13:17 | 100  | 2000    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x4bb60cdc198df3b6a120d4980a10098aee2ee426d71890afe66b51cd61f80b51 |
| Tornado Cash Depo 3  | 2024-09-11 13:21 | 100  | 2100    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x31f0b7e55d1d3b779c8da175d74bcf82decd7109a1bf1c7d314c7c2dd4dddf85 |
| Tornado Cash Depo 3  | 2024-09-11 13:25 | 100  | 2200    | 0x7d256f71507e7c7fea337e8518e2bd8f3cf8d30b | 0x0e67112c0f6324aff86f893e0b42e0157db18d9114f3ca40404ebd12d6f19654 |
| Tornado Cash WD 3    | 2024-09-11 13:25 | -100 | 2100    | 0xb26d02c22317e564e1f6f8e1812c85671ac2d001 | 0x9bb44f5bd2281100b97319f4c40a45ffb2031a77e765e03bd791c29a337dd7b9 |
| Tornado Cash WD 3    | 2024-09-11 13:39 | -100 | 2000    | 0x90129d4d9113e479c11097c487a5f06e07374ba6 | 0x8da3488f26c65102782953d793f9809fc1f116016f28146dbfe503f29a4b5619 |
| Tornado Cash WD 3    | 2024-09-11 13:46 | -100 | 1900    | 0x04e5094ede06dc3476fb923c67969b9e3e18596e | 0xe51ea2e69074cd3add22c069d20268e13485def1dda3db07159c0a150e043f85 |
| Tornado Cash WD 3    | 2024-09-11 14:14 | -100 | 1800    | 0x32283fe3acfdb027ccde9d614c9e6a6b775d0c67 | 0x58fc9144463fd8d562d8161d4e5fa857ef4c63ae829e3d17a4e99ea44dabb008 |
| Tornado Cash WD 3    | 2024-09-11 14:33 | -100 | 1700    | 0xbffd28e2a22a4ee0043a68098a97e10fef2bdeb0 | 0xb5e64b353296f8012815979fa14df8ff0d8ed04b1e2f9214b3c907d55318f55e |
| Tornado Cash WD 3    | 2024-09-11 14:59 | -100 | 1600    | 0xc523978a0e55a996c86b6e5b7f517cf65dbecbab | 0x06ba66440e1f5e530dd882e5fa4843d5aa6b96867692ccd501fd820a4ad44fe6 |
| Tornado Cash WD 3    | 2024-09-11 15:16 | -100 | 1500    | 0xfa1474ef330fe904502b896d30d22518f6b2b2a5 | 0xd5e4924027a99308544a65ba22f473520cce6e09adf32b237e7b73378a664ea7 |
| Tornado Cash WD 3    | 2024-09-11 15:29 | -100 | 1400    | 0x758f61d47c0da622f459f0d5b1ac365a9e8fa4ee | 0xaa3d34eb0bbefd6be6acbdc86d0318f05c6545b66286b4946ebd49d08f855a2e |
| Tornado Cash WD 3    | 2024-09-11 15:35 | -100 | 1300    | 0x83f704875716ca84e5e395cd93eaef7fdd2661ec | 0x9e84532b997a2023ff342797191c8311577bf3a08cb84c0576f163c8fcbca713 |
| Tornado Cash WD 3    | 2024-09-11 16:47 | -100 | 1200    | 0xcb3157cf14182df30a7fcd15a4908eabbc3dd468 | 0xe1c9a2a34dcdc854131229e239c17f4a4009e613ddbc82b83aa1ec330a10d5b9 |
| Tornado Cash WD 3    | 2024-09-11 18:16 | -100 | 1100    | 0x931ead27ef05d66974053d805ed273bdc63028e2 | 0xdce97952d3b6876492310f320f1931aba5898f76691005f93535e15b7d41f197 |
| Tornado Cash WD 3    | 2024-09-11 20:12 | -100 | 1000    | 0x6611075126ccfd00904b3559e6bd371baaf5e649 | 0x97caa4e4e89928844aa75217297c08e74ef72c67838bdeb073d0ae7d1d0c0333 |
| Tornado Cash WD 3    | 2024-09-11 21:40 | -100 | 900     | 0x91d07f4883708f109e6090729a1026d9d76f5d25 | 0x004f853627d31a26f9060e031145deb518e1fcf8323551f4f6ad831e7cdea74c |
| Tornado Cash WD 3    | 2024-09-11 22:48 | -100 | 800     | 0x90970edfbc1e69261d9fdc22e57d1f522319cf78 | 0x420a7182ee25b633969fade54301ba1a42f5f58d400aa76d80238e6e6c8adde6 |
| Tornado Cash WD 3    | 2024-09-12 0:00  | -100 | 700     | 0xf916c0d2db4a71c71417d36a9c6b543d7a3a44ee | 0x837e1a83c3a05bbdce2ae6aaa7ee2ac247b12cfa57e8c56d14976736eeb55b62 |
| Tornado Cash Depo 4  | 2024-09-12 4:11  | 100  | 800     | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xb7c9d3d0d64b77406f25ef21b7bfa0d916aa338d52cc2430abb7e1be11bbd554 |
| Tornado Cash Depo 4  | 2024-09-12 4:16  | 100  | 900     | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xcbe2e96df8be54dfb19f98e0a37b5e2db9788c0e310faf1f08aef6b5d8d6d7f1 |
| Tornado Cash Depo 4  | 2024-09-12 4:19  | 100  | 1000    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x1856aba1ced4358a2736bc213f173eeda9e84e92d586085d3db701a875560f68 |
| Tornado Cash Depo 4  | 2024-09-12 4:23  | 100  | 1100    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xa155ef0d1d88308c0008c14590842b657dff9d71e294a02a21a37fb69c721068 |
| Tornado Cash Depo 4  | 2024-09-12 4:27  | 100  | 1200    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x7c369db5cf67bab81b829b17eb49d83a9da2de8edfa18a4a17166f1a0ffb9706 |
| Tornado Cash Depo 4  | 2024-09-12 4:29  | 100  | 1300    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xa29dccee04c40991eeb2906961445ec0a00a892e28e0c018aa38b924224dc7fd |
| Tornado Cash Depo 4  | 2024-09-12 4:33  | 100  | 1400    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x9e8d6b9f67e04ca35247b1dec230dfaa2e3c6231bd36fa1e58128ae5cebd1517 |
| Tornado Cash Depo 4  | 2024-09-12 4:35  | 100  | 1500    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xc51c79ecb04b54d92b6bfc6373bbf29ec0c9aab98252d51eccf68db357f372eb |
| Tornado Cash Depo 4  | 2024-09-12 4:38  | 100  | 1600    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xea63c024dac139e6c50e9781062ba3158962e3ff3782c2ce2f0296aec7fd3a28 |
| Tornado Cash Depo 4  | 2024-09-12 4:40  | 100  | 1700    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xc9882f7a0904cd28af0a54a5b54606b298a9356791253f6f35b35ac7921c4cb3 |
| Tornado Cash Depo 4  | 2024-09-12 4:44  | 100  | 1800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xca85d115491c56cd4e95cce63b7eddb94dd3b043b50db45f6878f85b102b54ca |
| Tornado Cash Depo 4  | 2024-09-12 4:47  | 100  | 1900    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x5119584a77897798e65261721fb31a3b16d230373b19abfefb6480cbcfa66e10 |
| Tornado Cash Depo 4  | 2024-09-12 4:50  | 100  | 2000    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x4a710ff43a6fdb1e5e73fd1e8db987b988b97bff55f46cd141416bd6769fd454 |
| Tornado Cash Depo 4  | 2024-09-12 4:53  | 100  | 2100    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x7faf97b0f9d3b7cfdde543f4737c859a276706db9048ec368fe3ac26c0572013 |
| Tornado Cash Depo 4  | 2024-09-12 4:56  | 100  | 2200    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x1ef28d433716cecc3381300beef95d815cc4bb523dd318d25cd384e74bc444e9 |
| Tornado Cash Depo 4  | 2024-09-12 4:58  | 100  | 2300    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x13ed8be839b4fb887ba9c5cfca1131532b00f0f79cd413961fac5e131e395473 |
| Tornado Cash Depo 4  | 2024-09-12 5:01  | 100  | 2400    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xf07c261b49f129dd947e13627ec7f8b83b3330ccef1cbc3b758c18829bdcfabc |
| Tornado Cash Depo 4  | 2024-09-12 5:04  | 100  | 2500    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x3b5beb91fe294ad5d1c3cbbe57bc5a94fa58c757569fea24fe2528136d9a61a3 |
| Tornado Cash Depo 4  | 2024-09-12 5:08  | 100  | 2600    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x7e33eddceb94258db13f0b5e67e2df28fa0cd8f950f968c9b1bb883aba80b29a |
| Tornado Cash Depo 4  | 2024-09-12 5:13  | 100  | 2700    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x00be54e8cc969e081407f18b56b9840851cf561d19b3277bbce8cb0c0a1b9f9f |
| Tornado Cash Depo 4  | 2024-09-12 6:14  | 100  | 2800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x522b3eac608159713b32c87848daae8aa510bc9053219b3c2d6beb6e388c293e |
| Tornado Cash WD 3    | 2024-09-12 6:17  | -100 | 2700    | 0xdf23d1894f2a7060e7e7c55f46854c363f77e7f8 | 0xf07b6c28b4d13ceb6c0bada59b22805cb5576c8845d07fa0492b7cd18da28dcc |
| Tornado Cash Depo 4  | 2024-09-12 6:17  | 100  | 2800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xf2e5510fe0a7bf948cc9953dac5f3abb588553e9b5ed13e62be2226993bfbb13 |
| Tornado Cash Depo 4  | 2024-09-12 6:20  | 100  | 2900    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xd654b109f851f70eb4cd1977baf26c9f590245f8ceeb955d28191095fa30eca8 |
| Tornado Cash Depo 4  | 2024-09-12 6:23  | 100  | 3000    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xd925081ef0d4b301196fe5af59ba402ff4dcb63f8d192ddc5288e9b373cbfd1f |
| Tornado Cash Depo 4  | 2024-09-12 6:25  | 100  | 3100    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x1e3b7c1753a7905e945f461acbb90263b07c0d082f919f51a40b06181587cd97 |
| Tornado Cash Depo 4  | 2024-09-12 6:28  | 100  | 3200    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x4914dc57f2f3edb43e28358243f7cd7994c8ad2c2683a941502da111fdd90807 |
| Tornado Cash Depo 4  | 2024-09-12 6:31  | 100  | 3300    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x7f1407cda25b33a6e05d4e92855e4b1f0e8c8bfecb535b2234db50610ecec605 |
| Tornado Cash Depo 4  | 2024-09-12 6:34  | 100  | 3400    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xb928deae989c45104df247fe4a0915055dcd5eee8e49f8fc6884a4cd26a39101 |
| Tornado Cash WD 3    | 2024-09-12 6:36  | -100 | 3300    | 0xebfe3c5c6cc4167d85b56f155bc62b1ebd5951a7 | 0x3e5dbbaa44d3305e3480505a5dcb91d84c164774f9377c74fd353df8580be229 |
| Tornado Cash Depo 4  | 2024-09-12 6:38  | 100  | 3400    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x9a8771c5604b742fa2f0442bcf08692deaa75091b0c4b3f0970ec22669a82b16 |
| Tornado Cash Depo 4  | 2024-09-12 6:42  | 100  | 3500    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x91887e1fd88d872ddf7dcb426b76c1b2b9bd5466480876cbdc93d872987538f5 |
| Tornado Cash Depo 4  | 2024-09-12 6:45  | 100  | 3600    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x527463e524e303ceeb0bc6fd59a527469a99516628e1d80e0acf8e6063e39e75 |
| Tornado Cash Depo 4  | 2024-09-12 6:49  | 100  | 3700    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xf3c3610ac5869ad0b1efcebb148d1b3c519621e186a56a5b645619c00dc26d87 |
| Tornado Cash Depo 4  | 2024-09-12 6:53  | 100  | 3800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x96a884e0fce9335de6a7fcdba82516f027f91aa36e44dd2b3343c527d7a9bce3 |
| Tornado Cash Depo 4  | 2024-09-12 6:56  | 100  | 3900    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x5f65a4239b430153d486805b7c0df920d7358f0e0ebaecaa3c253b54b91480b1 |
| Tornado Cash Depo 4  | 2024-09-12 6:57  | 100  | 4000    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x8dcdf90920bbbc1a7af42cfe20fcf55e0270a2895106d947483e37050cfa4e6a |
| Tornado Cash Depo 4  | 2024-09-12 6:57  | 100  | 4100    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xadec1b7488a54f3489269ae5238e7a0e3945e08d2f89c82479d39cb6a22f3c46 |
| Tornado Cash Depo 4  | 2024-09-12 6:58  | 100  | 4200    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x3bfba4064b3e4fb004b62c952128e8a3ada264bfd9df86598a296c0b4e25c128 |
| Tornado Cash Depo 4  | 2024-09-12 6:59  | 100  | 4300    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xcd02097f0e0d63caff34e1f3506b5d32d6ce656b9977b0b882b84e07c015c020 |
| Tornado Cash Depo 4  | 2024-09-12 7:00  | 100  | 4400    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x3b585ca7d3227ced320bfcddc70e30d8d93d9a0aa4ebe676c6c5b6ebc50c27c7 |
| Tornado Cash Depo 4  | 2024-09-12 7:01  | 100  | 4500    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xffc47f923aeff9dfda9ea207167ac5faf959d22b2b08198be573193b8409fa87 |
| Tornado Cash Depo 4  | 2024-09-12 7:03  | 100  | 4600    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x28e37237f945f624c11a403754efbfaec1f114eb3efe76e8e7e3a8ff0424522d |
| Tornado Cash WD 3    | 2024-09-12 7:04  | -100 | 4500    | 0x00e653d217ef6fd11e7a17176ec755f8936ebc6c | 0xe76bf52f4fe4c6569120f93b089fd6600e113d6d57ec1dcd0407a167f9662b5b |
| Tornado Cash Depo 4  | 2024-09-12 7:04  | 100  | 4600    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x5a4acd86f905e11441fc905ad8d8f25584441c08eaa431ff0275e337a2b9c10a |
| Tornado Cash Depo 4  | 2024-09-12 7:06  | 100  | 4700    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x1fe037a9ab2821382dca0a5be1e6092b2cc58bcae6068132cbcff2214c669a68 |
| Tornado Cash Depo 4  | 2024-09-12 7:08  | 100  | 4800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x2aaffe55496076578a10b34eb823d81e735fbf40c702807d16d5ba1a75456c0b |
| Tornado Cash WD 3    | 2024-09-12 7:11  | -100 | 4700    | 0x8157d31fd7381494da1497af4621b9ff8160cbd1 | 0xe949273ec0fb5c7fc837b0cc14522421362b7f10107f3f9fafba02c8e67df172 |
| Tornado Cash Depo 4  | 2024-09-12 7:11  | 100  | 4800    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0xe32f5d7d9460b324f8dbb29d5ff8de8589bce7d84105086023f5ed00b5277e80 |
| Tornado Cash Depo 4  | 2024-09-12 7:14  | 100  | 4900    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x5e53603dfd79e9511ef106b2ef22a41eef20783f6b6184f7fe7e3538db793996 |
| Tornado Cash Depo 4  | 2024-09-12 7:15  | 100  | 5000    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x274dee689f3730db5e1d5d4602aef03d5c4d9811abdb5a30ac1235d33a7607ab |
| Tornado Cash Depo 4  | 2024-09-12 7:17  | 100  | 5100    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x896b6c6c10d975419b44ca96b6404dd67b9409afc3f3aeed3971eb26f4b6717a |
| Tornado Cash Depo 4  | 2024-09-12 7:20  | 100  | 5200    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x29a41377fcd7c72783644be94cebf7d216fcadceb61b242124bffcda7155febd |
| Tornado Cash Depo 4  | 2024-09-12 7:22  | 100  | 5300    | 0x5fe287e153c77c215d98a0b07eef67fe65f0ac19 | 0x745319ad30c0ac5c4177a73453b92b0135caae07c050289e899d216899c1b6b0 |
| Tornado Cash WD 3    | 2024-09-12 7:23  | -100 | 5200    | 0x879ecd03ae2859779c18ab5e6d7321542f14262f | 0xdbb11cf063176a99f9eccaac5dbd0d40f93743b8e077ff4eede81fe204459456 |
| Tornado Cash WD 3    | 2024-09-12 8:00  | -100 | 5100    | 0x98feb989a8f4f9aa1a3ad1907dae9097304d3196 | 0x3acb52fa987abeadf90b63f21cb6f207902ce0b33f8e6cae0b100087026a9fe1 |
| Tornado Cash WD 3    | 2024-09-12 8:10  | -100 | 5000    | 0x94ad34a0ae6cd4f9b84358b675e761398063c29d | 0x9186061a4bab43bb23452a76788cf041e71c3077e138f818d9211318b5c47182 |
| Tornado Cash WD 4    | 2024-09-12 8:35  | -100 | 4900    | 0x61af6e4169b31bd2702463cbdc9b3dcea8bc6b4e | 0x54665fb769a5379bbcf6eb0b15d6c8e4d28914b25e5b384f366fa19f79b25c9b |
| Tornado Cash WD 4    | 2024-09-12 8:59  | -100 | 4800    | 0x1d4514c55683dcef92f5d876054b86a9a9782004 | 0x0c3a6d54348ccb23af6390d591a333c09f07ffb7d93adaa56900e729a6543e59 |
| Tornado Cash WD 4    | 2024-09-12 9:07  | -100 | 4700    | 0x81eb54d4526f4eeedd96899a0f88e16bcaa6d037 | 0xa4f90afde641bbda2443c610108d6f79e3163982b7ca119bfca8697eef46c589 |
| Tornado Cash WD 4    | 2024-09-12 9:37  | -100 | 4600    | 0xc42b10b808a25f002bba1dd385bb3430b53aa2c0 | 0xa16c36febcafe5979c1add3b334027f96068e2e8270f479b03aaf3d5a765c4fc |
| Tornado Cash WD 4    | 2024-09-12 10:14 | -100 | 4500    | 0x585aef5668bfb37e2a38d3d2fed0efeefcdb8ebe | 0x75e59c22e501782a78c6c70c82b32fe275afd1d59a4dabf3ee7088404b2235a1 |
| Tornado Cash WD 4    | 2024-09-12 10:39 | -100 | 4400    | 0xe17a6287f8c04734ed8fc3f504300c44168f11ab | 0xf2ef2e49f03b5a6c2d47ebc71089f73df810b31baf765f4f10a64e1f8aff84e1 |
| Tornado Cash WD 4    | 2024-09-12 10:57 | -100 | 4300    | 0x820b6f9130576491bf88256bc141b759294c5fba | 0x484326f51434da47af96020ecc7d987724c168beaa8aa0b875509cea815e447a |
| Tornado Cash WD 4    | 2024-09-12 11:23 | -100 | 4200    | 0x3607fb35f46adc43119eb7ef94681d0cdb07c4cc | 0x9f0e3afae89ae86a5b50e4fe1420b12bec76b6dcfacec535ff880118fcb00fc8 |
| Tornado Cash WD 4    | 2024-09-12 13:05 | -100 | 4100    | 0x5e7acd7b878383ef6bd17c17a776e5e6ccf625c7 | 0xfdac292a3cb94fddf8a8ecc330cf4b1dbe9223ee9f9f0280d6c7911b271603a8 |
| Tornado Cash WD 4    | 2024-09-12 13:16 | -100 | 4000    | 0x045f9b38337c102163712d128a444a0d11363bf2 | 0x76fcca3045ce1599afae754b73b3b42eb0444f3aa52e4ebd5425a2e896c44da1 |
| Tornado Cash WD 4    | 2024-09-12 13:27 | -100 | 3900    | 0x7d89644f66c3afa7093045c84720141b0c997ec0 | 0x66c89a7b61941197851279dcefcff89c0b77a4a4d33298cc10b0872dab981369 |
| Tornado Cash WD 4    | 2024-09-12 13:47 | -100 | 3800    | 0x81c568ccb3d9ef50c2d297e4c5fde77b4893508b | 0xca86acc2f5a4a68061ec78343a837d9b664f81b867a68d8b41df6dc520b7cd61 |
| Tornado Cash WD 4    | 2024-09-12 14:06 | -100 | 3700    | 0xfc9d1072c1f7108084a8a9b19176e316166f38da | 0xdf44ffc353d921cbe56303a888eb7f52492fabe65fd03765ac086fe7c9e31f60 |
| Tornado Cash WD 4    | 2024-09-12 14:29 | -100 | 3600    | 0xcf26ab4cd9458a46e9d0c4b4267a61485ecfe6e8 | 0x22973fd018ab8a3efbcfef9b2eb5a71a80bc8f1c674a0add4ce9e0192683ea14 |
| Tornado Cash WD 4    | 2024-09-12 14:40 | -100 | 3500    | 0x22bc4428c3437babdf0c4cdd60b5ed6a161c4f0e | 0x352e5bafd7000cd071ab45a83566132f2199a9617d7aea1e7859df540e946b6a |
| Tornado Cash WD 4    | 2024-09-12 14:59 | -100 | 3400    | 0xc34c05b0847291536b78cf4905d38b82d08be4d0 | 0x50a15f32ecf1fca0af8728ee498d4cf7f60cc7254c3e8c842e24378b72ceb7d1 |
| Tornado Cash WD 4    | 2024-09-12 15:18 | -100 | 3300    | 0xb942750bc00aa9266812a1582321017f45d033b2 | 0x8f67dd87b786771e38b2c5ee96bad69744c06270bd6a7aec18b63848b63e8800 |
| Tornado Cash WD 4    | 2024-09-12 15:28 | -100 | 3200    | 0x4e379c0c094887c363c31cd98d427368bc667e40 | 0x922e60e8899171a813106af727e496f68faa8438a097c1c2b175a49a649f9d5c |
| Tornado Cash WD 4    | 2024-09-12 15:51 | -100 | 3100    | 0x0a77efe1cd8923bbb01349974d3d7072c08a3142 | 0xacd89c85e6ac9aeb5f2eac719b165567c20d5891084ddbe340b8de8a5813ae87 |
| Tornado Cash WD 4    | 2024-09-12 16:09 | -100 | 3000    | 0x9f027cfc838cf895a5ec9c91fcb90930910db613 | 0x8ff24298d189c149b7853f923e271a3cba62ee4b53f92a328c88d7aab830420c |
| Tornado Cash WD 4    | 2024-09-12 16:20 | -100 | 2900    | 0x08af33a05596ea07763cd358cb51b99e54baeaf3 | 0x92438a784359e3c48dc0101a07ad60dec80b34e5f50ee80e47c74ad80dbf4627 |
| Tornado Cash WD 4    | 2024-09-12 16:27 | -100 | 2800    | 0x04fc58dade16f459a79da6095e37970c708c3ecb | 0x7dfe6e34c52e1113160d46e33d7842f2b70f331ca0286907f68d3ca609c79a5d |
| Tornado Cash WD 4    | 2024-09-12 16:47 | -100 | 2700    | 0x496a2c91dcd2ab1222b0fffc65886595e579ea25 | 0x04276a7ca5f4badbb526a9ae15b5dac74045f964f03b0bc080bd528fcbde98d7 |
| Tornado Cash WD 4    | 2024-09-12 16:55 | -100 | 2600    | 0x9067dfbd5641ff48cbec2ff7f95bc521ba214d55 | 0x4dec79db30780cc9ae60299d24de71bdd7cc1e056448fc49cef41221308516e7 |
| Tornado Cash WD 4    | 2024-09-12 17:19 | -100 | 2500    | 0xa8a83da7852195b933f89570a4ac8e4726ba8255 | 0x248152e2cab1006c79fff671e7d80abae097eb3e82aaab84ca0e37cf3ee133a4 |
| Tornado Cash WD 4    | 2024-09-12 17:27 | -100 | 2400    | 0xe106243e6b6c611e3b3f7a83065ecb8614b09349 | 0xce8e492b7a392fce2ae3dbbf7b24c32142f82aee8a55c232eb3c81facc2d3e32 |
| Tornado Cash WD 4    | 2024-09-12 17:53 | -100 | 2300    | 0x57e809d2e613afe36484f049721d8bdda23f045b | 0xcf9438ee47b7d35e3afd6c8a5106992440ac217b814e5cfa3da97e2ec9e54c11 |
| Tornado Cash WD 4    | 2024-09-12 23:55 | -100 | 2200    | 0xf3bd33da885892ee67b0af4a80f59286b48a5ee6 | 0x4495c97d82452f1292cc2361baa388e79cd5df83197568be2ab943aae738b5a7 |
| Tornado Cash WD 4    | 2024-09-13 0:01  | -100 | 2100    | 0x308b4996b14c79de23f70a1d26cd7c3bfa54c478 | 0xa0840d16370ecbbd1f4abe8abaa263133e88e5a7678321addbf981c924f7f4dc |
| Tornado Cash WD 4    | 2024-09-13 0:10  | -100 | 2000    | 0xaff59f83ac1a70d68ff4f0b5e92a3b1d7d6c341b | 0xb1101ebd6348c3865dedbcadc8d1333c245c85e06496f325ca31e64e2921663d |
| Tornado Cash WD 4    | 2024-09-13 0:33  | -100 | 1900    | 0x801c44fb116c4ee476c5d6a7f041dcdd581dbc0f | 0x8c31d033a4e043fe2b824d3d8eac345a76fca1137231b0f82412d6fc06649fbb |
| Tornado Cash WD 4    | 2024-09-13 0:49  | -100 | 1800    | 0xef3c4fc0b0036090c75acd5be94176d002c1ef52 | 0x3647bf638f452382604f05395dc2ad2199e27881b3b08879c9f7c34aee0af4d1 |
| Tornado Cash WD 4    | 2024-09-13 1:04  | -100 | 1700    | 0xdb5c146441f08603ac3a15b5021b3bc6af32cea6 | 0x5662dc49fd9fde269524f438b1833a421c48f29fb0fc5d05fce893f383fce3c3 |
| Tornado Cash WD 4    | 2024-09-13 1:15  | -100 | 1600    | 0x8449cf36c28c7bfc82f05e471c0c472505752025 | 0xd1aa4c7e37064c4137ddc5cf92096b9279fc1522509d649e419607f298e57095 |
| Tornado Cash WD 4    | 2024-09-13 1:20  | -100 | 1500    | 0xed0dc7eb3e9ff019bf18a5edfbafd4a832a73c53 | 0xdfec75ad1fd3258338896589fdcd8b045a5a9aadeed661886bee4f179b93734b |
| Tornado Cash WD 4    | 2024-09-13 1:37  | -100 | 1400    | 0x04f859e6a721ef55170617532158d6db2f2d07a5 | 0xe6e104156c92e8fa4b1646222aa8e7bf24c51da673bc7ad6e4a8dc3f28fc9091 |
| Tornado Cash WD 4    | 2024-09-13 1:58  | -100 | 1300    | 0x8fc5c8147b8db102c4063484ff85e19b5c0cb90b | 0x89ee796251ec04a7fc5005dd16e5ccbe43d69799ee3cfe209bed94588ef44ae7 |
| Tornado Cash WD 4    | 2024-09-13 2:02  | -100 | 1200    | 0x8b1970558a1d7970e69eb5fbcfb977e9b6c0944f | 0xd5e9026126a6f0f00f6774ac2bc7c79c4400d94ccbf7775544141a9324b9c6a6 |
| Tornado Cash WD 4    | 2024-09-13 2:10  | -100 | 1100    | 0x38fb97f8049cf178262febb0c116291e262fa55b | 0x9da646e4ec3f2115c07d0d2936624be5f186199e67f08b635f0cb15a2e751a8e |
| Tornado Cash WD 4    | 2024-09-13 2:28  | -100 | 1000    | 0xfb3c5afed463534d25c7d6e08c72f7ad808a00b9 | 0x1e956dbf5523c775ed4ea981ef00e840a88bb9b7a51eeee5a135c43f487556fb |
| Tornado Cash WD 4    | 2024-09-13 2:53  | -100 | 900     | 0x1efd569bd88b083f144e0f02333e18ded2d9950e | 0x7edd32cf54244d1d5598ef45e16125729451aab672f7938d94b55c50ac7cc5da |
| Tornado Cash WD 4    | 2024-09-13 3:10  | -100 | 800     | 0x7b6837fa6bd52fb8502ab84765bfc38e2b53e2e2 | 0x96a3187f9fea54eaf70237fc322b4efd298319dde6d8728364a7c02d5a583b05 |
| Tornado Cash Depo 5  | 2024-09-13 4:03  | 100  | 900     | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xa4393df69d16b110297d2eaaabea23c1345073c9cb69cfcc0d9bb8a71f24e9c1 |
| Tornado Cash Depo 5  | 2024-09-13 4:03  | 100  | 1000    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x726432699987c9864d444ed19cda844711ee07d6e6b14ef5695811dca8db6e6c |
| Tornado Cash Depo 5  | 2024-09-13 4:04  | 100  | 1100    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xc62d9daaf69423686a93fcbcfaeadf7b6815877e755624b60e64ea106f034612 |
| Tornado Cash Depo 5  | 2024-09-13 4:04  | 100  | 1200    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xb1045a70ecc7c5c486e6f0611a64ab3a965a6a1285b018456617294dda2518da |
| Tornado Cash Depo 5  | 2024-09-13 4:05  | 100  | 1300    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x3eb84cc1cafb59bcc87ab06bc982ffc5101fda94658ec94f53df1bf2667591a0 |
| Tornado Cash Depo 5  | 2024-09-13 4:06  | 100  | 1400    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xf1bd78475d4afa2f84eaa2641233c1d4c495dfd9353283b09c4eec79f4273aac |
| Tornado Cash Depo 5  | 2024-09-13 4:06  | 100  | 1500    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x9c9545b2c012876446392719ef23a9953fe50c4364b9a8432ee0326096422f1c |
| Tornado Cash Depo 5  | 2024-09-13 4:07  | 100  | 1600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x0bc698c301e7e519ecbe6813105bf9aa7293b5b9a2150a72a00ad91d25203a54 |
| Tornado Cash Depo 5  | 2024-09-13 4:08  | 100  | 1700    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x4860b5e1da35afc080b802c58a0ea5be486b2d2d897332f6a7f191176644a855 |
| Tornado Cash Depo 5  | 2024-09-13 4:08  | 100  | 1800    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x5f8f4d94683525411a345e11cfd202c975f403be79548ed8a8658b94f6aec02a |
| Tornado Cash Depo 5  | 2024-09-13 4:09  | 100  | 1900    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x0db61188e449102d65a8465c54e3d7b626a7b4d6ad324044b862c6ee79b5f552 |
| Tornado Cash Depo 5  | 2024-09-13 4:09  | 100  | 2000    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x1252469536d01114e1163f378607e315fcaf4bdb3a105d4eff17b093b846be99 |
| Tornado Cash Depo 5  | 2024-09-13 4:11  | 100  | 2100    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xbae8e59a44467b699ef4e1594e9333c5939a9c1b3c970db5a373340358e09878 |
| Tornado Cash Depo 5  | 2024-09-13 4:12  | 100  | 2200    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x359e1dcb8867e30b623f85791aa8fe2cc88bb45bb2c2d7bc929e5865e3aac5ce |
| Tornado Cash Depo 5  | 2024-09-13 4:13  | 100  | 2300    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x803f96b3b5c2dc06d73e2d02c7d93e0c0dd5a38ad1e75e5c2c57b2320613e3ef |
| Tornado Cash Depo 5  | 2024-09-13 4:14  | 100  | 2400    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xc9d1d531387074d43b8c69dc07a797e86df2867dad3ac67d492115b6bf85cf96 |
| Tornado Cash Depo 5  | 2024-09-13 4:17  | 100  | 2500    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x7b94cb3bca9ddff73236b79bcf6e50bde252d22aeadbc103a9127f6698e37a1c |
| Tornado Cash Depo 5  | 2024-09-13 4:18  | 100  | 2600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xa0c9a9d0654cbd6a16d39469e406a58023e80bbaa6a5da826ae45e12e041193b |
| Tornado Cash Depo 5  | 2024-09-13 4:20  | 100  | 2700    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x91758f526c37cc9e89696ffcddf3a3c474553e1f9f6be8c05aceca2588f67293 |
| Tornado Cash Depo 5  | 2024-09-13 4:22  | 100  | 2800    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x5ee96e6a89231baa92a2826a3d761d2234430bd07c1a335a95309a3ca0e7e30b |
| Tornado Cash Depo 5  | 2024-09-13 4:24  | 100  | 2900    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x1ee8e65deb18449ad8b0cc97ab985979bb0c06eb5d2c87e6cc94e0e64694f707 |
| Tornado Cash Depo 5  | 2024-09-13 4:26  | 100  | 3000    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x4217671cd262e1006a88c86d4a7f553caefe15474ee547cd2b487729340eb428 |
| Tornado Cash Depo 5  | 2024-09-13 4:28  | 100  | 3100    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xcffd19be4825a7f3e95f1f3e4fe535d3eba12516c8137517593a823f20d1d936 |
| Tornado Cash Depo 5  | 2024-09-13 4:31  | 100  | 3200    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x504b0ba5d079dcd1a0e0efb40d154e7601f5a38c464c2bc191b098c043326674 |
| Tornado Cash Depo 5  | 2024-09-13 4:33  | 100  | 3300    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x0637b7a67d3c0ce7b224c43d270a1feeaee729ccdbf2e2402978688c02658271 |
| Tornado Cash Depo 5  | 2024-09-13 4:35  | 100  | 3400    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x22b91210ccd53194f948433462958b88a50d2672b24f060f5b6ff00220286545 |
| Tornado Cash Depo 5  | 2024-09-13 4:39  | 100  | 3500    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xc408b5512228d7e14569e2a7c1b01be5acaf021256c0b5feae6fd1c2d88d136a |
| Tornado Cash Depo 5  | 2024-09-13 4:41  | 100  | 3600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x7bd4c829912a3c7f56526b9566e298a844ba5b865c3f4570db0f6efcbbf18a2b |
| Tornado Cash Depo 5  | 2024-09-13 4:44  | 100  | 3700    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x5bcd66fbc6f29157c73f0ac32e6a0264d37e2cdb1cb3f8e13e347f6440bed7c3 |
| Tornado Cash Depo 5  | 2024-09-13 4:46  | 100  | 3800    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x3d41bd10cd4245dd3b1c7152093b47ab06789b6fe061d74f1edb0fe1c9994a11 |
| Tornado Cash Depo 5  | 2024-09-13 4:49  | 100  | 3900    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x8c7ef2f49daae30ce4f94fcac8035ffd0f862bf5b4dee2b0fb9d6da84b728a54 |
| Tornado Cash Depo 5  | 2024-09-13 4:52  | 100  | 4000    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x0ed5e8725a90a4a70d23ce8e416c7ef2190070ca0db7fbbd17288d9bf5e6db78 |
| Tornado Cash Depo 5  | 2024-09-13 4:55  | 100  | 4100    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x07f8694cc6d9c0938ee5089f1ba1d147701bb64460bd42c0b2ce7e25338aaeaf |
| Tornado Cash Depo 5  | 2024-09-13 4:57  | 100  | 4200    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x687b2ec581627d791d5b7dc61a2733b6d6fc6147fcaf11067674094f4d5fab27 |
| Tornado Cash Depo 5  | 2024-09-13 4:59  | 100  | 4300    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xfe92366f8ed1fa3db5deb521a50af917b8cac6de8b1e47e073963b94c0e383b9 |
| Tornado Cash Depo 5  | 2024-09-13 5:01  | 100  | 4400    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x5ffdb53756f3611e91fc44ec04f4ffa74f573fb1a81b901ebb7c736a5dcc6d66 |
| Tornado Cash Depo 5  | 2024-09-13 5:04  | 100  | 4500    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x90bcfee6fb29fb5b17592a9f59013ab5c27d2d3f21a398841bbfc4ffe9eab942 |
| Tornado Cash Depo 5  | 2024-09-13 5:05  | 100  | 4600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x4a64f3d70d02edbddc9f0f7fb980ce9dac42c93c35ebd0f83957a2993f405489 |
| Tornado Cash Depo 5  | 2024-09-13 5:07  | 100  | 4700    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x49177e43b4bd0f9a4c5725d5d6b45de9815f8e817754d43492e1d43ffec4fa31 |
| Tornado Cash Depo 5  | 2024-09-13 5:10  | 100  | 4800    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x0aa64373fb656367bdb43aacd368e6c6c3df3dbbc129dd64f05a04f01ece6070 |
| Tornado Cash Depo 5  | 2024-09-13 5:11  | 100  | 4900    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xd832b3ad62d6d01e54b49d0296b27bba239c66fc8aa69703ac67c503b71f3be8 |
| Tornado Cash Depo 5  | 2024-09-13 5:13  | 100  | 5000    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xe953ac210406cdae7bbe80e132c22a9bd7acaca8824b31bc0d311dc9640a4cce |
| Tornado Cash Depo 5  | 2024-09-13 5:16  | 100  | 5100    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x95db5dc28c85c6b0223f4a879919cde448247f11827326ce4ec9060a8f57047a |
| Tornado Cash Depo 5  | 2024-09-13 5:19  | 100  | 5200    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x2b1bb762b0cbaea7d1ebb12f326dd281d9f771ce1c6c06e11e57556a6a2cfc90 |
| Tornado Cash Depo 5  | 2024-09-13 5:22  | 100  | 5300    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x1cf40ee25943c2d93fd527249bd9002b1de77f3fc8b1b83d6153c8c76fede1a8 |
| Tornado Cash Depo 5  | 2024-09-13 5:24  | 100  | 5400    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xfc889d088e639820ed525577efb907b9f0728ef674340a5e09fcdc04b7ec6198 |
| Tornado Cash Depo 5  | 2024-09-13 6:05  | 100  | 5500    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x981c7d22d0f09e4b16ef95df6dd51b8143aa285a4cb8149cfaaf173b0d967fdd |
| Tornado Cash Depo 5  | 2024-09-13 6:07  | 100  | 5600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0xca37ff0267372daa747f93ccce66c170798f7273dd760f1dea41a8d77aa67da2 |
| Tornado Cash WD 4    | 2024-09-13 6:09  | -100 | 5500    | 0x8d5be3f6d41f56e6c2e39c9420f1736de9ca91d6 | 0x1a52f37106ded40be57ecee93129e86cd89cf9a5caa9fbb7d5c3fec0fb33564d |
| Tornado Cash Depo 5  | 2024-09-13 6:09  | 100  | 5600    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x9ce75448a65f7eb1e52e37c1f03b943efe8f4b5a37ad41bf4ec620cd2a30a30e |
| Tornado Cash Depo 5  | 2024-09-13 6:11  | 100  | 5700    | 0xa4d155734f0b704ea5568ce89b687d2285279845 | 0x7022576556c5e546365c9e7f98fe1e32b7f42dce400a66728b8aaff68bbabdec |
| Tornado Cash WD 4    | 2024-09-13 6:16  | -100 | 5600    | 0x92c627005058e67b5c84e17f4566dc9118edb689 | 0x25ed5a18150a3ea7e3e69a85702ebb73fe53adf8dc3b4c3cbf97d960eccb2dc0 |
| Tornado Cash WD 4    | 2024-09-13 6:32  | -100 | 5500    | 0x65dc7e985d1db21a24fdca13e61253b8f12a5b9f | 0xa49707f356b8ae247651f7b648c351130b33d1a90a7e94ed2571024fbc04d39a |
| Tornado Cash WD 4    | 2024-09-13 6:42  | -100 | 5400    | 0xcb887e43ac29036e4ff25027dac01d26ea9549e8 | 0xb60338826d4ddbc48b25daa97dbae0c5806e764a5fbf87e03bd7955de6ac79ca |
| Tornado Cash WD 4    | 2024-09-13 6:47  | -100 | 5300    | 0xd5dfb12a0bf09f745cc7d7df59516bf45b3f594b | 0x7507ba41e79920aa2c16aad787bf59663b4b621cbe17f259390acef8fdf41ed2 |
| Tornado Cash WD 4    | 2024-09-13 6:50  | -100 | 5200    | 0xce94da88537c8120a43eab2836ce45a14642a298 | 0xcd313fd698f3df6924729899d42ac70a3f51c2945ad6944f6e618deba5fbb54b |
| Tornado Cash WD 4    | 2024-09-13 6:57  | -100 | 5100    | 0xe844b155758bdaf18bf7d55118a4326c44da27d3 | 0xcaa048ba8568e2b54563d9072d700b569b8e1ddae8e8f4a91831d830af9b051b |
| Tornado Cash WD 4    | 2024-09-13 7:12  | -100 | 5000    | 0xabd720fd844120cc7be804947a0b427e09f658c4 | 0x121b88250bfbc89ef8e392fb8d1998cae1679abbb7de92aca1352dd9adf3bd98 |
| Tornado Cash WD 5    | 2024-09-13 7:22  | -100 | 4900    | 0xe54d59fd8281188c1f2d8ab2fa32356c5f761647 | 0x0e14db8addb0523302df2eaf04ec8edb74b690fca9c1012074c93e042ab93122 |
| Tornado Cash WD 5    | 2024-09-13 7:39  | -100 | 4800    | 0xe05ebaeb153d8cacc68631f05adee863fc9666f9 | 0x3e0ea91d98ea8fe2e540f0be4d3c261e31dd1794ce10c9e15d20caa0f486ed32 |
| Tornado Cash WD 5    | 2024-09-13 8:33  | -100 | 4700    | 0x6c76af0c792836cc403d3112c177f02555b7ac7f | 0xf16a174914eecafe1d6b2d0903758c38e2a1a3c1473cb023570d8c7d28a00e21 |
| Tornado Cash WD 5    | 2024-09-13 8:40  | -100 | 4600    | 0x55a58d2ad3ace022659112c3abe3cb7ddde494cb | 0x650a331cf604d6dfadee52734f12e06dd0426349fecefb420c447c930816a99f |
| Tornado Cash WD 5    | 2024-09-13 9:03  | -100 | 4500    | 0x373a81edeac09d8347474f8b4a874865760ddbf8 | 0x687daa71262b39d7d96a4c6c785fe84735f8dc452ace19fb7ce4e8a74ad6cc2a |
| Tornado Cash WD 5    | 2024-09-13 9:27  | -100 | 4400    | 0x4594651bd2180a63b04174748f83870f56401b88 | 0x87db07309178208638a64288aa8314bacdb28fc340e5db574a6ea65837f37b5b |
| Tornado Cash WD 5    | 2024-09-13 9:35  | -100 | 4300    | 0x6f99078979cc76dd46688ecf2cae997229556270 | 0xa7a8cefd569390e9e7ff9c80dd388c68f9c20f62c6fa8582671d42c7555273e5 |
| Tornado Cash WD 5    | 2024-09-13 9:43  | -100 | 4200    | 0x8ae40b93515a30c701dce8ad40f314564612beb6 | 0x5e0f94cf994c20b05856ed45395382473653381822b282ac53d873fa71e3e25e |
| Tornado Cash WD 5    | 2024-09-13 10:08 | -100 | 4100    | 0xe571382adbd879ebe7949a0c0b8825a77c878ea3 | 0x07106188bc68b51198af3b3aa8525c24664cd95c7a187a3ba2310e4b0b9ab8d7 |
| Tornado Cash WD 5    | 2024-09-13 10:34 | -100 | 4000    | 0x7c6fe09dd97014e0eed923ea843474b6cc6b9257 | 0x4e4ab9ec4b7c1e0ad9ee61fe89e993444f2b20c746d2612d9ed66b4c07ecbffc |
| Tornado Cash WD 5    | 2024-09-13 11:00 | -100 | 3900    | 0xd077b17656ff8a9abcb75ba0968fb8e68ddc277c | 0xd1e8812a7945dd42cbd39276ff79b695d2f54f17f36d9e47f900dc92620e03d6 |
| Tornado Cash WD 5    | 2024-09-13 11:20 | -100 | 3800    | 0xa5e31f435b60867fcdbce0d408eacee712229d00 | 0x3c85da0333bb8645782cf413a6e8d7048d559916c7775258b21467194e7484a5 |
| Tornado Cash WD 5    | 2024-09-13 11:41 | -100 | 3700    | 0x147067734eb5f7d22692e5bd89111f4a9f8283d0 | 0x559471d3c936f04de0dfd45741a7e074051bf6336b746d5fa35d97b9e90ab556 |
| Tornado Cash WD 5    | 2024-09-13 13:29 | -100 | 3600    | 0x66270c3aa1fcfaca8f033d3650c6255ac57c27a4 | 0xe1ecff89a94d839a4c96786254ae748422c10cb8f83b983804ca9b686c69f4bc |
| Tornado Cash WD 5    | 2024-09-13 13:38 | -100 | 3500    | 0x05c549ea65dedb7985fd6e57c6ede20d7a18a038 | 0xe60cc64029480103b767bde8e0a65ba031b98a89899470cb7db511e01e410ddd |
| Tornado Cash WD 5    | 2024-09-13 13:59 | -100 | 3400    | 0x9de9a3d51793ffc4f7c8d5adf5a82ec178dc439e | 0xc324ff6f1acc58b2109c3283ca7fbbabf38be6c014c08234515685af7fd928d9 |
| Tornado Cash WD 5    | 2024-09-13 14:05 | -100 | 3300    | 0x075da34c1d1ef8b5f96a93ddb3af57e7308173ae | 0xf767df0d51c2a014475a0743535461b9a862f9012d16ddf3bc2d5922eb06e915 |
| Tornado Cash WD 5    | 2024-09-13 14:18 | -100 | 3200    | 0x326742755592c8f16f37a8d0c65f91b208cd4082 | 0x4f22e99d86e43f0534687c80a4ae38589aae509b2e7a727860ccdb582208c2c0 |
| Tornado Cash WD 5    | 2024-09-13 14:27 | -100 | 3100    | 0x38323914d2fcbe39bcf4ed6ecfe78dd7a7292f47 | 0x027df9143b114a5687c58dcf3094e049fbff0990ab966bbc8ce443b8199b7e22 |
| Tornado Cash WD 5    | 2024-09-13 14:48 | -100 | 3000    | 0x53cd07a23ea9d20d3f08f00629a21d4be105e29f | 0xeae1c390bc7d10826edc3edd812c85ce62b32c7d5119af0f0a62583ebf2025fb |
| Tornado Cash WD 5    | 2024-09-13 14:56 | -100 | 2900    | 0xa4aa0734701fb1b5933bc2fceb72b98b23e235f0 | 0x52beceee2b01c769691aafdd8a83a74cc50a43dcb525f1b8d82c8661c1bed7fe |
| Tornado Cash WD 5    | 2024-09-13 15:17 | -100 | 2800    | 0xfa7011e60f6cfb30ac048e2b261c0b9125e2bd10 | 0x24b65dd1238e5495406e021d496fe2355da1306598e36e77aff6dea78bba2d6d |
| Tornado Cash WD 5    | 2024-09-13 15:22 | -100 | 2700    | 0x61e1b1d5af712a6a0b49ad56d873b0d6423c9c3b | 0xf2189eb3b0d3102a92ec0ed9086db027d2c1920fb3a09701113c9927550d1f51 |
| Tornado Cash WD 5    | 2024-09-13 15:27 | -100 | 2600    | 0x4dc94da4aa71e7f18e277da064c53ded4dd3a45a | 0x9e05f179ab16ba2e72d437ab822e5b4b93e876d32f60be7f346d9e696abca52e |
| Tornado Cash WD 5    | 2024-09-13 15:49 | -100 | 2500    | 0xb02de56c50ecd3278c4c79d1b67bb4292a22f4b9 | 0x6fcd65007fddb5ad806a459235c113400eae73dfeb8152623e1ee12a12efd2ed |
| Tornado Cash WD 5    | 2024-09-13 16:02 | -100 | 2400    | 0xf66541f80835a066be142541fcc02e22700d16f6 | 0x8b1d93f7cdb652de612dafaf532fc00f99f542e9f237b947c168ed3f2cd2ee9a |
| Tornado Cash WD 5    | 2024-09-13 16:08 | -100 | 2300    | 0x393be1c8e7a78cdd8b4ffd755d86ca515a00982f | 0x9d0101d59c75f3eb8210b334cecc6df2202018491826da6ef12a3e757eb265e2 |
| Tornado Cash WD 5    | 2024-09-13 16:20 | -100 | 2200    | 0xb252d1ff818d44fa8ccd2c0351ab01486c6aaaa9 | 0x4c4d72f0b97bb2ee905655083366eae4de5c036109317c4a12fd229f64a9a22c |
| Tornado Cash WD 5    | 2024-09-13 16:26 | -100 | 2100    | 0xd43e7a3b044120099b8f6a56080c2357530d5ef6 | 0xdb368c4d8f0e0aafad96153a14dd61474a6a40991054b036ac0dd64aa83b7c9e |
| Tornado Cash WD 5    | 2024-09-13 16:42 | -100 | 2000    | 0x5a80391059227f2bae6b4d3f1b37b6c399365646 | 0x884688b460f17b00163b356501546eca5cd3f379ffae929d8870e75fe0b9f252 |
| Tornado Cash WD 5    | 2024-09-13 16:59 | -100 | 1900    | 0xebf9b55a95e9062572d79e273cc6adfc417279d0 | 0x399b2480601b7a56ad4680951246017075c845880055cb1479582d9b143da5cd |
| Tornado Cash WD 5    | 2024-09-13 17:05 | -100 | 1800    | 0xc09a15894123249ec0af1e43509cfe61b13b368d | 0x9e9549dbe073cfe2ad8c86c1de9cdb2040a9ab595ec23c7aa19f45000aee87bd |
| Tornado Cash WD 5    | 2024-09-13 17:16 | -100 | 1700    | 0x51832b7b9e67ba5e2c8b39a71bd20e5d02e651d8 | 0xc47ac7072126285a62b0729fcf9316c5526828ce114f75e33f85aa7f0e999fe1 |
| Tornado Cash WD 5    | 2024-09-13 17:39 | -100 | 1600    | 0xd80e62a5e9bd58777a7c8b841e5bfc40ee8a4ff9 | 0x7272ec1f42f7950cd1d0545f320fdd3037464dbf729ff5bc692900835caca0e4 |
| Tornado Cash WD 5    | 2024-09-16 0:23  | -100 | 1500    | 0xee5343f52af4858e527c9a9ad85577c17f3836cb | 0xc879462734c405a9eaa805a351a6eac94d2d48823f3bfafbb8b80727c00a63ce |
| Tornado Cash WD 5    | 2024-09-16 0:39  | -100 | 1400    | 0x9810698b1df6fee775bafcc41933b929b12f5c9d | 0xcad3c5324e8ecf20b0858d5d9a4db05d42ef95505aa5b145ca8e5437c78a9ee0 |
| Tornado Cash WD 5    | 2024-09-16 0:53  | -100 | 1300    | 0x342b47ab0c5b3544ddf1e735a401165b25263b6f | 0xcd318907df46f55d3aacffe38b0884cc585c89398bb938be8b7feedab9b2b555 |
| Tornado Cash WD 5    | 2024-09-16 1:07  | -100 | 1200    | 0x277a53f0184aee437c335e0e0464b971c1dcc4b0 | 0x734fbdd2d07fe91a3037fcd9597e751ad5e86042f2bedd80be0dfc43db0137c0 |
| Tornado Cash WD 5    | 2024-09-16 1:24  | -100 | 1100    | 0xcff1760c7b9be9ecddb1248578257a7b01efda28 | 0xb416cd53f6e54e063386220185545cd7b5d1e6f4c94a40c597a4fcc29951f94b |
| Tornado Cash WD 5    | 2024-09-16 1:40  | -100 | 1000    | 0xca011ac352065e289814475984ae50f6e7ede448 | 0x469297e4028bb5606ca3852559fd96266669cbe2af9d0f4dbc7a836aae945ccd |
| Tornado Cash WD 5    | 2024-09-16 1:51  | -100 | 900     | 0x507e0e33fe23b7aae348a1f89bb08709062a5b41 | 0xcf3587c7538c58b0556f35a80bb02f7988641b8c679e4c1f6e764f2e7af02c77 |
| Tornado Cash WD 5    | 2024-09-16 2:16  | -100 | 800     | 0x91356bfc9d08471f356891f23143707cf32343f5 | 0x75d205e1e0e90c3fa0f4b446f076e5d9d4f4eaf7fbf3f3f4048ab6ceebaa9a04 |
| Tornado Cash WD 5    | 2024-09-16 2:42  | -100 | 700     | 0xeb003fba831b2bc58d5cbbb8255e968b9f4a04b1 | 0x87abfdf2d8cab48f4f92dbb0fc0679c801fa25601ea16e8e0775a3e49393c298 |
| Tornado Cash WD 5    | 2024-09-16 2:54  | -100 | 600     | 0x24b96753285e10883ae9b535b7fe71c59e7e8432 | 0x7a49ef0698246368d49e4169c501a3ed9c60b4cd5599259fab5d8b12d475ac26 |
| Tornado Cash Depo 6  | 2024-09-16 8:51  | 100  | 700     | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xa9f5d5f11e4616ce99c18e786bf7dfed13e74b663f3a6472d7d109e98111b1d7 |
| Tornado Cash Depo 6  | 2024-09-16 8:56  | 100  | 800     | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x28c0f5fe8df2db43ba01942bc4bf950693c02314a5ca264f4813519c489e8cc6 |
| Tornado Cash Depo 6  | 2024-09-16 8:58  | 100  | 900     | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1ee0d16038f32ae2d8eccb636621bc44c2584ad35e5613cc87e47bdc9b41ef35 |
| Tornado Cash Depo 6  | 2024-09-16 9:00  | 100  | 1000    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x3371097165feed7bafeb37af3e7b23974ad9c66dcd58e1ea8fd170875959e40a |
| Tornado Cash Depo 6  | 2024-09-16 9:04  | 100  | 1100    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x4665eb90802a6c45bb2c43a271974c96b040b477faef1a114f7326e9329af103 |
| Tornado Cash Depo 6  | 2024-09-16 9:06  | 100  | 1200    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x5dac3213d752a6516ad7b5cc2b5c4b3999d2e17f0aa621ef83add2db8667e21c |
| Tornado Cash Depo 6  | 2024-09-16 9:09  | 100  | 1300    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1a6660b600ad149f57e61e42a00bb77dcddc073f740f12fc1f30e4c98cafd3eb |
| Tornado Cash Depo 6  | 2024-09-16 9:14  | 100  | 1400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x88a9182ae0ea9f53628e29785ab891fb55b99dbb5e8f69beeaac9412c54aa710 |
| Tornado Cash Depo 6  | 2024-09-16 9:18  | 100  | 1500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xde060f272621b550949b934ad206cb380038229bf522c5c2eddd55f9df002203 |
| Tornado Cash Depo 6  | 2024-09-16 9:23  | 100  | 1600    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x713ea269995555e6f85657441a155698b63fd5e54902dd42a9cde738dff4d99b |
| Tornado Cash Depo 6  | 2024-09-16 9:27  | 100  | 1700    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xc6d818fe34fefada0c126b23011aadc8942a7f5788b2d4ddc92dce2c21240564 |
| Tornado Cash Depo 6  | 2024-09-16 9:31  | 100  | 1800    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x143945620ac7656cb187a63d6aa0aae8487cf2288f8db518fd913a6249634548 |
| Tornado Cash Depo 6  | 2024-09-16 9:37  | 100  | 1900    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xd02f8c58a184d0fdaad88bab4603214d74677b36fa54855b991213ee5021b43f |
| Tornado Cash Depo 6  | 2024-09-16 9:46  | 100  | 2000    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1377c4c1590b5cbe873baa2917c4fc0a41f01d33afa56d6d68294b9f93819f6e |
| Tornado Cash Depo 6  | 2024-09-16 9:50  | 100  | 2100    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x99b66412987275e35fc441ed938da6c0f291809211229372a819971c956bde8a |
| Tornado Cash Depo 6  | 2024-09-16 9:54  | 100  | 2200    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xf07b827dc33c9b71398e558b4f868cfd99c8420136aeefc533bbae74f3e753cf |
| Tornado Cash Depo 6  | 2024-09-16 9:58  | 100  | 2300    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1ae43df15d0c5411a79744c0e5ca85db827431f49a1b4ea314e87dae20c3c16a |
| Tornado Cash Depo 6  | 2024-09-16 10:00 | 100  | 2400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x622ad593b9f899f3c012e00f83097f9c613153d76aa72e295d94c6325c21633c |
| Tornado Cash Depo 6  | 2024-09-16 10:04 | 100  | 2500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x6b1c9160defe4fe250aebec89a729fe94853476db08d50cacd6e75e9d013dac5 |
| Tornado Cash WD 5    | 2024-09-16 10:07 | -100 | 2400    | 0x4a8c5e0c0b5246f7b1a2cc631c1b9aa2f1803a92 | 0x64605c8db68ea660939409c9676c8ffb61eb1cd734a8fc4ac07a962251002874 |
| Tornado Cash Depo 6  | 2024-09-16 10:07 | 100  | 2500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xc34c17bd6a645527e9827e9d40c62b5d0f45d12b2ee6c87c8d81f6eaafed5864 |
| Tornado Cash Depo 6  | 2024-09-16 10:11 | 100  | 2600    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1644a68b41f6260b39a567064d17afc08ad014f8d0e494dd4ea5f26fd5424cfa |
| Tornado Cash Depo 6  | 2024-09-16 10:14 | 100  | 2700    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x64b11fe85ebd44b4eeb4a9b8f5a275e830b9964d3c09e224fe5b81105dd59a1a |
| Tornado Cash Depo 6  | 2024-09-16 10:17 | 100  | 2800    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x9e08b006f16fe57c0508d85802220cd1376da06927c2ce9cd04cb96bf8743785 |
| Tornado Cash Depo 6  | 2024-09-16 10:20 | 100  | 2900    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x6b2dd5413d5096595add7a97439c7f78f5576e1eaf8da8fc095399b0c4bdc6b8 |
| Tornado Cash Depo 6  | 2024-09-16 10:22 | 100  | 3000    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x2a519cb73c310f43de6efbfa86b0b0c3f6cba3cfa8b4e9babef9acc83329affa |
| Tornado Cash Depo 6  | 2024-09-16 10:26 | 100  | 3100    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x0eef539e30d9ce8d113ef8a975e9fc8c7773d2fa07ecf0f0b74eb5139ec627f9 |
| Tornado Cash WD 5    | 2024-09-16 10:29 | -100 | 3000    | 0x74416176c40889843545c6b420806ad4a4630768 | 0x42d64b1665416a86f9536b99a7eae4f5b40e419dab576c7fa85fee2884264ade |
| Tornado Cash Depo 6  | 2024-09-16 10:30 | 100  | 3100    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x072d7658c4d039898082acb7e38af378b4412f342d610989166bba84683a004b |
| Tornado Cash Depo 6  | 2024-09-16 10:32 | 100  | 3200    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x0af3f1ecbeb2dc72d63273e3d07f8d63fa7236f469afedccf2ab9583c8e27c9a |
| Tornado Cash Depo 6  | 2024-09-16 10:38 | 100  | 3300    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x6b17c2f0e12248f8c3ce77d05c4db5e6c79ee61b26ce9d77f3c68ee7f2a79b92 |
| Tornado Cash Depo 6  | 2024-09-16 10:42 | 100  | 3400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x4fa05ff06cbff80b630373402805013320daee229571212f078d3c48ecb5c1cf |
| Tornado Cash WD 5    | 2024-09-16 10:46 | -100 | 3300    | 0x93d08b5b460a4b1c5d93a398f2ddf7c49fa4c48a | 0x5b111e375f31eff3cc3358b8ca60f24064c55dfd83f1d5d4583c52516e2157d8 |
| Tornado Cash Depo 6  | 2024-09-16 10:58 | 100  | 3400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xfe608e057e7b4d1eee35223611d93becb313b3f6596d38f521beee94885469fe |
| Tornado Cash Depo 6  | 2024-09-16 11:02 | 100  | 3500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xf28a89493f0518f0699b0fb7bea1267f430d107794c6f593517021ee3633ac47 |
| Tornado Cash WD 5    | 2024-09-16 11:04 | -100 | 3400    | 0xf0ec5da5dbfccaa70f6038bbedcb8659fdac064e | 0x01a47494ba671141c97cbf2a3a4f34a87f8e92e19e0e9fb69495f4a0790792a5 |
| Tornado Cash Depo 6  | 2024-09-16 11:05 | 100  | 3500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x26098de7aebd059dcc88eebb56662204873b453c266d9a1b517a9af3400ef582 |
| Tornado Cash Depo 6  | 2024-09-16 11:09 | 100  | 3600    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xa2a0d948cc03c04a088e6a615d6ef9d6dfffc9dd629285b1e587d38784ddccd0 |
| Tornado Cash Depo 6  | 2024-09-16 11:13 | 100  | 3700    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xcddb970efb59e5ba5a556d48d337a69e8de1fd4df444cfaf7e007f227461da50 |
| Tornado Cash Depo 6  | 2024-09-16 11:17 | 100  | 3800    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xb49983724d28652ef720419105a41e80ac13bd3d3c03fd402711b5242d2563d8 |
| Tornado Cash WD 5    | 2024-09-16 11:21 | -100 | 3700    | 0x6f8bf5dfe70aab0517d3eabab2837959c01bd9ab | 0x2177ae59e3f50c9efff8a5079f4a2ca734a5924d51cd1921e2afd3fe81d8a027 |
| Tornado Cash Depo 6  | 2024-09-16 11:21 | 100  | 3800    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x1731668a96f93f5e27c31b17d4ac7d2285e7338b57ecdb82b362c05da5f2727f |
| Tornado Cash Depo 6  | 2024-09-16 11:25 | 100  | 3900    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x02998ec9b69f6dd2045e5d04e99dfe85830dad9dc372f0c6b0d06ca26ad078d8 |
| Tornado Cash Depo 6  | 2024-09-16 11:28 | 100  | 4000    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x7f1b210661238a8e604a81ebc33b4ab5288248d559a9c9aa6a7b1220f0023d94 |
| Tornado Cash Depo 6  | 2024-09-16 11:31 | 100  | 4100    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xd41e4c2bbc0e1b608bc6c4068fc5f3457b73cfe722634c2a14635ed49ab6b80b |
| Tornado Cash Depo 6  | 2024-09-16 11:36 | 100  | 4200    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x92d9724c7d8c21ad474ea720ec083106dd5c3c82da5e668ea593bddb74137df8 |
| Tornado Cash WD 5    | 2024-09-16 11:39 | -100 | 4100    | 0x8ea83b39c0417b8df95eafd450328787c946e45c | 0xd348d78478092df0e5676615a9d6fe66705de71c5dbf5cd60cfcb84cadb970d1 |
| Tornado Cash Depo 6  | 2024-09-16 11:40 | 100  | 4200    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xdff8d5def4a80f24fb3bda3867a7022ea456269fc2f3fb6f5eaba81c17bddd7d |
| Tornado Cash Depo 6  | 2024-09-16 11:45 | 100  | 4300    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xff2ee95c189952c0950427f3d67cdb0a6dc9acfc105bee4d1c0865c540d99b58 |
| Tornado Cash Depo 6  | 2024-09-16 11:48 | 100  | 4400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x07d0e5f47fe4e6c5c5024c3224d02f166d9c13b9951d62ced6d375c197ef0052 |
| Tornado Cash WD 6    | 2024-09-16 11:59 | -100 | 4300    | 0x7974b5749f0d7f8a8053f92ab95c47ca1ab34855 | 0xcfe813832eb96779e23a1cd6147d2f0c508e9bdfcf928e12e3e2f66bdac265de |
| Tornado Cash WD 6    | 2024-09-16 12:11 | -100 | 4200    | 0x8a6f2865f578ae4417251ebce17931acf6e7afc2 | 0x32eb98ee4a06bc8e0a1e8994f817bac3cb1cc2deffe54f1686359ce432ea2c48 |
| Tornado Cash WD 6    | 2024-09-16 12:21 | -100 | 4100    | 0xdbc7f26b2cf2cc66fe5936b93f1a262b15b8b56d | 0x439324e6c2c072abd526705671a92e0e01ae86423bf03d0122dddb71c3b8e717 |
| Tornado Cash WD 6    | 2024-09-16 12:42 | -100 | 4000    | 0x3c08442f3934e4081e5a0f747e9cc5a0ecd99641 | 0xdd3272fb6ce43f11c134cc0abc6e533dc36085c4527c025bc604d81225a2cb82 |
| Tornado Cash WD 6    | 2024-09-16 12:46 | -100 | 3900    | 0x39c46a88a354de38e0015400dcd6ba5ef94231f5 | 0x3972b0e9492d9cff19df3285180c7cd8700ddbffe0deb4329aaf539b98ae8976 |
| Tornado Cash WD 6    | 2024-09-16 12:51 | -100 | 3800    | 0x0a01cdd11659190d611b12e52ea3c31adf95e282 | 0x7dc0118aa6e08da370108f272d61f24f8170b6b60b74acd7096aa9485e0ec78c |
| Tornado Cash WD 6    | 2024-09-16 13:12 | -100 | 3700    | 0x20649266a6370ab0a29cf04a561c9f739a8da37c | 0xf5b23b0b2e23067e1183bd665aee1ad281f0bcdff41baa408ab0d522f0b1369e |
| Tornado Cash WD 6    | 2024-09-16 13:38 | -100 | 3600    | 0x305ecee08e168d082bd981d7638d689ea0784e78 | 0x08eeefea4f1622acc6c77d2df21c873f918b506ae98a4137a289a003ffb0c2a3 |
| Tornado Cash WD 6    | 2024-09-16 14:11 | -100 | 3500    | 0x3f382d9c8421868135ca9c3e92aedcd337da21b1 | 0x83382cef9c7be1ab05c72e4ece1a8e20bdfd864ffa4696e351c5bcb4685dcbe8 |
| Tornado Cash WD 6    | 2024-09-16 14:25 | -100 | 3400    | 0x86c15f08c791374e951a3cba190bcafe4ae49c20 | 0x2f78b01110323bfd5ad3da20a8295c686d77e27a86b251b5c2ef9036ba532b0f |
| Tornado Cash WD 6    | 2024-09-16 14:38 | -100 | 3300    | 0x0591a528c173330c2a63a895c6118d6427cfccd5 | 0x7d7486755daf3daec4a5705cda75a087d957c1a47d6e2647a481f1ff60082bea |
| Tornado Cash Depo 6  | 2024-09-16 14:40 | 100  | 3400    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x3cbd5a5e52c611d794b7a78434cc4cc0010d2c1b69cacf33e4ac99551268a71d |
| Tornado Cash Depo 6  | 2024-09-16 14:43 | 100  | 3500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xe278f94eba2c8fa8b1a444414730e9c7a77621babd44eb08ea99db08e38b9992 |
| Tornado Cash WD 6    | 2024-09-16 14:49 | -100 | 3400    | 0xda39eaa3f2f51dcefa8978c9f5253ea5abe9aa4c | 0x5480c1d861943398b0169434a8003f37fbe907aa347fab57c19abb7458502372 |
| Tornado Cash Depo 6  | 2024-09-17 0:45  | 100  | 3500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x6ddd9c7f757a03b775e24276a90edacfb5ccd85dfafe07125e505e9c267849ed |
| Tornado Cash WD 6    | 2024-09-17 0:46  | -100 | 3400    | 0x192cb0ea2b29c8e0a380eab3774fbfe96580b570 | 0x4b9807828ed6d5f92df3c284ed996f7469ed7233648bd2e909dc9eb05245c16d |
| Tornado Cash Depo 6  | 2024-09-17 0:48  | 100  | 3500    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0xe971b45d4765acf0fd6afc74710f25d161acd4b6427c1c164cd20cc63c7cb718 |
| Tornado Cash Depo 6  | 2024-09-17 0:51  | 100  | 3600    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x6da0473c9cfe9dfac2d2c16899cba4643e8043d03a4eb40a5969ecd4c8f2ca2f |
| Tornado Cash Depo 6  | 2024-09-17 0:56  | 100  | 3700    | 0xd70d8a4763a6b9e913db96eba6d6c6aaf0484bbc | 0x5c03b34dffcb7bc68b00d10ac6fd0a87da30ec8771a2aa03962f0387b6fb04a5 |
| Tornado Cash WD 6    | 2024-09-17 1:00  | -100 | 3600    | 0xd9a561317c3a9934c72773c8164a297c995ae35d | 0xda722d801672b5ef2f49a55e2d63a70b99537b02cae9eea949e61359a3f3e1f4 |
| Tornado Cash WD 6    | 2024-09-17 1:16  | -100 | 3500    | 0x8382f8e81295a45d513a40ecb628279dd822334c | 0xba09adbabeaca9eb9c3bbf084dab9bd99bb80826b10014f351e6fc19a5975901 |
| Tornado Cash WD 6    | 2024-09-17 1:38  | -100 | 3400    | 0xb1e3f0548ca5e7ae479d244e90aa6bdf25bdcd7f | 0x787ef09ff2d5250cd7719f48ec86166418dbd3eeb84baa270815dbf9e43e615a |
| Tornado Cash WD 6    | 2024-09-17 2:03  | -100 | 3300    | 0x2500fe47c0202bdd8ecb798fe075044c1869c358 | 0x344e46edc5a3b9dd66a5f436f1060ac154c388adb8569d6f1d118a8c67c458d1 |
| Tornado Cash WD 6    | 2024-09-17 2:14  | -100 | 3200    | 0x49ad6478d3be0670679048d74e311e0edf9a96c8 | 0xa024a6ac059115ce906b3d2f9a15191c0091ab33ccb986087b8f23da267f5fa7 |
| Tornado Cash WD 6    | 2024-09-17 2:33  | -100 | 3100    | 0xba9fc7c5b027331c6b8ffec7a2175a174789a585 | 0x307ff4c09cdb56198cd85f1e82160bef11cff1a6ca19628b13357db584eb370a |
| Tornado Cash WD 6    | 2024-09-17 2:55  | -100 | 3000    | 0x0e19186c8a83e7d41f94d78f2057c264f23d46e4 | 0xc9b31c068c2390cdd96014523cfab4db889432ed02bc9d78c3316fa9f3c78a4a |
| Tornado Cash WD 6    | 2024-09-17 3:12  | -100 | 2900    | 0x480ed3ad5055d63c2e67a8d5781901e01699d191 | 0xabcdfe0438b6a794bfea8271c647377b6799078594aac90cb8391af7c3e5027d |
| Tornado Cash WD 6    | 2024-09-17 3:21  | -100 | 2800    | 0x330945b6e906bcd745e43ef9566064f2a7b2b0a2 | 0x8bd31bf5688b1de6c24de3b91bc177b733a68839354dc6c3f3e2ed8e8789b87b |
| Tornado Cash WD 6    | 2024-09-17 4:31  | -100 | 2700    | 0xc6f9fb51a425ab972b6f8eaaa49c35020e0d8f1a | 0x0f6abb3619001fc2095184112002533373df7a809017e190cfc5f7f98f6d0236 |
| Tornado Cash WD 6    | 2024-09-17 4:35  | -100 | 2600    | 0xf51328f279cd262d22ebc1ae267079f33f492635 | 0x72cc4c64b140353ee2bc50fdc4efe25966b53eeddb9a95c0e51e281a5ee44607 |
| Tornado Cash WD 6    | 2024-09-17 4:45  | -100 | 2500    | 0xe26d6144dddf5d3194d250c89e179b8645bc9bf3 | 0xa68335fcea39ef98d252cf0fbea846411c53a38ae633dd4c53c6a7251ec7b87f |
| Tornado Cash WD 6    | 2024-09-17 4:57  | -100 | 2400    | 0x5dbc522ef80dbb7d4014d9b0c90fa80ed23223ba | 0xfb7cca805c41490b42318059bebf5571fbf2a383b7f5785f18594a67c7271843 |
| Tornado Cash WD 6    | 2024-09-17 5:03  | -100 | 2300    | 0x632cd7c3aa127771881390e7ac907dd1de6b1b53 | 0x9341a804c2c49dadb14f66dc86c8342c831705d2a8fae70da71dc0a8cbf6b8e4 |
| Tornado Cash WD 6    | 2024-09-17 5:09  | -100 | 2200    | 0xacb5f58d31686acc720641038f0668ef54665f0f | 0xc44cbcac583174c598037c11387ec22a6cb05d8fc0d105a61721ec9715fcf893 |
| Tornado Cash WD 6    | 2024-09-17 5:19  | -100 | 2100    | 0x8f40ebb782ac0af5c14ee550f276f5d10c637a02 | 0x5f0f7d90e01777a5a90cdb8f070bd86a450f49c56a2b4b1394ffc966dd08fd7f |
| Tornado Cash WD 6    | 2024-09-17 5:32  | -100 | 2000    | 0xa608a96ccc3164ddcbcbdcdb9a2d200a6a231711 | 0xa6cc006165224596e56f3901e762c402030b9d04bfbf15820f27109e98bbd54b |
| Tornado Cash WD 6    | 2024-09-17 5:40  | -100 | 1900    | 0xdf105accecd919c74e57d53295731c661470b5e8 | 0xff020ea8d9a74fdbfa5e59c339b751207538292751b0e93b9a2191ee145a213d |
| Tornado Cash WD 6    | 2024-09-17 5:53  | -100 | 1800    | 0xa3a6442eb2ecb3f921549a0879217652dd60189d | 0x7ceb590f6b9ba519e2672d7d573cf009770c66081010fe561e70db2f041b6196 |
| Tornado Cash WD 6    | 2024-09-17 6:02  | -100 | 1700    | 0x582803f2dde7459283352a48224ea6f11f07b4d4 | 0xb741ee1b263160056a7638946cd42c980a90ebacc9bc3828a4f4fe13e0b8727e |
| Tornado Cash WD 6    | 2024-09-17 6:09  | -100 | 1600    | 0x5aa975bb69133aa9a9757c84147718ed99d40c1e | 0x0e0275c50134040e8600a212f377a2a3fef7d655d8f4453d9f0f2b728cc422fa |
| Tornado Cash WD 6    | 2024-09-17 6:17  | -100 | 1500    | 0xc52648f44610cfd2c3fefe0750479fb2d0ff7a6f | 0x1b643f7dcf2ff487ef20c6926eab8700695b77ab095d029db0b56aab19a5ba9a |
| Tornado Cash WD 6    | 2024-09-17 6:23  | -100 | 1400    | 0xb774b05040c8550abecb0aa851581ae2e8ebf33d | 0xbfe4c8fb79addcf789bbf76a735fc30f9d66f0975bd43c81654a179b40f4e912 |
| Tornado Cash WD 6    | 2024-09-17 6:34  | -100 | 1300    | 0x13964b844edd0a8babcfc1db58c499bb9b11350b | 0x10dbfd5732ac68b73613a0026a67ccaecdcff256bdbe22234522f97b97518aee |
| Tornado Cash WD 6    | 2024-09-17 6:43  | -100 | 1200    | 0xe080aa8bd639e00b9fb8653db52867699b4780a0 | 0x0fd57d6aac9ab2857020faa82b5bfea5422b739ceb07020080a39406cf769694 |
| Tornado Cash WD 6    | 2024-09-17 6:55  | -100 | 1100    | 0x69b993d0c0ed2df55115fce77f5a55334a85c57f | 0x2e1876df2a066ea6a1f5201073b5142fae3b21df2b096db0ed02a1a2953301bb |
| Tornado Cash WD 6    | 2024-09-17 7:01  | -100 | 1000    | 0xbe7caef1c93b8fe91d73e1322c719fb8e47024df | 0xbd03da66ecd32c833482ad78bf2c2a2dd9177a38d81ded76d6486a27c3c98519 |
| Tornado Cash WD 6    | 2024-09-17 7:17  | -100 | 900     | 0x0e019e1e3f6069d432b6fb0d4778c609fd4e824a | 0x46c8b752ca52adea22b40c8a83b49ab7c4fb332e14ff444cb4e2a3f9ad2a39a4 |
| Tornado Cash Depo 7  | 2024-09-18 7:00  | 100  | 1000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x797dc42cc655959dff09950e144e5cb2d331adcbdda7c584af357faf542e5825 |
| Tornado Cash Depo 7  | 2024-09-18 7:02  | 100  | 1100    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xd8460d7783c2de2addb5d7a275e8fb02149718a972b9e0727771a2de0de098a6 |
| Tornado Cash Depo 7  | 2024-09-18 7:06  | 100  | 1200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xde620810154a7b5b8c0d9b17a56af986af3d7594880ec759ad98bf01d7aceef5 |
| Tornado Cash Depo 7  | 2024-09-18 7:10  | 100  | 1300    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x2a3e27c0af69186ea6933d6955d2faabcc5df75314853cabfb17919e7ec51e26 |
| Tornado Cash Depo 7  | 2024-09-18 7:13  | 100  | 1400    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x34235f764823603f875550614554e66067c5bc8a009042ce910fac4d6515ad0b |
| Tornado Cash Depo 7  | 2024-09-18 7:17  | 100  | 1500    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xed6827890ab2f83e06d0a2705f4f75486e524628939c33eb4a148f08f58fe1e6 |
| Tornado Cash Depo 7  | 2024-09-18 7:19  | 100  | 1600    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xdee49e919a9337d14435a5c3b1b76e23bec7d78f1601151c77a8a084ed8d396b |
| Tornado Cash Depo 7  | 2024-09-18 7:23  | 100  | 1700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x9a9e604ba7344a69ff2e2158780e0b4de4e943020fbe6c5c4f7687cd3335f251 |
| Tornado Cash Depo 7  | 2024-09-18 7:26  | 100  | 1800    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xcae336815a7105795b063b3b7d7f99eede97e1634531ccb82a28c8e5bb1b236f |
| Tornado Cash Depo 7  | 2024-09-18 7:31  | 100  | 1900    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xb5161b44da6e8a7dcfadd477ad8b8c46d8421a60c2b74c21f45eec1e6a5a35dc |
| Tornado Cash Depo 7  | 2024-09-18 7:33  | 100  | 2000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc764c7aa6bfa812030e59491700983cd2d2fecfc43a1f553c2d644b111dca4f1 |
| Tornado Cash Depo 7  | 2024-09-18 7:36  | 100  | 2100    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x981312f8a336fd55733351709a2c09b6129719b410d1fdf6942e39aaf8ac8818 |
| Tornado Cash Depo 7  | 2024-09-18 7:40  | 100  | 2200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x36cd8e7dcf38ae8d742ea4634e8e8a67700db8d0a891b4d1781ab7b9640ed625 |
| Tornado Cash Depo 7  | 2024-09-18 7:43  | 100  | 2300    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xba7bd6f80519ce3bfe0fe360fcb4119578e488769ccb9cd9f3d8867112c751b4 |
| Tornado Cash Depo 7  | 2024-09-18 7:46  | 100  | 2400    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x577904b2f10c438e49c1df022f56eef1d84ce770a7a22719dc13394c731d2910 |
| Tornado Cash Depo 7  | 2024-09-18 7:49  | 100  | 2500    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x1eba44cb6fa4f381778ba5f01f95864986bd10fcfbe7b36833d77b30ca55e016 |
| Tornado Cash Depo 7  | 2024-09-18 7:53  | 100  | 2600    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xb587548136061d57cddec70bf1414115a86af7db4faea351c90183e03f9c7225 |
| Tornado Cash Depo 7  | 2024-09-18 7:56  | 100  | 2700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xb7a27accaecf740f7cb6bd8853bfd2ab6dd71eb404d40048a252a8e45766e226 |
| Tornado Cash Depo 7  | 2024-09-18 8:00  | 100  | 2800    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x23a4c175240949cd9042a3868e4a08de0de4e16192eec98ada4e460395547ed0 |
| Tornado Cash Depo 7  | 2024-09-18 8:03  | 100  | 2900    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x7bad007306f3f3edf4c0e237090279916f80eb97519b41596d630586bcbb2ab0 |
| Tornado Cash Depo 7  | 2024-09-18 8:05  | 100  | 3000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x89f383ab3189f3b54d1f9a65a7fe2201b672810e40d5a3964dfefe5db2dc172c |
| Tornado Cash Depo 7  | 2024-09-18 8:07  | 100  | 3100    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xa4837e87dcfbc686fd322befa2f8d9a561a810df795469c28a232b1cf720ad44 |
| Tornado Cash Depo 7  | 2024-09-18 8:10  | 100  | 3200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xe9433e069a6cc30634f49db92cde16456121b58de4fb118a3b909267d727b0ae |
| Tornado Cash Depo 7  | 2024-09-18 8:12  | 100  | 3300    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x6a26a1827260ff308110c5247256500d065b32b5950689bf57c23f499664687d |
| Tornado Cash Depo 7  | 2024-09-18 8:13  | 100  | 3400    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xbaaf96eeafe5b5e37ec273737e742cf039196c46f933356ad0174b958bb8aaef |
| Tornado Cash Depo 7  | 2024-09-18 8:16  | 100  | 3500    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xa4fb3de658c71fceeaa0a4114eb952a076f02311ce848832a2963c291b76178c |
| Tornado Cash Depo 7  | 2024-09-18 8:19  | 100  | 3600    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x45b93ce913ef136ebc88dbc3a16daacece0543204253b1f62c600ac8c9175f7b |
| Tornado Cash Depo 7  | 2024-09-18 8:21  | 100  | 3700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc511db40a755906fe165a84fec8c2193af42a8277359c200a48430776dd3bb49 |
| Tornado Cash WD 6    | 2024-09-18 8:22  | -100 | 3600    | 0x97326e4e9dc051d66c25759f4bc343bb8e1e2be4 | 0x0ccead211629d8b048a8e738c0932a13a3d2f8c339608eae42e44e24012921c5 |
| Tornado Cash Depo 7  | 2024-09-18 8:24  | 100  | 3700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc4e538876f7daf17f7269284a920433fad9b3e07a6f801da1783f3069ddcfc8e |
| Tornado Cash Depo 7  | 2024-09-18 8:27  | 100  | 3800    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xaa60032ae3e76c7e168559d746307416c3fae69e4f66df0e59d42c7729c40499 |
| Tornado Cash WD 6    | 2024-09-18 8:28  | -100 | 3700    | 0x201916690b8731ca39e7ad364690b18103d2ab87 | 0x4ae03ba2c9048c64ce1a4160a205c3077ef1e659afecde09717f26a83032abfa |
| Tornado Cash Depo 7  | 2024-09-18 8:29  | 100  | 3800    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x6144221eac273f47ce9e21e3073cc834112ea363d44bc4121432dd97d312b89b |
| Tornado Cash Depo 7  | 2024-09-18 8:32  | 100  | 3900    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x8ba40a8afd68f25b99ef510e944b1fbc9a682ab4a3195b233833ae20344866db |
| Tornado Cash WD 6    | 2024-09-18 8:34  | -100 | 3800    | 0xfcba540b44d2046fd93b52ba95df0254d831bcf3 | 0xd75f6a1af756fe02bad5c6b44487498cdd55a0a8e0c69019f5f9f48b4ae570fb |
| Tornado Cash Depo 7  | 2024-09-18 8:34  | 100  | 3900    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x1d11ee4e17d1a08f77e10d68de02eb4c0017edbe03c75c1c0c3c22ee8b3b1fb1 |
| Tornado Cash Depo 7  | 2024-09-18 8:36  | 100  | 4000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x13a0206afb750d2a52dfc8a86b25449a5fee17e3d24ff0aa3dcae24975421cc9 |
| Tornado Cash Depo 7  | 2024-09-18 8:39  | 100  | 4100    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xbb53f571b508002b3badb3999cc6c7f9f1dddfbf812bcca9c4c7e6b790098ec3 |
| Tornado Cash Depo 7  | 2024-09-18 8:41  | 100  | 4200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc63f8c703dd3539d23079037055f23b2d68bb27058d1fbdb8ac420cb96e806c5 |
| Tornado Cash WD 6    | 2024-09-18 8:45  | -100 | 4100    | 0xb522f4fe7c839a602b83c86336e521fae13765c8 | 0x9dee04b5e7d0ae70fa3fb46f44cc8c8f2add1fa7bef5a42d20a92e34aad54831 |
| Tornado Cash Depo 7  | 2024-09-18 8:45  | 100  | 4200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc2bfc802b238e27e09626d719018bb24f7753c393b82c4818ac44bad451594ea |
| Tornado Cash Depo 7  | 2024-09-18 8:47  | 100  | 4300    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xd952b54d8b4b3eb0f28224ecddc81b8175bf3a4f81a46ad6b833132b701e275c |
| Tornado Cash Depo 7  | 2024-09-18 8:49  | 100  | 4400    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x13621bb26112ad3013004595798ef2f52489e8aefcd7252a91d081e3dcfefb28 |
| Tornado Cash Depo 7  | 2024-09-18 8:51  | 100  | 4500    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x2c18953ebe72873187bce212c42b1a9fc2b2e7438a7bd5a4dafb2355bef192cf |
| Tornado Cash Depo 7  | 2024-09-18 8:54  | 100  | 4600    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x75555be3f32dd18da5f0b5263f0c2c591d1d78d3dc675850cf5927f064eaec72 |
| Tornado Cash Depo 7  | 2024-09-18 8:55  | 100  | 4700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xd84a98b90317b58c9c6d8f5c871bc519182d682fa9eb115433f0e94ce58aad74 |
| Tornado Cash WD 6    | 2024-09-18 8:57  | -100 | 4600    | 0x06810c99cdbcd0d3cc69d9bbfb84cf950e733514 | 0x65d99bc1a57b9629b1bd8d52574287b9030499f6f458ce1d5fa39442ccce6f45 |
| Tornado Cash Depo 7  | 2024-09-18 8:57  | 100  | 4700    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x59abbfa3726c8d7838e34dd50a9a0e988cda42a11ddd9d2f37cc2beba2945f85 |
| Tornado Cash Depo 7  | 2024-09-18 8:59  | 100  | 4800    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x1a8d2c8816567ff657759b0c482fb68991fbc008291b55fbc1e7e548aa775e9d |
| Tornado Cash Depo 7  | 2024-09-18 9:03  | 100  | 4900    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x4fc8cb9aa36c2a36e8c3f5239632710c8784c2e779203f956c23236d7f1d9e4a |
| Tornado Cash Depo 7  | 2024-09-18 9:06  | 100  | 5000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xda45bd3d2c1d4951d7623fdaf18b149ed726b316f31301c357b3155391a5c863 |
| Tornado Cash WD 6    | 2024-09-18 9:11  | -100 | 4900    | 0xc84da11908e63e4f3a48227928374eff6eb8552d | 0x90b1b3ad43cfe1c9e8acb091a703b59e48758a664a2d304d82eeefd793c741fc |
| Tornado Cash Depo 7  | 2024-09-18 9:11  | 100  | 5000    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xbe047f03928fe3dba8447f387ee599cd1a0d11723b32bb7a5ba1cfe06b234e7a |
| Tornado Cash Depo 7  | 2024-09-18 9:14  | 100  | 5100    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x3936682d5858fbe0f344361ac195a6d3cebc329bdc08bed9061de27f2c0f9af6 |
| Tornado Cash Depo 7  | 2024-09-18 9:17  | 100  | 5200    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0x8761f989913f1de783d9c410e9b21d9d6e685c63d358d41477f89a2202a9068d |
| Tornado Cash Depo 7  | 2024-09-18 9:21  | 100  | 5300    | 0x5990c7e24816bd103982b02e82ebf3adb49b6a6a | 0xc87c259989bc403b4c3d29090eaa614c608c6fcb3bf12c6a91ce27efc0a396c1 |
| Tornado Cash WD 6    | 2024-09-18 9:26  | -100 | 5200    | 0xb6394c3422fbc703a7c4f2bcb315d53d21228692 | 0x6f989d2aa15f967f5b5cc4618cd12a8b1d136387a2f9dc8e8081f5ea76b7da7b |
| Tornado Cash WD 6    | 2024-09-18 9:35  | -100 | 5100    | 0x79ed1cdac2e340dd624de0ad1b9235fc7103dcbd | 0x870e7985453c90f84645d6d97b438006d623b13281fb676f1515ad6685e8bb00 |
| Tornado Cash WD 6    | 2024-09-18 9:49  | -100 | 5000    | 0xcf571d132227c25d8afd6c887aa06fd730f39ebc | 0x75fa05092bd653798d2d43a04b10406f5ddd186e92fa2a9cb3bd652c2e24a087 |
| Tornado Cash WD 7    | 2024-09-18 9:59  | -100 | 4900    | 0x81c288f2b53c26cf67249f2116df5187b1cb6b8e | 0x9dadcd8dc0e923b95f3f4d9723ab2cf7617432f957c7b02dced7e4045fbca43c |
| Tornado Cash WD 7    | 2024-09-18 10:20 | -100 | 4800    | 0x1d98e0ffb6fb73e2d7952892d685ce440b53722c | 0xdbc5d3e652f5b02345998a7a1859c93dde4305d1662397362008a9de6e817fb8 |
| Tornado Cash WD 7    | 2024-09-18 10:32 | -100 | 4700    | 0xf3b14da38c165915bd4add9fcd206a7f07385744 | 0x03bf8a752caa98da678e5d755af41f62471dd22984004a3df11d7281a00d07a9 |
| Tornado Cash WD 7    | 2024-09-18 10:44 | -100 | 4600    | 0x98e3883eb455894eeddd29131765fded523aaa9d | 0x86dd19248bff743d5372ad9459a8f7c468f1b43d11fe54381000c613836809b8 |
| Tornado Cash WD 7    | 2024-09-18 11:03 | -100 | 4500    | 0x7cee5c109f93236109d0095325736ee8ddf675a0 | 0x5800faa1f30a2a67195bcc16a856aec99af544d6d91411089275812285a9a5f9 |
| Tornado Cash WD 7    | 2024-09-18 11:20 | -100 | 4400    | 0xfd0986e106a1ef39c33e5c295c3d9a1234e4f653 | 0xa1e88a7fe53f2ac019e60e7cbfa15f580d469f7ba8d64fbf078b9397e901557a |
| Tornado Cash WD 7    | 2024-09-18 11:45 | -100 | 4300    | 0x755f3b53346f81e5391467295ef4aa322e02cda4 | 0x7fa1e52ecc39636eed3331d353d5723a681c808ba0e8a2f16dc76fb463f933b6 |
| Tornado Cash WD 7    | 2024-09-18 11:54 | -100 | 4200    | 0x9b531a7fb45f6db89e17e025a33fa13a2965138b | 0x3a4b43ae0885114bbe9ec17f080b715e3cab56896f25483ed047659fe0aab4e6 |
| Tornado Cash WD 7    | 2024-09-18 12:09 | -100 | 4100    | 0xe80fed7113af98390c5719e60009bfda40ee1566 | 0x0922ed3697f3db6e884bd97714ddd3b9258867a69548f4101c4231e013603311 |
| Tornado Cash WD 7    | 2024-09-18 12:21 | -100 | 4000    | 0x33de13ef77d603349ebd5c6ed7a41530ca5caf9b | 0xb05c54897c11d50e9532cce1b90d50583db4c28f9514cadc722212da8d11edf6 |
| Tornado Cash WD 7    | 2024-09-18 12:35 | -100 | 3900    | 0x7f78d6d8a57fb3e9ae839b5010fa87e260fa759f | 0x548bb760c8d9e0287865e60919aecf859220550e416c1ee19041ffd8a93bca84 |
| Tornado Cash WD 7    | 2024-09-18 12:53 | -100 | 3800    | 0x5d62f617ff1418b9756eb736548771ed8b7a3516 | 0xe6124749f58c892e3ebe4f74a6ccbb723eccce45e5a72cacf6255473f997d5b6 |
| Tornado Cash WD 7    | 2024-09-18 13:18 | -100 | 3700    | 0x60a152c0f0c2dd6068d588f42027352bee593ee8 | 0x030953dd20630ce2396462c12741072195b37e143afd8e4a709e1d259babb852 |
| Tornado Cash WD 7    | 2024-09-18 13:29 | -100 | 3600    | 0x8ed2058166e3cb65131b2aeff889b641450b4f01 | 0x1e8aca470f4253e7e92feb9147f2b3e4a96a17ef34c9ce9bc2b3ccc7d5764347 |
| Tornado Cash WD 7    | 2024-09-18 13:37 | -100 | 3500    | 0x198d7e11ba4967144d509b8ab19026e3a79c452a | 0x16cb20479c4861f9766f039375ae9ebc317b12e9c3926cab4006ed02ada01013 |
| Tornado Cash WD 7    | 2024-09-18 13:51 | -100 | 3400    | 0x3177af4edd3c939f381cc29b4dea6ba73a99b73f | 0x7280dcc75ff14ec2e8b9e8b27f7eac84abfcfc22394b0d9fdacc68b35ca903af |
| Tornado Cash WD 7    | 2024-09-18 14:08 | -100 | 3300    | 0xd89187f929a4e8081d23a71a25f3848c33340886 | 0x6d6638ff4eb68473f5a500dc53b415bcb81524c245d5b5a871ec9488da112b4d |
| Tornado Cash WD 7    | 2024-09-18 14:21 | -100 | 3200    | 0xb93f02ce87168457893e4654ffce31f6d3247d87 | 0xe1d2b9cc6baf1e7b9ecd8e813d6734022d22e882df58bc0aec4e5fd2a628a513 |
| Tornado Cash WD 7    | 2024-09-18 14:30 | -100 | 3100    | 0xd9f14535c9f27f98b9b988002df8e62d5d59ccd3 | 0xa2a94fa1bbb4aa0d808b0c670d094c320ee20806544d85d0b052290c96049398 |
| Tornado Cash WD 7    | 2024-09-18 14:39 | -100 | 3000    | 0x24601cc4295a5b0118426da0a2c3f5b5337e8d01 | 0x6b526e7c52efb2d6de73bad757a3f648adb87bd2e38b585af4063fa936635cce |
| Tornado Cash WD 7    | 2024-09-18 14:43 | -100 | 2900    | 0xddc015433f64b35da01b411c452701894c469357 | 0x7aef2745fc9e73559443d700046ddc73d013ba0236461102056dba340c69965f |
| Tornado Cash WD 7    | 2024-09-18 14:59 | -100 | 2800    | 0x7e80caaf9d8d2a0ad82e532184fdac0467d72eb1 | 0xddd02ddb12581e2216e52bab0ec339141770ffdec3928aadfb2bfb3ba9c8f1c2 |
| Tornado Cash WD 7    | 2024-09-18 15:04 | -100 | 2700    | 0x9bfd4c868fee7ee982554079cf1d12de917e5425 | 0x1b5b4382afa5d72381c44f84ba171a26386e7bb955a30214a0a778d5e2c4530d |
| Tornado Cash WD 7    | 2024-09-18 15:22 | -100 | 2600    | 0xed36d96f5c4895ba0b013e3d1d5ec9c31a410db7 | 0x90c91fc20491d52f69cb6b55c9683565c099470e989678ff55672c8de4217c67 |
| Tornado Cash WD 7    | 2024-09-18 15:34 | -100 | 2500    | 0x4337d577f7a84ba51fc4ab7ca22327ef711d866d | 0x669b808dee2129604151c198ba4ee84af690570cc21738eb72c6db604456faf8 |
| Tornado Cash WD 7    | 2024-09-18 15:39 | -100 | 2400    | 0x7dee98d6b875aab9f660797bef3cdcb620b0199f | 0x891635bd7c036913a7aa7425cefe4adf6782907291f71b19ace3d0509ecb88cd |
| Tornado Cash WD 7    | 2024-09-18 15:52 | -100 | 2300    | 0x7dcc98a165e34baee566c31127309711320e9211 | 0xdd99e0140e8e6f71ebe8f6ea1fbf4adbb1d5b9e419b6d2bb86d09aa49eb614b7 |
| Tornado Cash WD 7    | 2024-09-18 15:59 | -100 | 2200    | 0x09de4ef5fe71f07ca2d7d570f29008a223ecd598 | 0x8685e711f6eb1e62706e590e528f88e80480fbc624e5dcd09f9499b265eef903 |
| Tornado Cash WD 7    | 2024-09-18 16:07 | -100 | 2100    | 0xee8b3d4fefb1b37e39af50c4cf036c1a8eecd45e | 0xd929267dcc6973b8fb231de3047b1b04186f2baea486bdef02b0be6972187fc1 |
| Tornado Cash WD 7    | 2024-09-18 16:19 | -100 | 2000    | 0x2692eb0b4b4a7d4f7df2e322819bbf5ca1ea0859 | 0xe840931fffd83687f05fe9a82923c6f5dca9b3c23ac00f3a1a36e48ab3b3a562 |
| Tornado Cash WD 7    | 2024-09-18 16:32 | -100 | 1900    | 0xbb469e1d0e92bfe08aea69a1a5d54ba30e03276e | 0x98cdefc511a1d71859553f485b239a70623a4adb422191fad9242bc455cbbe9a |
| Tornado Cash WD 7    | 2024-09-18 16:46 | -100 | 1800    | 0x55aef76900daa727f45789bcfcab0504965dd28d | 0xcbd2327240b0803eb5468dd5f5a31dc2da36078a184560dcfc28a4ce41892153 |
| Tornado Cash WD 7    | 2024-09-18 16:53 | -100 | 1700    | 0x23455954f3728f9eb248891ed11f6d42e4f9cfc5 | 0x9cc634499bbab36b7ee8d2d7b799ecf41296797cd7c8ef15d6941cbe93b8b627 |
| Tornado Cash WD 7    | 2024-09-18 17:11 | -100 | 1600    | 0x1f6793b7cca4e057266259336443e8560f108540 | 0x451fe633344ff61817ca4613241856604423c14b84f5d1314a1ad76bf642c9c2 |
| Tornado Cash WD 7    | 2024-09-18 17:23 | -100 | 1500    | 0x052194f17aad2a46155b7b7f83354b94fe892339 | 0x29ecd86e5c4131fe1d7a423841ea17a18eb353250d64f9fe749fce74b86a5615 |
| Tornado Cash WD 7    | 2024-09-18 17:40 | -100 | 1400    | 0x6f3331f755575d7bece19dde014856bcdd6a9d3e | 0x2f470f458860a0d9b108e2941bf6533a013bc9bbf1855d17a20558e842df719a |
| Tornado Cash WD 7    | 2024-09-18 17:46 | -100 | 1300    | 0xd11612ecfd734713f150073b8f4313a6473feb7a | 0x7590ae454cc809b12c309874abef7417e082fff88d3b58824e37637d320c93b4 |
| Tornado Cash WD 7    | 2024-09-18 17:57 | -100 | 1200    | 0xe5925eaec89d1574750ce5e7aa2dac4559bb2864 | 0x4df43f2b772e9037fbb56dd906b6ebf4b5f47459f61c06c8267770d2ffd9668e |
| Tornado Cash Depo 8  | 2024-09-19 6:29  | 100  | 1300    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x3ce8d070b85ae252195ecfcfee7986ee052ef911e76eb101de9b45a8373d2c31 |
| Tornado Cash Depo 8  | 2024-09-19 6:32  | 100  | 1400    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xb2f2afe1cc0a20acd34335c7d953490bfdad3047d5fb496716afb0f84864fe58 |
| Tornado Cash Depo 8  | 2024-09-19 6:33  | 100  | 1500    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x7476d3e047198b059c7024afe42a00fc668b076b3b9ceba0c1dcb6fce1f95739 |
| Tornado Cash Depo 8  | 2024-09-19 6:35  | 100  | 1600    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x94228bccd710a8e083b27ef7baffacc64e05806f7661bd13f6c8edaece569ede |
| Tornado Cash Depo 8  | 2024-09-19 6:36  | 100  | 1700    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xc50399a204561d6f2c5cfe211dbb8feb7ec7dc874a3bc6e1239619402565c271 |
| Tornado Cash Depo 8  | 2024-09-19 6:39  | 100  | 1800    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xcd7464f8507c5a1065e9ac179097e761234aedbee90b71413ec5661f5d5e9f4e |
| Tornado Cash Depo 8  | 2024-09-19 6:41  | 100  | 1900    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x5d8a0b8e59d3b09e2c049b40b4d6cdb097a6e5a668dafb48fc3ebf869c83bca6 |
| Tornado Cash Depo 8  | 2024-09-19 6:44  | 100  | 2000    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x46bfe2fcdf5c758417b5500b427d8edfc0afe7c75709b6312d661ea7ffccb501 |
| Tornado Cash Depo 8  | 2024-09-19 6:48  | 100  | 2100    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x8d5f2fba5c1875ea4777f40133a6c95247b0e02541b26cb4eff8f887c116f8a5 |
| Tornado Cash Depo 8  | 2024-09-19 6:50  | 100  | 2200    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xf055b6092511462305f0853e47ff62339a07e7464fcf0a5f4613ed5d1504ee10 |
| Tornado Cash Depo 8  | 2024-09-19 6:54  | 100  | 2300    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x5746342115822d64e280a4f8085cc76002f1811345fc1941af2144a59beb3187 |
| Tornado Cash Depo 8  | 2024-09-19 6:57  | 100  | 2400    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x32992cf720ccdbfc9632c7ef30369d9e00349683b8cf5dc19b09bac31520f045 |
| Tornado Cash Depo 8  | 2024-09-19 6:59  | 100  | 2500    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x6fa9ded8d12d665cab98ec180430ef15a48b8566e9e72caf83d8d518e8e7a4e4 |
| Tornado Cash Depo 8  | 2024-09-19 7:01  | 100  | 2600    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xceeb26720caf1ce4530b3ce68b1ebd486394ac0d0e1b2a2baca78ecff7b2db27 |
| Tornado Cash Depo 8  | 2024-09-19 7:04  | 100  | 2700    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x553a0966b5693872dd3b504e20163d44b788486ec996eacda9718beab87f286d |
| Tornado Cash Depo 8  | 2024-09-19 7:07  | 100  | 2800    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xfe9d9800235ae9289af9638a3679a7ee8bf89d53341bda92c16ea8947fb3fa14 |
| Tornado Cash Depo 8  | 2024-09-19 7:09  | 100  | 2900    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xa420ec304069a0dcca7367a31c5c9384153b98da2cefe186e22becc20e731201 |
| Tornado Cash Depo 8  | 2024-09-19 7:13  | 100  | 3000    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x1e537efd3a9fa567cbf765398c62e82bd31a6848e872dc33e91dd2c2d144ddbd |
| Tornado Cash Depo 8  | 2024-09-19 7:16  | 100  | 3100    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xbe3f05b6994bda43f5b0c64a95cdef155c2a4d091179418429705f8c9802a6eb |
| Tornado Cash Depo 8  | 2024-09-19 7:19  | 100  | 3200    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x8ff6632bba8a61089d1b9a407ce837376dfa1910ba380bd47b12a7b1603e28c8 |
| Tornado Cash Depo 8  | 2024-09-19 7:23  | 100  | 3300    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x626580a46076bf7468b37e764e7a45f417e174b4d8e0ed5a76368e571e4dd8b9 |
| Tornado Cash Depo 8  | 2024-09-19 7:25  | 100  | 3400    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x95be472088b3a0b58e133f31b28b9352d97d1cb748c2172b40266146be0d7a8f |
| Tornado Cash Depo 8  | 2024-09-19 7:28  | 100  | 3500    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xadcb0a416e7f433f740627f53878891a287f4f2dd8c0862eef6d2de91f8f9cb9 |
| Tornado Cash Depo 8  | 2024-09-19 7:32  | 100  | 3600    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x00a732d3cabb9032e85dff0ef4155849438c02163b2abbe53d6659cf66aa0c81 |
| Tornado Cash Depo 8  | 2024-09-19 7:36  | 100  | 3700    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x595ae154437e238864007e4702a3476c4b6e9fb4325af715ea0961c649b81c17 |
| Tornado Cash Depo 8  | 2024-09-19 7:40  | 100  | 3800    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xec1bd07f39be7b3241aff3da677b0842178a9225ba8094eebf34df9b7aae425c |
| Tornado Cash Depo 8  | 2024-09-19 7:43  | 100  | 3900    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x2df17c37e33be4098f4994c8bf8cd33a7da3f19bbfc5fc39d8cde7bc6fafd0c9 |
| Tornado Cash Depo 8  | 2024-09-19 7:46  | 100  | 4000    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xb7cd150c6a45ba837b88e7ab2f07cbab07fdaeb0b80186f17becdf6e51228908 |
| Tornado Cash Depo 8  | 2024-09-19 7:50  | 100  | 4100    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xb2a2bd6a6fa11017a0eba823aabd750e6c4cdedfe136116e36425d16f441cf5d |
| Tornado Cash Depo 8  | 2024-09-19 7:54  | 100  | 4200    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x4e87798551bbd46bcf74bf79c21315b25601f613537adbd438fe07f0bc54824f |
| Tornado Cash Depo 8  | 2024-09-19 7:58  | 100  | 4300    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xde5d1d24369d9d291cdbc4407eb7db5b63d7e22565d67312432b030b43d92275 |
| Tornado Cash Depo 8  | 2024-09-19 8:01  | 100  | 4400    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x2531477f3ba75b692a35f664b5b44cf0fa5db10525a41aa9004a4104f396f057 |
| Tornado Cash Depo 8  | 2024-09-19 8:04  | 100  | 4500    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x8778893403223f78c0558af9611583118d970143ee7d8eeec9877e96bbe61c3d |
| Tornado Cash Depo 8  | 2024-09-19 8:07  | 100  | 4600    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xf27df819568b74586bda4bb8baaa58ae65e6af52c9e211ccede53068a16730de |
| Tornado Cash Depo 8  | 2024-09-19 8:10  | 100  | 4700    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xdffb63b2fbcd6a69c284cbb8d49ada19d7cc358463c97fb9ba2836dc2563b3a1 |
| Tornado Cash Depo 8  | 2024-09-19 8:12  | 100  | 4800    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x57ed50def775181954f17324521d9fe07bd848c1749a044e985945b1fc61c11c |
| Tornado Cash Depo 8  | 2024-09-19 8:14  | 100  | 4900    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x77933bd922dcae72ed1982ea31c9eed574f2b332e9172f8c610dbf64ec872f5c |
| Tornado Cash Depo 8  | 2024-09-19 8:17  | 100  | 5000    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x237fe20d4f0bd36af8f4b940aaa5723782896cad45afaea665898ffbce3fc115 |
| Tornado Cash Depo 8  | 2024-09-19 8:19  | 100  | 5100    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x421e9455ffd14622ac441c4485f6a976994c2c26f114ecf59f6eb9a6cb15ced4 |
| Tornado Cash Depo 8  | 2024-09-19 8:22  | 100  | 5200    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x86b6652cd08b166cce82fd7e09c40042136d1a69f38622969d57840da25c1350 |
| Tornado Cash Depo 8  | 2024-09-19 8:24  | 100  | 5300    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x3bbf456a045b9ca8e732435132295b75d1310830bd0d305c19bd1e268da48789 |
| Tornado Cash Depo 8  | 2024-09-19 8:27  | 100  | 5400    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xd1364fbafe84ed5cbdb5b47d8f6e3a734f33a0a4a35f092c24b516a17509d730 |
| Tornado Cash Depo 8  | 2024-09-19 8:29  | 100  | 5500    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xc651c410fea5586056302fa3588f9a3e8a1cbaf9005ff71de05028a9e33b3780 |
| Tornado Cash Depo 8  | 2024-09-19 8:30  | 100  | 5600    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x3f4d035c0c1d6077721e8c2a8dd7c61a35d9b618f5f0a9c0e00a5cd45aacb22a |
| Tornado Cash Depo 8  | 2024-09-19 8:32  | 100  | 5700    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xdf47271ed39a65c2af7c5f84366ca5cf87792785e2b26aabf879714a4000f181 |
| Tornado Cash Depo 8  | 2024-09-19 8:33  | 100  | 5800    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xc9550cf4232dc41cd6d9bf32c7e5fd674f0bfc34fbc9d96c96c7595047b07f0d |
| Tornado Cash Depo 8  | 2024-09-19 8:36  | 100  | 5900    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xb6dfe01f394223aa8881f43010553a3bd826eb13dc7ea7300600f5ff3c5230d0 |
| Tornado Cash Depo 8  | 2024-09-19 8:38  | 100  | 6000    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0x5155fbae76751db6134c9668d93df9a1b2aa6cc35b3fcfa797f8e308b91a0620 |
| Tornado Cash Depo 8  | 2024-09-19 8:40  | 100  | 6100    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xf0eb1a50c1695517881df6ad81bff70d625c6cb0622e461a0ec1e2fe2daa4b7e |
| Tornado Cash Depo 8  | 2024-09-19 8:43  | 100  | 6200    | 0x46b9d6f8424eb8075bfaa28127446e5b38340a0a | 0xe57fe3cfe0ad4609c97a08e0a2178af6916757da817e47a847ee9e53dfbacc49 |
| Tornado Cash WD 7    | 2024-09-19 9:03  | -100 | 6100    | 0xca85e50558e4319fc861a6a0c3220f5015f2789c | 0x2629333e2e6fd2260fa2bef447bb02a1426a93bd03c1bcb6baeb3e1cf6cac5fa |
| Tornado Cash WD 7    | 2024-09-19 13:12 | -100 | 6000    | 0xb218dbb8287900fa819490fb8952a1f742271cfe | 0x38f9188b73a0f2f8db4d3dcbf18f06f6fddfd72aa5ba801e073a4c098994854f |
| Tornado Cash WD 7    | 2024-09-19 13:36 | -100 | 5900    | 0x9698f51bc5e96f2a8e05422388555aeade76c845 | 0x104d1b436e78d9d7cc5420414ae879e876faacdbab54d63bba6d49ca33181d97 |
| Tornado Cash WD 7    | 2024-09-19 14:02 | -100 | 5800    | 0xb6a580f1cc72ec9ef1c104211092e086940e934f | 0xba4f55593d0215421e1ead11e93e43174709d2b7fc36ed996fbbcbfeafe460f6 |
| Tornado Cash WD 7    | 2024-09-19 14:33 | -100 | 5700    | 0x01a9111cc503b9977ef2c888d956beb48a249a20 | 0x0f9eda828bb99feaaf0b9fd48dc610507c39f232e4e2b229c74cec1c7e46dd42 |
| Tornado Cash WD 7    | 2024-09-19 15:06 | -100 | 5600    | 0xc1ac5d46ef4fb6cf926ce1590f9a8f537f9c8943 | 0x62f6466bb7befa064a8f5a8e94c4700aad424600a9e9c87ef6125bccb1f07cc1 |
| Tornado Cash WD 7    | 2024-09-19 15:34 | -100 | 5500    | 0x804e31705491770ebc476d4b0599df255d5eb15e | 0x2679cf94ac0dee74834a68a2ca246472aee9c5170f19e11c8f97d59a219597b6 |
| Tornado Cash WD 7    | 2024-09-19 15:38 | -100 | 5400    | 0xfe0ce8d939e510eaed46366671920221c71771a2 | 0x6a0bebf1631136fbc9d803ec8bd1a4867d611961788f63efd23d667eea684f77 |
| Tornado Cash WD 7    | 2024-09-19 15:53 | -100 | 5300    | 0x7b5fdbbf731f3cd80a1ef0327a203dbbd4d6e0ef | 0xcdcb66f4445e57a62c4e4d67f2cd0b4a0b528e123580dfe6dca8efcd984ff0ad |
| Tornado Cash WD 7    | 2024-09-19 16:11 | -100 | 5200    | 0x2b404660164343b6a3e2cd94e6ebe112be06af2e | 0x08cf93fc8aeb8446c7af79756cd79e64e572250121c816bb052390da7eed114f |
| Tornado Cash WD 7    | 2024-09-19 16:27 | -100 | 5100    | 0xac4d1ef28faaca846eb078fc3b59a73a624a67d6 | 0xfc91ed703c03330a7bd7792b9116501a6ba3830f4dbfd462cc783858a5677296 |
| Tornado Cash WD 7    | 2024-09-20 3:56  | -100 | 5000    | 0xc2738e31660c9a9b6ac456659a20f86ea77d2058 | 0x3fc6022cc27d1613c68ccd48fc7ca7955755d5ee763ce5c614e389032ac572bc |
| Tornado Cash WD 8    | 2024-09-20 4:01  | -100 | 4900    | 0x49c41326f8d58cb86ca2dc867c2ee734c29c3419 | 0x2656c90f490dbee642f87136964bcebaba969e08d8d0277cc379b573861f1b73 |
| Tornado Cash WD 8    | 2024-09-20 4:14  | -100 | 4800    | 0xf19eb318b7dd12d3f6fc0ac4a11429c618435159 | 0x8ff2e9b5deaf81a896a3b4f04284284e0ffa7363a036b5fa12ad4e6316d16c2c |
| Tornado Cash WD 8    | 2024-09-20 4:27  | -100 | 4700    | 0x3caf269caf892d0b81d560443f4192e7710dfbfd | 0x028b28689227026b507aed5f5e31f4c29336b87b5dd2dcf275842679d61836a1 |
| Tornado Cash WD 8    | 2024-09-20 4:33  | -100 | 4600    | 0x9b738e7df48cfb3ea663bdc4af764929092e4b6b | 0x436c920724def9ba2e194b4c47fba08bf3b6eaa03b8e83ce3aacbc77bc9c0d2d |
| Tornado Cash WD 8    | 2024-09-20 4:45  | -100 | 4500    | 0xc8186f97d54e4235401a5a515ef2b6be770ea8a7 | 0xb4838e75e41d46414d190dcc1d4fb50e807dd44bbf1c4f08f5fe18cb767bb7ed |
| Tornado Cash WD 8    | 2024-09-20 4:58  | -100 | 4400    | 0xf67448b7d0aa69e147d8b2b4c690cbade513d8cf | 0xada0459153572e253b16ddda61af8a1a360eaa1b2d72367ae422238eb4694bf8 |
| Tornado Cash WD 8    | 2024-09-20 5:09  | -100 | 4300    | 0xa3cf6ed0fac70d5677dae39c8ded07d07f88092c | 0x96ca8551155b5769b2e12f83c322dfd90fb6e11c08a98ad62f2cd7cb1eb14250 |
| Tornado Cash WD 8    | 2024-09-20 5:19  | -100 | 4200    | 0x21c30e720e38bd59610c19ed3f481be01b69fa9e | 0x0f8c65c46b659c895f3c645eaa0532b3de4559b6b360f163902041672357724a |
| Tornado Cash WD 8    | 2024-09-20 5:26  | -100 | 4100    | 0x48bbef7bab92fcba7dc37c6be4241e2eeafffcae | 0x8161ac4ed854cc463a71a714af14b9d1c4fc233cc71a596dfd4901e847e0a1ce |
| Tornado Cash WD 8    | 2024-09-20 5:34  | -100 | 4000    | 0xdfb64afa632fae3392d81951f1a603c78630c379 | 0xd48d4c8dd9cc744cd7996e309cdb5bcb3bc2728bdf47ef4c88537f8e027762df |
| Tornado Cash WD 8    | 2024-09-20 5:47  | -100 | 3900    | 0x475dc1adf826bff32f2b98bf872bfc753e005da8 | 0xf3758a77f472a56d1d125bfd13c6412c72f321a378e04bbf0ef8982a3b554ece |
| Tornado Cash WD 8    | 2024-09-20 5:56  | -100 | 3800    | 0x3bfd2395d08094fd9e3d87d0c2578599dfd3e8d1 | 0xd8a6b85d752d11dd0cdb5c265abd2f17643ccb544c0aa59a86a4291e9f416c13 |
| Tornado Cash WD 8    | 2024-09-20 6:07  | -100 | 3700    | 0x5840cd76591a7f70c5b6530a8f288dbe094f6fb5 | 0xa9499fb034c6362fab520cb2f4f8b16296ec58a4f847d9073437ad6e71cda102 |
| Tornado Cash WD 8    | 2024-09-20 6:15  | -100 | 3600    | 0x299d9d57da813ed506e51369652682bcc4d02010 | 0x9f33047d8bd26bbfd291c593aee051c30bd6b3544f83d10757c92fc624e5bf3b |
| Tornado Cash WD 8    | 2024-09-20 6:27  | -100 | 3500    | 0x7bbdd090c86852345677966febe3d02897a816ef | 0x9ec557dc90db7195f9ff1d030eb76b564d2c6d204ef95852dce9bf74f03c4f0d |
| Tornado Cash WD 8    | 2024-09-20 6:35  | -100 | 3400    | 0x093dc10027ec09c32f7f5f623bbd3c9d26d27db8 | 0xc647f21343c6fdd7eca083d09608f13e6298517c70d9ca8dfe83ea9d963a66b6 |
| Tornado Cash WD 8    | 2024-09-20 6:45  | -100 | 3300    | 0x0bae9ff6d2d5561ea6a996b28171e5d41217c079 | 0xfa7b2c29b5d7e3fd6fe2941c542f3ab3ce902a56427d99561ad0e7e2a7367f82 |
| Tornado Cash WD 8    | 2024-09-20 6:55  | -100 | 3200    | 0xd531bad2230ba08bd2e323d9c1c50a5bdc5f8d38 | 0xecb25924aedf41fa1a9623dd9ff56452e72134a2f5ae88d7dc9e4c59fec7e39b |
| Tornado Cash WD 8    | 2024-09-20 7:08  | -100 | 3100    | 0xbb41814c0d922cb7f12231ede83c0d4db0168494 | 0xe0abaf9582c6ef38ca348b6ef75bf3df9000582b4f75bf5ef94ffe37e2cd11d1 |
| Tornado Cash WD 8    | 2024-09-20 7:18  | -100 | 3000    | 0x2cd8d674db9c2b5ca2adbdb64bf9c765de052b6c | 0x62e266950790521b804a0b46bb3531f987fc622cacbf1d40038799014f30d2d0 |
| Tornado Cash WD 8    | 2024-09-20 7:28  | -100 | 2900    | 0x809177fcea7c594ed4861b7e4d9c6cc07e38ddff | 0x1bd478bee2ea93ff4d5538393b63d5d26b9d06a86221f32e12d8617293cf24be |
| Tornado Cash WD 8    | 2024-09-20 7:50  | -100 | 2800    | 0x1e54c84e5a12de8815f5307eeec63f68b0a66350 | 0xabdf969e797c70b5a16713fb97639e8bff21cb7525fe619106fbd528ff74c103 |
| Tornado Cash WD 8    | 2024-09-20 8:07  | -100 | 2700    | 0x140621b4079aa885439d3066a1defc833820566a | 0xe08a1886bd5c6b055bb797f411c7f5a339485e94a22060f0da00e5ef64248f8b |
| Tornado Cash WD 8    | 2024-09-20 10:57 | -100 | 2600    | 0xd5d886b595f7cfc22fb13590a8455b338a21e43c | 0x3ae131cbac94cd9313c1c192d3110a5eadb88b240fc5f4f617aa496ee269f064 |
| Tornado Cash WD 8    | 2024-09-20 11:14 | -100 | 2500    | 0x5b275de98b075a08dbeb09dd41040f52708709be | 0xec389193aa8022a0a1fcca006917de4ef2793f3b53206aa02963c2c94a5d3c06 |
| Tornado Cash WD 8    | 2024-09-20 11:33 | -100 | 2400    | 0x9109e567c2086905e0cd1f90b52110ba61966466 | 0x6aa670340a033e4f419abf03ff73609571239e3c43a43cc5bf17946e1506e1a9 |
| Tornado Cash WD 8    | 2024-09-20 11:44 | -100 | 2300    | 0x3f536024012c43aed4434f58a0ef02f54a32c630 | 0x5f5d30b3f637f37ec02721c8fbdc0ed5963d67c0886b394fd3c265ac9bd4bfee |
| Tornado Cash WD 8    | 2024-09-20 11:58 | -100 | 2200    | 0x5081ff1818f6465ec9c735a8df9bee6d25dd76a4 | 0x812019430eef583d0d70a4aacd7120872918a7dcff9363597d62ab4a88927794 |
| Tornado Cash WD 8    | 2024-09-20 12:12 | -100 | 2100    | 0xb55ed1f3387f6316891bcefee38cd60ba213a8cd | 0xcc542dd82715601db60d2a10fbaa8a3a5dde2b606af32343e6c256294eea4d38 |
| Tornado Cash WD 8    | 2024-09-20 12:22 | -100 | 2000    | 0x64e52498ed84e03b1c1963df9a40ec3ddb44fd8f | 0x82150613410ae90393f5f7a319460b8a61422ae1a9a87627810cd5f0a229a85e |
| Tornado Cash WD 8    | 2024-09-20 12:37 | -100 | 1900    | 0x371561f6f7b80a41f83d7c84dad3fc16520cdece | 0xd21c98773774bfabc7f2ce68a47c3833999d1c7c3f2217bded8257a87b766d17 |
| Tornado Cash WD 8    | 2024-09-20 12:52 | -100 | 1800    | 0x528ddc867c07dbc2be7300b9980a8a8cc72f9891 | 0x6928ff5890028630b927f67a2ee926c97249cf8d66dcd8adfaf2261d6a8e8068 |
| Tornado Cash WD 8    | 2024-09-20 13:27 | -100 | 1700    | 0x63b38190b4803df5e579ae5b1b5e1f7189cc104e | 0x0cc3107d149f8dd658933652ef9cf7f22336bc6049aa9eb23eccd59edfb8c044 |
| Tornado Cash WD 8    | 2024-09-20 13:43 | -100 | 1600    | 0x1a6454cc345371d834bb8142dbb2a026241f912b | 0x6767b8c76795d985937f9b49b16828c7d1f4fa03bd1cde734dfe528fd3faf531 |
| Tornado Cash WD 8    | 2024-09-20 13:58 | -100 | 1500    | 0xcea1ae20785a063d80112dccea50b80ebef55a28 | 0xe321ed03c09964dab71e039f9bf65d662c81ba3339708b134b799b1647483022 |
| Tornado Cash WD 8    | 2024-09-20 14:10 | -100 | 1400    | 0xd9fde6f6dfb17e8b91cdffbfe650e6708b86e2ed | 0x6cb061a6ec514cfc87766a8831db1c331393c7752568f98f147a43a40f25daba |
| Tornado Cash WD 8    | 2024-09-21 9:08  | -100 | 1300    | 0xf0321d6a59629966c09ac928e21fd47dd5ae02f2 | 0xec1bcac1108822165555ed900c913672b822c118ca2212ca358cce1810242384 |
| Tornado Cash WD 8    | 2024-09-21 9:22  | -100 | 1200    | 0x57ba188567258f1eec8144e570588adfbe7bc5ad | 0x71f9f3b5f293e57780b720ed59f85b47faf7188c71e32b05cfb85df6b62f65e9 |
| Tornado Cash Depo 9  | 2024-09-21 9:25  | 100  | 1300    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x1fb7c78cf4df063d79ff2808253b7494d55980a0a23380cbaded8a43fffccc3e |
| Tornado Cash Depo 9  | 2024-09-21 9:28  | 100  | 1400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xa3b074e227264ca08794391f6e8f5dfeb0554e10c8cb633da21a58f545dace02 |
| Tornado Cash Depo 9  | 2024-09-21 9:30  | 100  | 1500    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x0af924fbc6f82890ddc8806f28b3a76da3e644aef38f34c5d4bc537867b41cc1 |
| Tornado Cash WD 8    | 2024-09-21 9:32  | -100 | 1400    | 0x213ec646d47c0151458ae50b0895ebdc1558a864 | 0x65d6e3484f04b82446adb591ebafaa0507c4d3ce4f21d285b5b4e429198c5efa |
| Tornado Cash Depo 9  | 2024-09-21 9:33  | 100  | 1500    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x548664e44b97e5900e98d1f40e90771f7146319f74b964d9950f5f24ce9c4c84 |
| Tornado Cash Depo 9  | 2024-09-21 9:36  | 100  | 1600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x6d443c198af65e08464e2febd3922003e290f03e7a86cbae0e14d937b3b34bf0 |
| Tornado Cash WD 8    | 2024-09-21 9:40  | -100 | 1500    | 0xe7bebe50df652c90473972494dad4c96d0a1677d | 0x80896706951ce5db4f60aec7a68183baa20ca3187f4aeb92f9191a31cb28970c |
| Tornado Cash Depo 9  | 2024-09-21 9:40  | 100  | 1600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x23e56daf368b82e9e146b4b979724e379f85b9ff923cebb4707c4270ff922d5b |
| Tornado Cash Depo 9  | 2024-09-21 9:44  | 100  | 1700    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xb44403ea66019e4c5a110de431ee6b4e1aedd32e517adbbd6b965c26003d830a |
| Tornado Cash Depo 9  | 2024-09-21 9:47  | 100  | 1800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xa09953c47e5eb3ee142c9aa88cb31db6d8046575d1b76701ce2799b726d0fefa |
| Tornado Cash WD 8    | 2024-09-21 9:49  | -100 | 1700    | 0xae7524e04516e3b0900060db1cccecf76d85fdb4 | 0x61a76de16d0c626b5a387b819c8f6979f3cd847978fc84acb2e6ca2db029cd1f |
| Tornado Cash Depo 9  | 2024-09-21 9:49  | 100  | 1800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x6ad7094e82bedb237bcecd17e6525a299bae63a28e004865a4cc5cf716c11675 |
| Tornado Cash Depo 9  | 2024-09-21 9:53  | 100  | 1900    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x019c4debc55f7b8ca307c4867aa219506371ea607317e5c35bf1f772b83e1969 |
| Tornado Cash Depo 9  | 2024-09-21 9:56  | 100  | 2000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x6ffe50407fd402feb1bf488d2db16536ce3319efc7183ea13fa554cab09d7a51 |
| Tornado Cash WD 8    | 2024-09-21 9:59  | -100 | 1900    | 0x5e9e1992293db05cd808d6bcb28f5113bec23cc9 | 0xe97c2b27a6770f14d28e950c9037cea11b9d0dca85732fff9fdcfdad8edd19a6 |
| Tornado Cash Depo 9  | 2024-09-21 9:59  | 100  | 2000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x4d30dd39197f052dbc39fe279a439fe36014fd87f286aefdb106829b84eab27b |
| Tornado Cash Depo 9  | 2024-09-21 10:03 | 100  | 2100    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xc0e1995c7a585346740eda0828674d59f9b29c3699dc829aa6b252b656bb9dd7 |
| Tornado Cash Depo 9  | 2024-09-21 10:05 | 100  | 2200    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xc34b033fa18a4dbc301af7dd03968d6e5dbbd44755c624a987e205f0bbd95b11 |
| Tornado Cash Depo 9  | 2024-09-21 10:09 | 100  | 2300    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x4640ac8dcb38fa008ff3f15a6972bd71fd54b8f4580275cfa462b9d8a5ba3583 |
| Tornado Cash Depo 9  | 2024-09-21 10:13 | 100  | 2400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xb1f4da3d06397f5113aa0d1539049894ae35d0f72407274b891166f0b7b49e3d |
| Tornado Cash WD 8    | 2024-09-21 10:16 | -100 | 2300    | 0x7135492489ea081b6cbd1b273c8a1d949d337817 | 0xbc62651d4965037ab3e84cce692731a817ab1b02fcb39ab52b88f80181c20188 |
| Tornado Cash Depo 9  | 2024-09-21 10:17 | 100  | 2400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xc8c550916879be0cc6ad7a227c1da9600a2940633d0856e62d702b1e69dd5896 |
| Tornado Cash Depo 9  | 2024-09-21 10:20 | 100  | 2500    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xaa88c781058dc1444fdc150d35286dcf0db7d2bebc9781edf02f43edcd64cd6c |
| Tornado Cash Depo 9  | 2024-09-21 10:23 | 100  | 2600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x0bc86732ce161388ea2c0c90c751e2b47b5f6606f6342e50bdafe1d1b02c4bd5 |
| Tornado Cash Depo 9  | 2024-09-21 10:25 | 100  | 2700    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xf23b2d7970fcb736809bfaeef02201bbe9383184dee7d1ced1eff6f99ce4d91d |
| Tornado Cash WD 8    | 2024-09-21 10:26 | -100 | 2600    | 0x77b3ccc6890f6b0709ee6c5e19c929c24482bde9 | 0x8f362a8e90d7ca5e8bae94cb2eeae4914e53261e3ad696b87e3687379a00d1df |
| Tornado Cash Depo 9  | 2024-09-21 10:29 | 100  | 2700    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xc30949889284e009104d55c215748fcd3e113785629080d710dc2199e5f7d3a5 |
| Tornado Cash Depo 9  | 2024-09-21 10:32 | 100  | 2800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x5c7a965dbd3c359e376aeb85c8b0055bc62dd50b2907d809ce4e300e26c28a57 |
| Tornado Cash WD 8    | 2024-09-21 10:35 | -100 | 2700    | 0xae550ad745f4058b33a95421e69fcb6d24d8c611 | 0xf5af34302e6d5ec02a0972126c07b17e55c380ba0d4cd9943aa53a767377c710 |
| Tornado Cash Depo 9  | 2024-09-21 10:35 | 100  | 2800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x833f2fe163b57e25425cf08e6634b939c20fa7b2be1880f465a5db84bbb99460 |
| Tornado Cash Depo 9  | 2024-09-21 10:39 | 100  | 2900    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x56030fd23a4e1d34307cc4cc9f589700778d5784fcfee9aed34825edab42bff2 |
| Tornado Cash WD 8    | 2024-09-21 10:48 | -100 | 2800    | 0x49cdf54a304029407b33a74f9206b4abc55f77d3 | 0xc7030752f502616fbe59ea2c3f0d88d085be972a3c32f1266329e0793e7fd799 |
| Tornado Cash Depo 9  | 2024-09-21 10:58 | 100  | 2900    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x60506895ef35cf163e305b3b8d8865d9a3aed3c2d59407c2c5acdec311cc7d7b |
| Tornado Cash WD 8    | 2024-09-21 10:59 | -100 | 2800    | 0xf4622847e1248a6c8d756a6d90cea6dbaf69e16c | 0xba6a14ba9df635e3f383a98398b69d7be16c5878114f9575292f54a024813ec0 |
| Tornado Cash WD 8    | 2024-09-21 11:12 | -100 | 2700    | 0x3874e1502c70c854b376f1b717a047c9b45dba33 | 0x1deb37118d4b9d79fa557bd7b798701d0602ebc101cb152ff5ba7bb158e9aef5 |
| Tornado Cash WD 8    | 2024-09-21 11:19 | -100 | 2600    | 0xa4f643040c4f757d83be3f27dc0ddf14c9898db2 | 0x60454b802f514a2cc943843b71e673bfc9e667c95af6e7313c3d687a51b83b5c |
| Tornado Cash WD 8    | 2024-09-21 11:30 | -100 | 2500    | 0x188a7c5438173eb590671030c234654cdbcc977e | 0x146fde28737af12dfe4e25415056baa5df25784fe906b640c34bcbbb8ef7442c |
| Tornado Cash WD 9    | 2024-09-21 11:40 | -100 | 2400    | 0x2448593024a07db74d35268f0089e8e61308a2d8 | 0x89adc52d23d7b3e8e3eaa28313fa387b5a433f444c401d13624a61b5ef26cffa |
| Tornado Cash WD 9    | 2024-09-21 11:56 | -100 | 2300    | 0x05add1149adec8fc69c4cbc759b7e18b467f99b4 | 0x4a9d0b85e9a886165e78ea04669a31ffe18a03da8e38dafa2c4271eb4f5e5f82 |
| Tornado Cash WD 9    | 2024-09-21 12:20 | -100 | 2200    | 0xb05835dd07d6102d4ef9df394565913b430a0036 | 0x5d0ec089c6f31d007407847b2943add39a28c9c0c6446da7587f0e88b05ea4d0 |
| Tornado Cash WD 9    | 2024-09-21 12:28 | -100 | 2100    | 0xa56647bb211ba3700c1ad3c904deff606f538bb7 | 0xb23c04472f00b62a758295f3476f12781fb55a40cb139e930c630ad721dd6f24 |
| Tornado Cash WD 9    | 2024-09-21 12:42 | -100 | 2000    | 0xc3ef0f9b14da0d482c19d5c1812f6584312e5d37 | 0x1d1303eb546145a0e3599554a2ffeffc7113f253df282c8650716dfdb0ed4f39 |
| Tornado Cash WD 9    | 2024-09-21 12:53 | -100 | 1900    | 0x2dbb4b05c3185b37822f498778c4abf56408352a | 0x521d7110e259f62a7f4acae494e52bf449d24e94a7f6674d2ed8b6600d62ddbd |
| Tornado Cash Depo 9  | 2024-09-21 13:00 | 100  | 2000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x6e0f2ca42f18ec16e177275467cd25fa9dd46f95660e2ff3c2d07817b4387e89 |
| Tornado Cash Depo 9  | 2024-09-21 13:03 | 100  | 2100    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x630bd40aa7de38e04f95ec9a5ae2d0d70d7229bdcc7a9fa1d2e645c9d251e1bf |
| Tornado Cash Depo 9  | 2024-09-21 13:06 | 100  | 2200    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x63c8cf8e7d7a904d0ad0a5befc26f669b0798f2d28be6d24e1bfc355f23e1933 |
| Tornado Cash Depo 9  | 2024-09-21 13:09 | 100  | 2300    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xbed87d815333a6d0e43f5344753f208f74cde86bab04f3455dc1530750cb8af8 |
| Tornado Cash Depo 9  | 2024-09-21 13:11 | 100  | 2400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xeeb48ca608e9fa1479bb8447fd935a7eaa048a53df8389abda7952f762119e9f |
| Tornado Cash Depo 9  | 2024-09-21 17:55 | 100  | 2500    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x05fe67a5edcae54b1d3e934a65c5800c8f9cb8eb045b47c1a54fc8b8e9508492 |
| Tornado Cash Depo 9  | 2024-09-21 17:59 | 100  | 2600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x9a8f87a7aac0b6d88caabcb3e26fbddfb05bea18f5b3f795e273e0125b482535 |
| Tornado Cash Depo 9  | 2024-09-21 18:02 | 100  | 2700    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x8ceb5111ace8ab176ce0d0a16469520c8088428c13ffe00ddf2c3b101e4ddf64 |
| Tornado Cash Depo 9  | 2024-09-21 18:04 | 100  | 2800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xd6bb34b32364b8e3e3d7dcd13b36afd5706c88b5d765cb53bf9d17e2d6700627 |
| Tornado Cash Depo 9  | 2024-09-21 18:09 | 100  | 2900    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x47f199aaa78f5ce1e0950ad8a99e23e09e9723587c846f8bd2ba3c55314aa937 |
| Tornado Cash Depo 9  | 2024-09-21 18:12 | 100  | 3000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x08430e3137b53c59655902954c44bf578743e0ee70a7d6a52a219a16e4471f04 |
| Tornado Cash Depo 9  | 2024-09-21 18:15 | 100  | 3100    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x7a0f7f6d5660762ddc64e10408f5d2398c290e0e38f2cb338e34371eb2d90e1c |
| Tornado Cash Depo 9  | 2024-09-21 18:18 | 100  | 3200    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x571e1c771a2a0803d25808b7ac2e18cb9e3a34f9cabcf163135f3274a6254773 |
| Tornado Cash WD 9    | 2024-09-21 18:20 | -100 | 3100    | 0x8ac194df73369e6162e51333407f0772d85a5b38 | 0x5a8592ad9789aa4f08b6de968d513db65cba44df40b0b05c6d5562c459a66b2a |
| Tornado Cash Depo 9  | 2024-09-21 18:22 | 100  | 3200    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xeb1ecd25e7bb873ba2637725008043e348e3c7953fac0efd0887a7109c258854 |
| Tornado Cash Depo 9  | 2024-09-21 18:26 | 100  | 3300    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xd5d5e4e507e25618d1fa5dec240548813f058f888a0b539a4a640b5c2302e1be |
| Tornado Cash Depo 9  | 2024-09-21 18:28 | 100  | 3400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x141244a058510b065eefa6478f0f2651a2e70df1cab79dfa45c374dcd4541632 |
| Tornado Cash WD 9    | 2024-09-21 18:31 | -100 | 3300    | 0x920857caee0a46a32788a95510786a35904998b9 | 0x319aea6eba2246dad5041bb2d4830eb7b26279ce8bb8e7bb89dde89fc8db58d5 |
| Tornado Cash Depo 9  | 2024-09-21 18:33 | 100  | 3400    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x4699bacc81fc3e8c4cf499e78d57a2b1c1a42ce29ec31d4c0ab8624cdbfb841d |
| Tornado Cash Depo 9  | 2024-09-21 18:37 | 100  | 3500    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xaa95b1095d6edd97db554728010728a6487e9b1c3fecf2e561c8c6ef609f9cf9 |
| Tornado Cash Depo 9  | 2024-09-21 18:41 | 100  | 3600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x3a32daa125a2bd3c051560b226037b1723573862aac1b77099e723850e6da9c3 |
| Tornado Cash WD 9    | 2024-09-21 18:43 | -100 | 3500    | 0xff0e869e2898162cd4b62a925ecec519ceb33a25 | 0x62aad2045fc0f841b4811d69b1be722c98ce55091c9fbac1d76fbcd8c1ade654 |
| Tornado Cash Depo 9  | 2024-09-21 18:45 | 100  | 3600    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xe5529e35b35a842e7752dac8ff1eff018d8e95c637fcb91afca8450e04b0d076 |
| Tornado Cash Depo 9  | 2024-09-21 18:48 | 100  | 3700    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x3f69db3f3f35c138ddb3839fcda5ef372a95bb05b4c5d61bddcba136fda9ca90 |
| Tornado Cash Depo 9  | 2024-09-21 18:52 | 100  | 3800    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x0f1205d90e588cf5b110fb0fc6a3979ecf051d1d6634907e61cff604eecea60e |
| Tornado Cash Depo 9  | 2024-09-21 18:56 | 100  | 3900    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xbd734ad5fdd717c85879b22c841c4f778c7bb8656b0ce01ae849533526de4371 |
| Tornado Cash Depo 9  | 2024-09-21 19:00 | 100  | 4000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0x05f1339b8083e226eb9f0908ce7acfde3a790737f6a8c4d8063a5cef56be50be |
| Tornado Cash WD 9    | 2024-09-21 19:00 | -100 | 3900    | 0xed2148c2df469b82272486bea90ccbd9011999de | 0x14bbf48b7f6e7fcdd760b008ec2daa1d0b499fdfe5cdff130b547c99629f5e40 |
| Tornado Cash Depo 9  | 2024-09-21 19:04 | 100  | 4000    | 0xfb4f28197258a085969e8c4000090a65c9000eba | 0xcec23fb824cddd1bdc055e544dd7f422243c1859a7afc3b591b8a180f461a9de |
| Tornado Cash WD 9    | 2024-09-21 19:09 | -100 | 3900    | 0x6639f5a45219213aa07d1a0c53de146c89a4a665 | 0x6ce76f1700eac943c8652146e1d52513897a0c56e63aaa9d22e0353866a34147 |
| Tornado Cash WD 9    | 2024-09-21 19:20 | -100 | 3800    | 0x0f308a6ec7cfefaaa2d580b356b10a42073510be | 0xcc21921375dd9fc3a5e47b9870bd632ccb407dc0f045e8cdb180fb3870d3c258 |
| Tornado Cash WD 9    | 2024-09-21 19:36 | -100 | 3700    | 0x3fa4028eb2b652054a33f2aaaa00d69869df5a22 | 0xf74c6af0f4fb8656de947aab3a55c192526af690a3c0e6c9990be876bf62b05a |
| Tornado Cash WD 9    | 2024-09-21 19:48 | -100 | 3600    | 0x89a026676cae9bd60783cab2f47a0f9a5d9abfd6 | 0x33ced12cdd01bbc8c46742d0c3b11528c1b81b8f590673c719f8b4f2ca5d2044 |
| Tornado Cash WD 9    | 2024-09-21 20:04 | -100 | 3500    | 0x3c8f00f786b590b8b7f5fa11e5832580664e7e71 | 0xafd78a6adeeb91378b2a5f13c6ada9350fdd0f6ecde228b6143e4d5b506cebad |
| Tornado Cash WD 9    | 2024-09-21 20:15 | -100 | 3400    | 0xc5f7506ea9f278b1c6b30572840128ab8bc6a71c | 0xbae066dcb243c9f275875b1d5c1149a6b222e258d86fd161562566fc2a14e861 |
| Tornado Cash WD 9    | 2024-09-22 3:22  | -100 | 3300    | 0x4cf9fb0f68c9876f0cf511c7910c2f341adef3d8 | 0x9b54292f93ffc842f227f064171581916cb6500f40b4b72bb69b48264378b376 |
| Tornado Cash WD 9    | 2024-09-22 3:28  | -100 | 3200    | 0x36fde9ef1a086200bb4c7669c51a872e2570c94e | 0xd08c413d5280c030a5670088f34a0b77cbf87169b46a01ac53a49fe0af6b21c2 |
| Tornado Cash WD 9    | 2024-09-22 3:38  | -100 | 3100    | 0x3d24cb1850ec031c441dbf827b2d2277d25ca0b6 | 0x5ee9370edbbfa99d746fbbda5eec416da72fd2950710bf68056d4825967238c4 |
| Tornado Cash WD 9    | 2024-09-22 3:51  | -100 | 3000    | 0x7311c79eae80fff2b55a506e75f8eff5a9657f70 | 0x083744a8f0bee54999bc9403a9890996ff640f2f47b25aef11b8ac44eaa216a0 |
| Tornado Cash WD 9    | 2024-09-22 4:00  | -100 | 2900    | 0x6b5026f6970525de2d1e085b6fdf876f90810eff | 0x04d745a2f09c4d8c730db32a72022d3d1d73978cdc4167bc08fb965a2e98d57f |
| Tornado Cash WD 9    | 2024-09-22 4:10  | -100 | 2800    | 0xb1e676ea71dbcf24ad55ed6033cd0ed4763da6e9 | 0x21b438dfaa6adab604e2c9f149ca5c8aa031c4045d134c2b38043072e1889583 |
| Tornado Cash WD 9    | 2024-09-22 4:20  | -100 | 2700    | 0xbd9956ecd8c100a629c04ab6534eb810f2adf2a6 | 0x73e5068d0055721e6224951173f09456aec089e31b5bcbab7e9c57b3954db71b |
| Tornado Cash WD 9    | 2024-09-22 4:27  | -100 | 2600    | 0xaae94af8d265a94daa12c6c320953a0cff45619b | 0x04df7804da3e933bed66a6f5ac2af2a96426f5babf3e4f122e9056981e962502 |
| Tornado Cash WD 9    | 2024-09-22 4:35  | -100 | 2500    | 0x20910d3fb697c38d239b0c40b9f97b71abaf8168 | 0xd4e8c140866e5da7874c3e080e3809b76b286e17dde3fe2e3943b881bf4ddc1d |
| Tornado Cash WD 9    | 2024-09-22 4:48  | -100 | 2400    | 0x1d724024c1028b63f2a45eab549473d7adfef3e5 | 0x714d645ab8a9d9e6bfd41515345e10cf856c5c92301e01b6d87420f1c3069a48 |
| Tornado Cash WD 9    | 2024-09-22 4:58  | -100 | 2300    | 0xc874d0dfcf49681b59f6354eb03cba0efe80ada0 | 0x09d1c617f541e6b1c69ab35461e6d48d2ae4f18853f31edf13ecd04244788f6f |
| Tornado Cash WD 9    | 2024-09-22 5:11  | -100 | 2200    | 0x29d410d53e175571fe2b44ca982c5fca1bf53bbb | 0x2926291775a37a8535697aad3ec2a6203e5815209e1756bda99988aaae90d32c |
| Tornado Cash WD 9    | 2024-09-22 5:23  | -100 | 2100    | 0x28ae8eac20a64812a37c2aae676ac4f2b515ebf0 | 0xce6265df9b5b4a81c2fe47436fe3552cb94b4c5fb717940fb7d2f60e3d1bfca1 |
| Tornado Cash WD 9    | 2024-09-22 5:34  | -100 | 2000    | 0xa9fa667753ed39cf79fa1faba3cc80d282fc1a14 | 0xc211bd05dd5ddd74ed5fa89af8a68607fc0e91cc05cdac46eb8b2a8f2f3f90b5 |
| Tornado Cash WD 9    | 2024-09-22 5:42  | -100 | 1900    | 0xad0649a1a261af5c563eb60177ccc35abd5aa7a7 | 0xc6b5dc831ddac055d082456acd21237727ac73a315127b1c566a6bae2e84e3f9 |
| Tornado Cash WD 9    | 2024-09-22 5:50  | -100 | 1800    | 0xf061e98aa21e09b2a6897fbb038d7944c44f91b9 | 0x61f10aa23706eb29ec13eb2ee9df7389847ab7ee118efa4ad00ace4518d42174 |
| Tornado Cash WD 9    | 2024-09-22 5:59  | -100 | 1700    | 0x8cd57fdd589d5f69f846dabcbd3dd3e83c95a9eb | 0xcff07a9dac64065657aa49d14132b9333be43f5b2c6f2a5b7f9909d580661ced |
| Tornado Cash WD 9    | 2024-09-22 6:09  | -100 | 1600    | 0xb79a9a764c91556c09747c0c921065789e13be30 | 0x9c90eb4b994bc00180003eecf62a3c24819f9884cdf881f4cf9b40c84b766630 |
| Tornado Cash WD 9    | 2024-09-22 6:16  | -100 | 1500    | 0x0a8fe8a70084a4fa9d79864e280782bdee747b6e | 0x5553be299ce6c4d7e89f2b6d8e03ddf4a87f4d76b7710f5e61c5a0c7a8019625 |
| Tornado Cash WD 9    | 2024-09-22 11:56 | -100 | 1400    | 0xd64b98a4fe51eff365327677489ed02a26174e9a | 0xc45a5381cc353385e81c718d01d60d62272ca2222719b4eea5c4e565e015bcd9 |
| Tornado Cash WD 9    | 2024-09-22 12:11 | -100 | 1300    | 0x8e25394b0432c601a8331dee3652baf010087a85 | 0xf7eeb63ca802f95d01700f7c8c3f8fe88aefd09e2be4875bd6f2970841b9dba8 |
| Tornado Cash WD 9    | 2024-09-22 12:29 | -100 | 1200    | 0x808983a6053430264cb021e8c61d1936ac217dca | 0xc37b204254d0423af56ac3f7e95ad155183a4098d156cbdcc9e892cb2f6db2b2 |
| Tornado Cash WD 9    | 2024-09-22 12:42 | -100 | 1100    | 0x433df4642b2b70a71e38c7b0192c5084fb7b9146 | 0x2e366c5dc7c0a2d9a071d62542a1db6d6476e7ada1b264f5925ff3bf4298c9b0 |
| Tornado Cash WD 9    | 2024-09-22 12:50 | -100 | 1000    | 0x6588a50d2cd3e85493fda84bdaeda8392bf4bbdd | 0x3cd0ed2ef9584987e3f58d0714aaa3043aade787b2db9c8e853119495cb6af68 |
| Tornado Cash WD 9    | 2024-09-22 12:59 | -100 | 900     | 0x24ace3669d0e80ff6dd285fdf0607c7826afa080 | 0xa6b02a4471ce7432d20f8bcba4f388e0e5aa0be4a669502d2fc80e44964e164c |
| Tornado Cash WD 9    | 2024-09-22 13:11 | -100 | 800     | 0x41d45bc8ecee219a311bbfada151936a2d7c42ad | 0x3ed16eade9053b8fa79c14a29da85c4033e009da650c4485affff68be23e554b |
| Tornado Cash Depo 10 | 2024-09-23 10:56 | 100  | 900     | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xfa2abaacd28ec66ea36d956e4fc4086d6a490e2a62a58a6211d2346bc7840d97 |
| Tornado Cash Depo 10 | 2024-09-23 10:59 | 100  | 1000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xf5b2bddec79dc89b3626578e4627bdf1a3cf4945d6930ef97b90c5605181f78f |
| Tornado Cash Depo 10 | 2024-09-23 11:02 | 100  | 1100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xea9d244833c0ac120c974832ffae460f03499f6242f0d7cc9d8c3eba48356c31 |
| Tornado Cash Depo 10 | 2024-09-23 11:05 | 100  | 1200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xf359a2fe2bc35d6420d9528ee4a20653686d15cbb4773193fbb477adc6368efc |
| Tornado Cash Depo 10 | 2024-09-23 11:09 | 100  | 1300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x74109c3099818afdf318f3ea058a2aba9573611ef5986bcb00bfd095eeb4b5b5 |
| Tornado Cash Depo 10 | 2024-09-23 11:13 | 100  | 1400    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xd20529d5dc2226819b50988f1a3a1aae6938867a63923928c53f8749da984ef2 |
| Tornado Cash Depo 10 | 2024-09-23 11:16 | 100  | 1500    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x6b2b07d21501b525715b55fbde26efbbc401452a0535cd9f0523b72a36579146 |
| Tornado Cash Depo 10 | 2024-09-23 11:21 | 100  | 1600    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xace67fedf596d236f36dc3adf29ada2056b1d76fac421f1ca8776583aa96d3dd |
| Tornado Cash Depo 10 | 2024-09-23 11:24 | 100  | 1700    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x0f34c5626743bb01a49e423fe7e066c0bcbfc234dbd9ff31093a5b33e01dd58e |
| Tornado Cash Depo 10 | 2024-09-23 11:28 | 100  | 1800    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5d10efad53aaf4f59552ffb13bf28f7169551192c5d6a007e354a6897daceb5d |
| Tornado Cash Depo 10 | 2024-09-23 11:31 | 100  | 1900    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xe84f7fba705d95d77e136ee690141bcb5185a64e51f35cc706566f75c415e65f |
| Tornado Cash Depo 10 | 2024-09-23 11:35 | 100  | 2000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x7797e24344ec0029bc3e999ae4ebd00623e0fb070ae867abf6b96ba1d2f04e4a |
| Tornado Cash Depo 10 | 2024-09-23 11:38 | 100  | 2100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xa1c6cef51c8f09bfc1d704112a93de40f64e50e82f575b15fb90687d5493417c |
| Tornado Cash Depo 10 | 2024-09-23 11:41 | 100  | 2200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x481207f7ef0b18b2275866b96509ed0a3d18886d8529efd764f9a133ae957a12 |
| Tornado Cash Depo 10 | 2024-09-23 11:43 | 100  | 2300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xf4711f75ff369fd5185a353aedb5af6afa8452cdb29d38cd40730e5b1a76d720 |
| Tornado Cash Depo 10 | 2024-09-23 11:46 | 100  | 2400    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xa8dba07650e890014384a4fb36674f6d8b23b0bc645db582c41899998faf985d |
| Tornado Cash Depo 10 | 2024-09-23 11:50 | 100  | 2500    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5865de1a781030459ba680c33e67f13c838ae7d8b2bea07868bc1d44b4f2f6a3 |
| Tornado Cash Depo 10 | 2024-09-23 11:53 | 100  | 2600    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xc99b55252d8b94e7ac9e9ef4eac5cca763e2df7127980ed960d2afb264a79cee |
| Tornado Cash Depo 10 | 2024-09-23 11:56 | 100  | 2700    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xa7a995aa770137070b4bb843684144f69534cf63d40f7338622c5fd4207bb36f |
| Tornado Cash Depo 10 | 2024-09-23 11:59 | 100  | 2800    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x2c0ff0615361afed4c6a312010e77bb69fd921a9d3aa362cd537a6b9ca1fce0c |
| Tornado Cash Depo 10 | 2024-09-23 12:03 | 100  | 2900    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x8d55a222f890f9c9afa249973f9251f6f7882bd32b8e56d002d2437d0cf99a0a |
| Tornado Cash Depo 10 | 2024-09-23 12:07 | 100  | 3000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xdc66ba0c506763e2f1feb6c7f34c2d11a927fc0e56120b24ba158b13d8f43933 |
| Tornado Cash Depo 10 | 2024-09-23 12:12 | 100  | 3100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5c5cd4e66c366e4d0a573bd926f860444eebe02eb75ee6f4b8b9e5933989b6b1 |
| Tornado Cash Depo 10 | 2024-09-23 12:15 | 100  | 3200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x2f5429a136968b2d3f742b8979ff0ffc892cea1750a03815b215548cd869ceea |
| Tornado Cash Depo 10 | 2024-09-23 12:19 | 100  | 3300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x4fc8a7374d01c8430a8e161b38bc0e43e92caa7b700d6d15271013514b1336ac |
| Tornado Cash Depo 10 | 2024-09-23 12:22 | 100  | 3400    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x4abd8d78cd286a624531c6287cd4b24c785f811f5b9dece9bec963bb97163ae8 |
| Tornado Cash Depo 10 | 2024-09-23 12:24 | 100  | 3500    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5742ee6f3d2e8d21165a09c9d5fb2ba31b01bfedf064660780066ca34abb3e79 |
| Tornado Cash Depo 10 | 2024-09-23 12:27 | 100  | 3600    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x927897caa805c2c4b744f53884ade57a24ed7d2c82872ae3c8b3c613e006c80e |
| Tornado Cash Depo 10 | 2024-09-23 12:31 | 100  | 3700    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x920ab34957943ad688ab8c090f05ed3b35cfeb06737550c3c26d28163ade0540 |
| Tornado Cash Depo 10 | 2024-09-23 12:35 | 100  | 3800    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x436988775cd633c3d3cbe2edc378ece1f4f272f22ee7e993a23223dc281367c6 |
| Tornado Cash Depo 10 | 2024-09-23 12:39 | 100  | 3900    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x642bb2b5a1a7bc2b7150caac5ff513c8b6224098bb3814b60eaa76c11fe46e2e |
| Tornado Cash Depo 10 | 2024-09-23 12:41 | 100  | 4000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5a18d80822c08b286c6b5f6271cd81c122a5e2ce59ca2fc666f5a0731478be2c |
| Tornado Cash Depo 10 | 2024-09-23 12:45 | 100  | 4100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xa12cc88be016e25d22a853c5ad431a1e0b323da3cbad2e3e20b4adb9a5dd1609 |
| Tornado Cash Depo 10 | 2024-09-23 12:49 | 100  | 4200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x375530028dff44556b5161f9a9443918c4d8913018b88410e59b640d23c21375 |
| Tornado Cash Depo 10 | 2024-09-23 12:52 | 100  | 4300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x2dd87686021fb6b1f42fe2a81d82c73187731e386520959ba49957a00f663526 |
| Tornado Cash Depo 10 | 2024-09-23 12:55 | 100  | 4400    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x83c4a708dcd13690fa642ada7f7ef5467037f1b4b74cc3d6ec2198e8602e086c |
| Tornado Cash Depo 10 | 2024-09-23 12:58 | 100  | 4500    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x8306200adb2a6665b83141185bc10d3d04a91bbf74d943e7ed588200f045382c |
| Tornado Cash Depo 10 | 2024-09-23 13:01 | 100  | 4600    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x30c73125eaf7b445acbd73be406bbff5376c8239abae50b725858ade7f83a4c4 |
| Tornado Cash Depo 10 | 2024-09-23 13:04 | 100  | 4700    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x836ac3b867f912273bfa16a146b908aec5127b190a535638f9df58e3e73bd063 |
| Tornado Cash Depo 10 | 2024-09-23 13:07 | 100  | 4800    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xccc7e5866f6185637ae0e744ca9fc77cfc4150f8b563209627c7941bfac4d044 |
| Tornado Cash Depo 10 | 2024-09-23 13:10 | 100  | 4900    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x755a4f78ccdf92c6b8c00e09f8481f56ab2ec658d40e703db79fa1320b1c8463 |
| Tornado Cash Depo 10 | 2024-09-23 13:14 | 100  | 5000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xd95cc3166b7f8c612655c8bccdc0e9c1075762036a75250248b243ff4ed0fb76 |
| Tornado Cash Depo 10 | 2024-09-23 13:16 | 100  | 5100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xbd72a30273cec15ddb3e417b88c5b406e1663278d8ce11e9ee1d4d275b8dc5ca |
| Tornado Cash WD 9    | 2024-09-23 13:19 | -100 | 5000    | 0xf23ba00ab73911d0eb23af6573fdb5242ea2ed41 | 0x2b1226dd1b1ac9a547c8e28d24eef43dc233610be36412590715fb3380bdc4d7 |
| Tornado Cash Depo 10 | 2024-09-23 13:21 | 100  | 5100    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x7f24168efc7cc3952cef1a2c4ecd334df150a6ddd997db8f8765fd900f4818f3 |
| Tornado Cash Depo 10 | 2024-09-23 13:25 | 100  | 5200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x26084a786d780e4961d632b99f1c26981fea33da6fb9229a9232402957933ce9 |
| Tornado Cash WD 9    | 2024-09-23 13:27 | -100 | 5100    | 0x87ca81866e5e1fbe05539d8ae90c0c97ad41bd7d | 0x53cccb077b4eb0d796426b854a9d0704cd33271d3aa8188fd535953d4f5e216d |
| Tornado Cash Depo 10 | 2024-09-23 13:27 | 100  | 5200    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x9816f2c74c59b5bb55165c56265abcf258113234e65b253d75f0c87975447b81 |
| Tornado Cash Depo 10 | 2024-09-23 13:31 | 100  | 5300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x12c359ac2bee0fa6a0cf70718f71cb7bf742df9b3a44ef079d8a1d26dbe9257d |
| Tornado Cash WD 9    | 2024-09-23 13:37 | -100 | 5200    | 0x1dbf60490fd92c5c8e0927699ab2f1dcbf239a35 | 0xf16eb47710bab50af0711710662c66eb2f35a6599591f83d3ecca9dfa91dcaf9 |
| Tornado Cash Depo 10 | 2024-09-23 13:37 | 100  | 5300    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x8e2151673dbd6978d96ddce019f677ed912c2d59956319639072af4ded363372 |
| Tornado Cash Depo 10 | 2024-09-23 13:40 | 100  | 5400    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0xc0297617fe0d89e7086fba5b4c35bcf834b148cfa03e7ae659b92a70b1d327cd |
| Tornado Cash WD 9    | 2024-09-23 13:46 | -100 | 5300    | 0x189df6bf06c7aef516d8adba4d768b065ceae975 | 0xb69f5ee63ccc86ce2a4e45ba2a5614889b5ca849c0e95ab56cb98544a0144bcb |
| Tornado Cash WD 9    | 2024-09-23 14:02 | -100 | 5200    | 0x262f3cbd538d8049ffa883288fc8c2fc389ab9c0 | 0x8373b63e93189254bf0ddc79272259728d63b8ab02ee74327451e4261882843f |
| Tornado Cash WD 9    | 2024-09-23 14:15 | -100 | 5100    | 0xf2418f690295f037c02bf8494e7f7d727f281351 | 0xab53dee31ba6eb084d81c77aff42ca9c54008871d2c691a28d8878176f35b3d4 |
| Tornado Cash WD 9    | 2024-09-23 14:28 | -100 | 5000    | 0x2f0590feece9c54a93e426fa44ac44a4315252c7 | 0x4bf3c6baa45a63f5485215f4137735ecacd74dfea730745fa2d044914cbc0bea |
| Tornado Cash WD 9    | 2024-09-23 14:39 | -100 | 4900    | 0x60adf001e3822b716ff7730b7f0bb0b9c603ec0b | 0xd5b32633733eea5ec488f7c2a7daca4fec0885bd799d60ff94671c02266f01e9 |
| Tornado Cash Depo 10 | 2024-09-23 14:45 | 100  | 5000    | 0xdbde5d6ba3e2dc7812c73dae9ae23c585f638c56 | 0x5bf5a0b434921d25351f6a3d1264777302a7656b0b91f6ae44efbf9e2c870070 |
| Tornado Cash WD 10   | 2024-09-23 14:54 | -100 | 4900    | 0xe0961d49d95921885e4b0346fa805281f81c21e9 | 0x94a48ce668e4b99ebf9aa3bcf0183511da7e77512bbdde401645494ef3acf81e |
| Tornado Cash WD 10   | 2024-09-23 15:13 | -100 | 4800    | 0x510e4e37b3157ea21ba66716df9a8e58e5322506 | 0x15decbbdfaeb7ffc33a53be5a49435f460fd2276a0bf212a8a0421f3c5b31acf |
| Tornado Cash WD 10   | 2024-09-23 15:23 | -100 | 4700    | 0x2efad3a39b6a0ca3fe381ab4b96cf5201d26446d | 0x8e34b67fe19956a7d56987e10551688291691654a8b18965e765e784ad166535 |
| Tornado Cash WD 10   | 2024-09-23 15:37 | -100 | 4600    | 0x36a021d8070e8e9c3e7871e9b41c9401ff09e0fb | 0xacd5b12d8c894cfddf922d410e2e922a987546bf0eb8133d9267724a1c89ed4a |
| Tornado Cash WD 10   | 2024-09-23 15:51 | -100 | 4500    | 0xd378fc5de3c23032b0c353145e888ab80cf2316e | 0xb0079e78f155530e84a12429f74fb760d43e423f3db8ee1a6ccb2e25093c32d4 |
| Tornado Cash WD 10   | 2024-09-23 16:22 | -100 | 4400    | 0x9db64d79710bfb249e60c805cdc9db694caaa1ff | 0x85d00ecf75f88f39e82a38c3640caf0fac2cad08c9cefe0a5a1bb8fbb8a5ef38 |
| Tornado Cash WD 10   | 2024-09-24 0:03  | -100 | 4300    | 0x12459e10b62213e6b64a56711aeca886d76205ac | 0x9e83094de4051eb05abf2ddaad77638fa7c274e09069474992c2fa04130f3905 |
| Tornado Cash WD 10   | 2024-09-24 0:18  | -100 | 4200    | 0x74335834bfa93d349448456c61526f7a1dc3659c | 0x3234921ac85a357b32935b413af7d987f38d5a9b431ea261e3254f7d86196808 |
| Tornado Cash WD 10   | 2024-09-24 0:27  | -100 | 4100    | 0x22706c466a5affe2567b271af8911589743da3f8 | 0x62088389da9078af7f4501fcf9dde37c3750285d34334208143e28274131ee0c |
| Tornado Cash WD 10   | 2024-09-24 0:44  | -100 | 4000    | 0xa2c8594275d867c1c06438afe8504067426819ee | 0xca669b40f06f7659b9d790a728c83d57423da5d583ab7841aafe22545c7dc287 |
| Tornado Cash WD 10   | 2024-09-24 1:03  | -100 | 3900    | 0x5ded64f62b1e8ddc96ff8ebefeb179cb97738ff9 | 0xd19c76a0a8996d251867b22ce5a3cf7d8ff53ea6095d0e2221de14f13b3b3f5b |
| Tornado Cash WD 10   | 2024-09-24 1:19  | -100 | 3800    | 0x3c39da0453d490f9403ffe1899527af904a07b1e | 0x53edab7a587d49f022dedb09b776dd34bb238b0a85ddf4d342ed85254c71229d |
| Tornado Cash WD 10   | 2024-09-24 1:34  | -100 | 3700    | 0xf0fa6d87b11af18e4271f0351930c650cb2553b1 | 0xc05376607514ffda792e1f4997bc8341e68198807634d3c15cf2ababd3aa7572 |
| Tornado Cash WD 10   | 2024-09-24 1:49  | -100 | 3600    | 0xeb278aab90169dca373b2daaad5d9efaf68e295c | 0x971028c629f4d2b7e8720d7f93b1ddb92348dcf6ffbfa042557b8eac5d9dd72f |
| Tornado Cash WD 10   | 2024-09-24 2:03  | -100 | 3500    | 0x3d9896da34ddc36ce6cccff511c73ab409d18684 | 0x0697302671b97be4616688ab36f22bf33c3acd3ab2193377d3ba64b867d08a90 |
| Tornado Cash WD 10   | 2024-09-24 2:16  | -100 | 3400    | 0x7c490b9fa060794e72eb28a641e6b28f6b0833e7 | 0x2aa9f13fecec8adf36f43d0c3f813861662b1dd30ac19d5a1d983155d772c41b |
| Tornado Cash WD 10   | 2024-09-24 2:23  | -100 | 3300    | 0x5117acf41f16ab23ba2e5d35c1da4169589aaee9 | 0x5defc9f86b6f88b86ffe11e7eebda6cb63fedb54bbf58c9bfdf864f382f607e1 |
| Tornado Cash WD 10   | 2024-09-24 2:39  | -100 | 3200    | 0xd3b589b60d7c15b23b4f97985027100a0777ac40 | 0x1ac46f3ec36ab6f73d10b017c2e93e7fd6938c7d1910fcda67edeb5344f89ec9 |
| Tornado Cash WD 10   | 2024-09-24 2:52  | -100 | 3100    | 0x7a1aca1ebcb35f430172cc6d0e8b1755195e95e5 | 0xf5f92ae6f0a0bd105893163ed71c49f8f66bd256eeb023e82a152624e1c16871 |
| Tornado Cash WD 10   | 2024-09-24 3:08  | -100 | 3000    | 0xede0848696562031276d8bb06c50ba93099ef9eb | 0x748a76ca9ba22816eb4b977887e35890d1151774f1e06dfdb1e69c0e5e9ecf5c |
| Tornado Cash WD 10   | 2024-09-24 3:20  | -100 | 2900    | 0x2312104c95a7766dde5f16c7ca770ce26dd676a5 | 0x0a81b8e177c0a37d390aa43c49feaaa1b5146335d4d2f20776e7fbaff7a06b74 |
| Tornado Cash WD 10   | 2024-09-24 3:32  | -100 | 2800    | 0xe800ff8c971445ef4b5663fa61896c38b9517a43 | 0xe5e93e2d23bd59b63fe94d8b6ae8243b8ccd76b41112c52dbbe25e3318cd9ac8 |
| Tornado Cash WD 10   | 2024-09-24 3:46  | -100 | 2700    | 0xb77e94e2eaf04a5031f7a2973d464c641142a36f | 0x36729105c99704f5b257a772692696a65a8631de3d448a86b2f283e0fe03438d |
| Tornado Cash WD 10   | 2024-09-24 3:59  | -100 | 2600    | 0x582bee47f206dd40c0b2bec7692a8298c984292b | 0x11a2cb1c0613a50c2e331098e8bb0fa4ca57fe62b1709e1c03cfec8b06a0a30b |
| Tornado Cash WD 10   | 2024-09-24 4:06  | -100 | 2500    | 0x0ca475ab67aec2aed2815ac8ec5f9df0156b5ebf | 0x0973b3f79ccd1ff65dcb46107553c07db6520c2343d0f32bb5d1f2ea509d5330 |
| Tornado Cash WD 10   | 2024-09-24 4:16  | -100 | 2400    | 0x0b456989f0bc29ff2ae3dd9af034832e2af6f94d | 0xa7f98cf28e406435e3d47cff425c947834ecb2c84a57043d488f3f0aa818885c |
| Tornado Cash WD 10   | 2024-09-24 6:11  | -100 | 2300    | 0x5526cc24c96ac3886e825b975058bcbaefb3729a | 0x3eb1d0a72f0f3e7fc62933c74778ffbd561d30b4753c20784fd20175afc4b93d |
| Tornado Cash WD 10   | 2024-09-24 6:20  | -100 | 2200    | 0xe4a7d2a1c7db94b59c59a9f913d89152a0cc2c54 | 0xe392c4dfbdbaf7f91dd2bd6fa083c05c882c92fd2372013f051fbd7064e3d8be |
| Tornado Cash WD 10   | 2024-09-24 6:27  | -100 | 2100    | 0xb9c18c6361a7e547fddbf3f6ddddfbdef92b24dc | 0xfdfd0d5f743e8791e86306855710145b946a5c15351d701426d22fbc2a7d6749 |
| Tornado Cash WD 10   | 2024-09-24 6:35  | -100 | 2000    | 0xb4cfed28714ee1f45ebafabaff6c4fbff447bc45 | 0x446cfddcd117b5ddd503bc5ec6c63ff226db54683eb611ad122baaaf49be25d5 |
| Tornado Cash WD 10   | 2024-09-24 6:48  | -100 | 1900    | 0xc67565e798996d2973acee042314d0d436b84ebe | 0xa7c0026e3dcecc738456646c56473264b244a2ff16475a6cca65bab54f5fa3c4 |
| Tornado Cash WD 10   | 2024-09-24 7:00  | -100 | 1800    | 0x460ead15e7312068ddd3440017b0e5b6fcc9d2f0 | 0x1756733ccc1e625a0887ac90bebdd7e9f10fd89ba866bc87ba88434e5c54932b |
| Tornado Cash Depo 11 | 2024-09-24 7:14  | 100  | 1900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xb0b015c9b0c70887c8dc062e1dff78a60052ab749285e9327a5e5759a63469d0 |
| Tornado Cash Depo 11 | 2024-09-24 7:17  | 100  | 2000    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x52eff4a9596b9481c0171485b0c357ccedde122946034386f4463656db8c791e |
| Tornado Cash Depo 11 | 2024-09-24 7:20  | 100  | 2100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x5e6d7c03eaf382ada11102a552227662b5fe1e9dd6e646d3c487803e30948393 |
| Tornado Cash Depo 11 | 2024-09-24 7:23  | 100  | 2200    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xc9ad3cfc00a76bd431e4d687a4e447cfd0ad96cd22917d766db3b3ebfb96745f |
| Tornado Cash Depo 11 | 2024-09-24 7:26  | 100  | 2300    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x8cb8372eed892245dfbf4cb6eb59c984f8cd8a629855c5920218bf089a757e17 |
| Tornado Cash Depo 11 | 2024-09-24 7:29  | 100  | 2400    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x8aa16dc287affdc6abee53f7dad67d52cfd51eebae83fc518e8dfec4ef5a4269 |
| Tornado Cash Depo 11 | 2024-09-24 7:33  | 100  | 2500    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xcc7db645e8bd1b4c28ee9282278fca22224c1ed725d58566f963c46ea06a97cd |
| Tornado Cash Depo 11 | 2024-09-24 7:36  | 100  | 2600    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xb92b34d3226ea46c2c7bf403bd67c37c52d45196ba0cc7eb28ff2f44aedf3e33 |
| Tornado Cash Depo 11 | 2024-09-24 7:38  | 100  | 2700    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xf0adeb30c672867b2bb0949df84b7f18a70d204b774b69644f350556883cf7a6 |
| Tornado Cash WD 10   | 2024-09-24 7:41  | -100 | 2600    | 0x724eee940a4e428681b22e3468c5c1b9eb69f5b3 | 0xbe39d8f4b4ed0d956c6bc0b4e308f194e452a9eda1e884d75bffbf7629f86cf5 |
| Tornado Cash Depo 11 | 2024-09-24 7:42  | 100  | 2700    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x212fb9d9cf6d36ae0a4399ab6bda5bf831514627d4eb574d2fdd6d081b2c02f1 |
| Tornado Cash Depo 11 | 2024-09-24 7:46  | 100  | 2800    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xfb17556505f937b9c68b28541919b813475cd88850f191afe0c31d5b58fa6963 |
| Tornado Cash Depo 11 | 2024-09-24 7:49  | 100  | 2900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x1934261b597fc020f9a516d247ef18bd3679e4ebb14b4e033403af5eeeffd656 |
| Tornado Cash WD 10   | 2024-09-24 7:53  | -100 | 2800    | 0x24c5e04228303ea246aa894745b30a90cf99bb35 | 0x545314778139cadb78a6f155ec1936d23db43abc903bf0414d158a3a65099198 |
| Tornado Cash Depo 11 | 2024-09-24 7:53  | 100  | 2900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xf04067165991a6b26d693ac7ea998ccb2ee4529bac3238b282aee0482bb014c9 |
| Tornado Cash Depo 11 | 2024-09-24 7:56  | 100  | 3000    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x450288ce0198ebf4b2fe9b82e9cf71a312def70d82edb8ed5f0c4c72874b2e34 |
| Tornado Cash WD 10   | 2024-09-24 8:07  | -100 | 2900    | 0x8fbb5cea0372c67b95170ebc600aa64b61238b48 | 0x3c731bbb4ec0d577fb8fea769728284e5f0128f649bf9ca2781d40813f54a904 |
| Tornado Cash WD 10   | 2024-09-24 8:14  | -100 | 2800    | 0xcefa3cf1b578a04625d55e6534cb196392e1e115 | 0x0019283316e13eae721be5c63fc34d93f28000eb3c90c3a6b4429e798e8db16b |
| Tornado Cash WD 10   | 2024-09-24 8:20  | -100 | 2700    | 0x7a315d08db044d168e5e497693508c25e7703dd5 | 0x090beca77560aab746a438dbd70ef5da5a2c754aea3a0e45bc166289377f0b8e |
| Tornado Cash Depo 11 | 2024-09-24 8:24  | 100  | 2800    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xdc1c1763d6fc224a1adc4119ee908ecd782d0a6164116b20468980bfab0bf71d |
| Tornado Cash Depo 11 | 2024-09-24 8:26  | 100  | 2900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x80c797f07b7cc9c94c1226ffa8fee10ede23c8c61f8e8e5c9af4c730fd5738c2 |
| Tornado Cash Depo 11 | 2024-09-24 8:29  | 100  | 3000    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x119922e1111a8ab37e3499777b773492a58e8e5b5bd617b530d591be918c480f |
| Tornado Cash Depo 11 | 2024-09-24 8:32  | 100  | 3100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xc6a041b45b0e1aecad636fc47cbbb8ec26131d4e96bbd38697420c263bcfc32c |
| Tornado Cash WD 10   | 2024-09-24 8:33  | -100 | 3000    | 0x9cdad13015d904be748eee5124f4efbfd8f80434 | 0x32d40baafab5fc6e7a761209b20100662fbba28c2e444542838ccb2c824b5445 |
| Tornado Cash Depo 11 | 2024-09-24 8:35  | 100  | 3100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xa841c9d6a2bd96b01f2411bfc951f60c9d8fb9332a57f27c4c2dff60daa6d9cf |
| Tornado Cash Depo 11 | 2024-09-24 8:38  | 100  | 3200    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xf5ad2b4d4e34b2e289eed4a3213a4687e5c6d81f91138ace9258b27620fa19ff |
| Tornado Cash Depo 11 | 2024-09-24 8:41  | 100  | 3300    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x5e4d7c73bfcac1526cbef557d2c900f5d10e5bd4b7563f7fa6739e2252d79d4a |
| Tornado Cash Depo 11 | 2024-09-24 8:42  | 100  | 3400    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x83e9f5016e52dddc02da8501379bc7da6761ae484911d641c87d419808dcd3e7 |
| Tornado Cash Depo 11 | 2024-09-24 8:45  | 100  | 3500    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x7c8577e7abecb22a05ebfc3800ed61f6563e444c71889c28669fd2afe2215150 |
| Tornado Cash Depo 11 | 2024-09-24 8:48  | 100  | 3600    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x2e5a0f3598356d33851c7261fc8fb128890401dc02d9d4bb09ef5ae20cf3ffb5 |
| Tornado Cash WD 10   | 2024-09-24 8:49  | -100 | 3500    | 0x8787801655d756e964823ed25373a0b83970599d | 0xb8529251533ea5edb04f8de17c2ffdb04aed23e590df382c49eb82f3ca99b7d6 |
| Tornado Cash Depo 11 | 2024-09-24 8:50  | 100  | 3600    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x6bdace102847950f0c39af6684ea3bffb8fca58cf6c360aa4618aee0887efd43 |
| Tornado Cash Depo 11 | 2024-09-24 8:53  | 100  | 3700    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x3e47ddfe9da38d734b9c6ab0413434112569d6c9b01da441edc3a646ef30ab2a |
| Tornado Cash Depo 11 | 2024-09-24 8:59  | 100  | 3800    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x4a62d3f486cbf0b821e9badec979ed16246499af7bebe3afaa27044bd3357b78 |
| Tornado Cash Depo 11 | 2024-09-24 9:01  | 100  | 3900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x3d5996a677467f29593143456603ab3974c16024e482418567ff6ca6e2f1484a |
| Tornado Cash WD 10   | 2024-09-24 9:02  | -100 | 3800    | 0xaa7f4b46b6c1d715dd14c4ac38d4d52a309620e4 | 0xe427593bc048712797b518af62d3e621d99a73795670e9da3e720312ab8f66a6 |
| Tornado Cash Depo 11 | 2024-09-24 9:04  | 100  | 3900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x1eb82a7d801b3e1d3f61c5b58054983434732b3a3a541d26fbf22d2f268c0d50 |
| Tornado Cash Depo 11 | 2024-09-24 9:08  | 100  | 4000    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x45cd57420aeb9282e7e17c07f5b2e533a44a76367a20f02afb823f96af9c0118 |
| Tornado Cash Depo 11 | 2024-09-24 9:12  | 100  | 4100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xe9c5b137248fe50d5a18fd1f1602da6f9f46ab4afbceabb64fef4e4177a947a6 |
| Tornado Cash WD 10   | 2024-09-24 9:13  | -100 | 4000    | 0xf8690551a5b0e698f1535038e4455b6e94068496 | 0x284205f3416c977dc0235586a4d50d1906cc23c32cf5cbce292b8371a8e4552e |
| Tornado Cash Depo 11 | 2024-09-24 9:15  | 100  | 4100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x44467aaf7da361ef6627082c206ba2e8e15de0b022eaa7a83041acd9feca27bb |
| Tornado Cash Depo 11 | 2024-09-24 9:18  | 100  | 4200    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x344ff3a30162668e445e2f020cea15ec2f9fb00c3e04f62213c113c50383346e |
| Tornado Cash Depo 11 | 2024-09-24 9:21  | 100  | 4300    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x6f74138d80f3a64fd4cae6f655b4af6c8325e3962e77d5b7e95b5d716a229859 |
| Tornado Cash Depo 11 | 2024-09-24 9:23  | 100  | 4400    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x4016e708be023cb89643a99f039e04805ceb2481abbcfe0b4eae2ae66d60bafc |
| Tornado Cash Depo 11 | 2024-09-24 9:26  | 100  | 4500    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x065ab6f012c8aa626551d1b243167c9dbbe733e267494555ccd15b5a3ece4f49 |
| Tornado Cash Depo 11 | 2024-09-24 9:28  | 100  | 4600    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xe23eefe132f4549aab38af0b18946804539018d50d9e61fb74a1e7651e972caf |
| Tornado Cash Depo 11 | 2024-09-24 9:31  | 100  | 4700    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xd99875385f4b75d7eaa8ab47b42567126b5fbb7a1e52d0e7c04352045960a9eb |
| Tornado Cash Depo 11 | 2024-09-24 9:34  | 100  | 4800    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x1c12b2e40c535e67610ceaeb5286e7eb23724060bd9a4f8c6da0dd9e011fb3b8 |
| Tornado Cash Depo 11 | 2024-09-24 9:38  | 100  | 4900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xd9bc93e2bfcf939a67dd69a94b8c2368b3e978ff60202395d2cd1c39bf7164a2 |
| Tornado Cash WD 10   | 2024-09-24 9:40  | -100 | 4800    | 0x49500d2a43a9d4b617f31686b1adb474af36c084 | 0xe0eb496d90435d9e77199a9eb64cee1914f57b4e40ddbdc38f5c8000070e1300 |
| Tornado Cash Depo 11 | 2024-09-24 9:41  | 100  | 4900    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x3a628f1a2aaea6e32a3d83136d36a391700710ba6b328c8e553ad0290deb4750 |
| Tornado Cash Depo 11 | 2024-09-24 9:43  | 100  | 5000    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x9a7f9641be8c9cee5a4773bf12539b1ccfbc82dab4c062aa05651d1783c70851 |
| Tornado Cash Depo 11 | 2024-09-24 9:46  | 100  | 5100    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x7c1affe7c70260bc5b1f55f7b6cf9837c65a63d04e94fb05b08b89d1282a05ed |
| Tornado Cash Depo 11 | 2024-09-24 9:49  | 100  | 5200    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0x5a99813f9341638516fafb59fae390b16dfb7bae5133b25ac61ccdf1d4c4a481 |
| Tornado Cash Depo 11 | 2024-09-24 9:53  | 100  | 5300    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xa31182a8c6889e441a8e33e2e46ddc797b0b27f95e16717e31d5eae8541f320b |
| Tornado Cash WD 10   | 2024-09-24 9:54  | -100 | 5200    | 0x287f76bc7d9ba622a4b591fd84996a40f0bfb680 | 0x99bbe24ba85d5e5bfebdbc4426c83e303e33759a50ddfa21f1efab5d9eb4ab8e |
| Tornado Cash Depo 11 | 2024-09-24 9:56  | 100  | 5300    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xb790d1690fc88cc6f4af13f0602d396d1929b727c4f9fab8fdcaff5b897e9824 |
| Tornado Cash Depo 11 | 2024-09-24 9:59  | 100  | 5400    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xe82551bffddef42d16edf494a56d9a3112943083370e21f84d9ebca2dfe61114 |
| Tornado Cash Depo 11 | 2024-09-24 10:03 | 100  | 5500    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xc3afa8149fa101658e6696613eb5bfe51f841277d4615a634b1e83b85043d0d2 |
| Tornado Cash Depo 11 | 2024-09-24 10:06 | 100  | 5600    | 0x06414c80e12d3c4c831acb615f98abf7d6387b4a | 0xfe71b3870875b2a0cdb05ef8748f609eaa862d2f7ee8b4dae2f0cf2acf87359f |
| Tornado Cash WD 10   | 2024-09-24 10:09 | -100 | 5500    | 0x02d8bf47c3672a0295959e8001370d405383bf9d | 0x2a27ed3e0b9f0b08de0110ba9f5a471f7976abb77e4f2b59eb82414db3945472 |
| Tornado Cash WD 10   | 2024-09-24 10:21 | -100 | 5400    | 0x12f26d82e4df3b13e1296ad7ac937cfa127e15e3 | 0x1a4d386fd1ce6aca532ef0339e6048bc65fe521bb9823e4d6cb01a0271b0a58b |
| Tornado Cash WD 10   | 2024-09-24 10:40 | -100 | 5300    | 0x3c552fda4043cfe6b650da2ab87cf1cadcfcaf25 | 0x6d43454c32bb60ee8ceef8e3e61710e6da3920882f97b2130f8b1636d3cdc0c1 |
| Tornado Cash WD 10   | 2024-09-24 10:58 | -100 | 5200    | 0x06dc27afdf50f2e0f0c3eff401fc3f92c75b76c2 | 0xb022ced826da48e5d92438ef0ff78a038c445bc3ccef1bb9d18750924a0a067d |
| Tornado Cash WD 10   | 2024-09-24 11:23 | -100 | 5100    | 0xdee87eb4bcf6ddbb7dc220ecabaad8a174141779 | 0xd7d776591740938259030fb28f88d19172573528af8ac53bf8472aae54cbaff9 |
| Tornado Cash WD 10   | 2024-09-24 11:34 | -100 | 5000    | 0x14205149859f7bc79b63ef6a7d9d686ca2c7f4f4 | 0x2d328271f28a081d07336bb1bc1b44d9d6567fbe57d6b5470b651859d98c1d33 |
| Tornado Cash WD 10   | 2024-09-24 11:47 | -100 | 4900    | 0x48f0de984f129d471c4537733654f0b63a7866b2 | 0xe8299fcdc61380f8d00c7debbeef68dd7354f489bd3f7fb6a6963571848b4d6f |
| Tornado Cash WD 11   | 2024-09-24 12:01 | -100 | 4800    | 0x73a846c95d1be7d4df9e13043daf0d8bd4a4ae38 | 0x615741304b17a110e15d2287a33f835540d57dc18506c0d46759eee29dc82c37 |
| Tornado Cash WD 11   | 2024-09-24 12:16 | -100 | 4700    | 0xe8c40f1cd3d3bc77f795945f8afeca62ddb076ff | 0xdf117532f39761613991dcad5742b830ca3516c4e439b285e2bdbe2dc17c47f6 |
| Tornado Cash WD 11   | 2024-09-24 12:31 | -100 | 4600    | 0x910165b84f5062fbb3276e1aa0af501fd4657991 | 0x80edfc1a5c7902593f6efa4acec1af457dfc3d272e39ac8a7d40cc862b4d0202 |
| Tornado Cash WD 11   | 2024-09-24 12:43 | -100 | 4500    | 0x415b9321cb864b6a018dcc746351827a2b1f4bda | 0x4bd293a492072935a9a2af1787182a23f320f0775f990cfdbcb9421becd99594 |
| Tornado Cash WD 11   | 2024-09-24 12:52 | -100 | 4400    | 0x1e2e521ba1b3b6da43db1e9fd5422b65a58719e8 | 0x1533ba44663fdb848483adb23d58922c34c97aa9b135e002c03e6d868a1c313f |
| Tornado Cash WD 11   | 2024-09-24 13:03 | -100 | 4300    | 0xa5d9fa0af2c5b1d30e40b8f2b15c7724dcf85e36 | 0xefb92d670800cdb9c8b418c66332ac32261ed60d5b6c0ebaea90a25021c7a944 |
| Tornado Cash WD 11   | 2024-09-24 13:22 | -100 | 4200    | 0x59ac86395d1e0d44fd5a3e3d5eb76c3aa60ae01b | 0x94a6ff471e83012588cddd5f4eda12671d7d77a0306c404bec55e6bce3458216 |
| Tornado Cash WD 11   | 2024-09-24 13:37 | -100 | 4100    | 0x694db03e67483126ec02121611d011d1779cb86a | 0xeee4228613c451a6fbcb0a90e2ef36cb09f4ebb34d30d96283225a53cdb9efb9 |
| Tornado Cash WD 11   | 2024-09-24 13:52 | -100 | 4000    | 0xf88cebfd97e9e14e434bb7ec35392b9b0d73de32 | 0xccb0e6d2cff0845709a6872584a824125d726ba7544c194c7eb8c3585831616b |
| Tornado Cash WD 11   | 2024-09-24 14:08 | -100 | 3900    | 0xff53661023fa4ba911936ea279359930dd30d706 | 0x57110c6942c826a36907621bd0e7de69c44e3aec8bdd2a534edb65cc0bf64bd2 |
| Tornado Cash WD 11   | 2024-09-24 14:19 | -100 | 3800    | 0x01edea2c477d054c2cc98addd3d30a06a49996cc | 0xcd7beb90d356e03f7f3cc903e2338c865f98a043d6fea4ca3ceb54dada2cd5c5 |
| Tornado Cash WD 11   | 2024-09-24 14:28 | -100 | 3700    | 0x411f248995067668d51612178d59cc00f41b1279 | 0x70ac0a114be096a0fc2ad9c87e99843c62227323d55a7317ee0df1b84d28e904 |
| Tornado Cash WD 11   | 2024-09-24 14:37 | -100 | 3600    | 0x02e65d7ea7a1289d7506afb07d841da1d24983a8 | 0x08aa3d2851494b7ad64bcf32c2177491477b86636a73e27d784e44b1496c20b6 |
| Tornado Cash WD 11   | 2024-09-24 14:56 | -100 | 3500    | 0x01754991bb720282bd688e44f345da9e3df343c4 | 0xd659421e2de79b72d4329e1c3db7d82b7419275010defc519c0d1b004195d07f |
| Tornado Cash WD 11   | 2024-09-24 15:29 | -100 | 3400    | 0x47bbe128eaa1888b6c07d3e48962b84a71b0fbc6 | 0x3903367b4e2d195a2aec9243958bfbee954755d09ce1a4c3b98e5692497de3dc |
| Tornado Cash WD 11   | 2024-09-24 15:37 | -100 | 3300    | 0x83c71854d4e30a509562e09b3a08a00594426a2b | 0xf6d8c66790303e7975a07f0399e8de78f846d9dc8955c793088448e67765dee0 |
| Tornado Cash WD 11   | 2024-09-24 15:54 | -100 | 3200    | 0xaf19922993f99554a794b459d6330646791ae47b | 0x3e807abcc420d3d41fc10f16e2b5f963c38ebc9a2278d404a6eb3226ed9838d3 |
| Tornado Cash WD 11   | 2024-09-24 16:10 | -100 | 3100    | 0xfadf12f623deb0488b598479f33c1b768300e599 | 0xea639c66297ba83892e8b4b4739b2ca5e74487f4fa8167f36d91ce5feda758ab |
| Tornado Cash WD 11   | 2024-09-24 16:26 | -100 | 3000    | 0x019fdc1e08172e332704599f5ed9f8c412047076 | 0x406f0180410198c0ca8a00c75f64c0d1fc7a6eaa7de58bc80e370c61149c4cc3 |
| Tornado Cash WD 11   | 2024-09-24 16:34 | -100 | 2900    | 0xb332f02e3387f0a7183bc99adc1af6eda2a15074 | 0x300380692c038ce52c35748e584684872271d1bac7836fcb5af085eadde24651 |
| Tornado Cash WD 11   | 2024-09-24 16:45 | -100 | 2800    | 0xfb14ada116ea07daaa134dbbd7dfbde33b1b8efa | 0xde16e7fadce5ba1bd3f525a37860b7ece5912b3f8247780aa5a14c8cc3e5d97a |
| Tornado Cash WD 11   | 2024-09-24 17:04 | -100 | 2700    | 0x246eaa3a7b1bcf1cff5b9110775a75ab6034de82 | 0x7c500adc518e6130a0676e710d8444748808d0f0734fc23a3138eedc145906ca |
| Tornado Cash WD 11   | 2024-09-24 17:17 | -100 | 2600    | 0x2d3390eda5436e95ceafd7dbff054f8a42481ef7 | 0xeb7834b78037277297b7b4009af9bbd1e6cff260aff39fdbaba30d04bb63fc4f |
| Tornado Cash WD 11   | 2024-09-24 17:36 | -100 | 2500    | 0x32810b4551ff7bac9bb54469214fc57246af6e12 | 0xef6ffe657b7c8a9cc4ff802a5e4e54ad1d990b2813e26d2426e685b3f817259d |
| Tornado Cash WD 11   | 2024-09-24 17:46 | -100 | 2400    | 0x66d146526db1825e2016e22b31f7251c78913186 | 0xad53614aac9d54206cf1e79c312aa2c606fae3ecf576cb67556f1f5a2a1aebb9 |
| Tornado Cash WD 11   | 2024-09-24 17:55 | -100 | 2300    | 0xbd7f1a74a5a75c3cbcf62e522e318e81a3ceb0ab | 0x419506e2dc5170b677a14728f3e54a421b16ba9bb1b1e153e10bf1f2e745f869 |
| Tornado Cash WD 11   | 2024-09-24 18:08 | -100 | 2200    | 0x6030e77eaec645cd96c2074e01aa8ae5c68abcdf | 0x62332a95a84f9acac322601d80af1e1d7cb6df2d8c29adfb72f0859e9e5f0604 |
| Tornado Cash WD 11   | 2024-09-24 18:17 | -100 | 2100    | 0x9cca339f5b1655719128c47aa9cfd14b559d66ad | 0x8e956752bef8d5b9caaf17ae2fa77518a75ef62cc2b75b6713ad6d0ee49d3bd9 |
| Tornado Cash WD 11   | 2024-09-24 18:25 | -100 | 2000    | 0x605f47134f963018e72b43a055bb106a81e757a0 | 0xa3bce65839bc3d2223332ec1e55f2073dd130396e98cdda60b82f840fd576227 |
| Tornado Cash WD 11   | 2024-09-24 18:39 | -100 | 1900    | 0x221ae6a659e98d1253e7d693a8927a31f7c86bdd | 0x51db60728640eb1a4a06c285a821ca5403331b7ccd528c7febf6af0dc4a1df18 |
| Tornado Cash WD 11   | 2024-09-24 18:47 | -100 | 1800    | 0x9af89040fbf01d64f2730877101297c8a37eeb14 | 0xd33166d66c1ea173e368da8797ca7f5dbae463ca6f207cfef111020f521adbd4 |
| Tornado Cash WD 11   | 2024-09-24 18:56 | -100 | 1700    | 0x859abdedad55e5f3b5d0dc07e8383980c441adbc | 0x94c4111e48e5f18896aca9fd4b576c21332282fdf3028f356e196a8b5051ab74 |
| Tornado Cash WD 11   | 2024-09-24 19:03 | -100 | 1600    | 0xf123327bd6e44b0ab1f40f9199a9add4f0359a2c | 0x6396fc3df2624ae698bb7658c6f6e36ecad49976e68afe2659c616d8c978e14a |
| Tornado Cash WD 11   | 2024-09-24 19:12 | -100 | 1500    | 0x006fdf9941ee8bdcaa1020ba83737b200dc083d2 | 0x08d9edb2920529f64eb0cfc59227f2522f0c4333a3a3cdddca425823352e4c89 |
| Tornado Cash WD 11   | 2024-09-24 19:21 | -100 | 1400    | 0xd057480a9f6abbaff0d7aa4335dbc65ae98df541 | 0x1ebd310567fe5b3675f48624586cd9ce57a9c0866606065890009b09a9f816e7 |
| Tornado Cash WD 11   | 2024-09-24 19:33 | -100 | 1300    | 0x43f27f6de3d18a69cbee3f4bd1d5d0f1d0e53511 | 0xebf5d4d072b6e438d57476c2154f123b5e67f70f210ea68b2d0f986a5d3424c2 |
| Tornado Cash WD 11   | 2024-09-24 19:43 | -100 | 1200    | 0x5d267475586edfeeb81bef1ad3152c3b53512818 | 0xa705b878e3597e40ce9a81728e17bf9de4da2e935419b3da01eb0a547c6e0c68 |
| Tornado Cash WD 11   | 2024-09-24 19:59 | -100 | 1100    | 0x8c66a9809ff827f03f21bf1ea1224a519c712637 | 0xce38dd37173ad65ae8c63053cd90bd425ef4096a2f23158a13e3786ba2f05df9 |
| Tornado Cash WD 11   | 2024-09-24 20:11 | -100 | 1000    | 0x95843ee8b0b005ce83bd1fa1b9bc340a6b96a9c1 | 0xd61b9eb89fad80b259b29eebb7af3a8ac3f6bbf640d02813b9cfb144d7140e59 |
| Tornado Cash WD 11   | 2024-09-24 20:26 | -100 | 900     | 0x77eddab8635e7f6d8add523793596df5cacf4944 | 0xd13187f822acae6dd0b0dcacdd3ab84e94ff03d1f68ca8bb241a01e762451cb7 |
| Tornado Cash WD 11   | 2024-09-24 20:41 | -100 | 800     | 0x81142408bffc9f53bdc6b32c692db2612b6be477 | 0x7330f75bf64c0a5a95e6415a4c33728c6cb67c945db341a3df98a886e30f1c2f |
| Tornado Cash WD 11   | 2024-09-24 20:51 | -100 | 700     | 0x05ffdea77f63865e960e5ced45178a616eeecfb6 | 0x5bae1b3d88801b90461f5fd9303649ef1d2903d4e632e41e376b8a3b1c07392d |
| Tornado Cash Depo 12 | 2024-09-25 7:12  | 100  | 800     | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x612f30b12dfca7f5dfd899354ef8d1e129d75f2aa1ac3477b5039ce892024f66 |
| Tornado Cash Depo 12 | 2024-09-25 7:16  | 100  | 900     | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xd7cc6706b59a4c1e35fcdd04b41a02ed60ee5fc81138d3db8bdb5b4bdbf8270b |
| Tornado Cash Depo 12 | 2024-09-25 7:20  | 100  | 1000    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x37c8d401099393c3bdbdef1c32b62c0b0c09274cfb9244b87f06fe78a00cce3a |
| Tornado Cash Depo 12 | 2024-09-25 7:24  | 100  | 1100    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xf7503dc57c064db5fb3b050e04b8151cde5f1195bc2baeae812d2a18d39aba01 |
| Tornado Cash Depo 12 | 2024-09-25 7:26  | 100  | 1200    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x79ea08bdd85daf171599d0102f416e7b82c409cfb99c123aa4886c4668840df9 |
| Tornado Cash Depo 12 | 2024-09-25 7:31  | 100  | 1300    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xee51f6868078f1bc82c53b0c65e9b7d5bdf30d92b36f7c7095b499f244821f89 |
| Tornado Cash Depo 12 | 2024-09-25 7:34  | 100  | 1400    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xb83b11bd9f1fcaea8e98980ada01d9100b44f7d48177900ee1231de47bd02698 |
| Tornado Cash Depo 12 | 2024-09-25 7:37  | 100  | 1500    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x3e1000e72329f85b38dd33e2d615bd79e74d12f94be710127bdb6232a6781ddb |
| Tornado Cash Depo 12 | 2024-09-25 7:41  | 100  | 1600    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x2ae03ed7a8cc1adc0e5756cafb957a0284e64a0e4152629bdaa9f404b88dc2e3 |
| Tornado Cash Depo 12 | 2024-09-25 7:45  | 100  | 1700    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xff81b4997e13584a414dc70eb170b4eaea9f86cc01d7b2c658f92bbaf44bebfe |
| Tornado Cash Depo 12 | 2024-09-25 7:47  | 100  | 1800    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xd96708317cf2773e57af4b984628ac52d9c5c132af9fbb023a55acf99377954b |
| Tornado Cash Depo 12 | 2024-09-25 7:50  | 100  | 1900    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x942aba7d1cfd7fc69b23df0b0f6d30012914b2ab8f63162625dc2140943adb41 |
| Tornado Cash Depo 12 | 2024-09-25 7:54  | 100  | 2000    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x01ffae10a3453089499c1ae8b30fa3cbc0f3519552e8fb349bdfee6308a32bf3 |
| Tornado Cash Depo 12 | 2024-09-25 7:57  | 100  | 2100    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x585283800413c7e9a858046d1d46b0f4da0b233780ea9ea26290a9280f98bfa5 |
| Tornado Cash Depo 12 | 2024-09-25 8:01  | 100  | 2200    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x71a582c6660b27338eeb54a73b2bd741c8dff2457ca2496ab5b3109300f44979 |
| Tornado Cash Depo 12 | 2024-09-25 8:03  | 100  | 2300    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x4ee4305feac627c8b0b98e7d2a373eb81cd379f7e63d9c9beeb175104c973d78 |
| Tornado Cash Depo 12 | 2024-09-25 8:06  | 100  | 2400    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x99cad80899996418b56b3ec389fda29972d8d9d4ceea1efd54906ec09a356ddd |
| Tornado Cash Depo 12 | 2024-09-25 8:09  | 100  | 2500    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x64b129d1e4cd5916ef1f87e1c6592d27b0a02134295715641baa88e25ffad7b2 |
| Tornado Cash Depo 12 | 2024-09-25 8:11  | 100  | 2600    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x520a47d5c22b449016a4f2555339bd4799fc6678db3c9ebdc8f9d6b7c9826888 |
| Tornado Cash Depo 12 | 2024-09-25 8:12  | 100  | 2700    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x1a141026bb66762e8f081e51253a0cb3da5c6dbe75d682b229d39f4b99339772 |
| Tornado Cash Depo 12 | 2024-09-25 8:15  | 100  | 2800    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xc220d146356893da9801da784fe852d6a01f986752ec5538ab8a2625933cefb2 |
| Tornado Cash Depo 12 | 2024-09-25 8:16  | 100  | 2900    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xd30f6876f560403914c0391866d8ea50f2b15799b90b1bf4bb2dafc302311818 |
| Tornado Cash Depo 12 | 2024-09-25 8:19  | 100  | 3000    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x91f5d4d45981a0059c9764fbaf789e4949e243cb41c4ce4709e0e8a5fb02024d |
| Tornado Cash Depo 12 | 2024-09-25 8:22  | 100  | 3100    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x610622a25507e40f99368c6a57e18b43bab35acad383cf2d4214f1797d410a4d |
| Tornado Cash Depo 12 | 2024-09-25 8:24  | 100  | 3200    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xf2f5d6f38383c55b0c987478202aa4bcc4c8883b790dc5d71a24ca07afaa2bdb |
| Tornado Cash Depo 12 | 2024-09-25 8:26  | 100  | 3300    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xa7297a96c983ff3e7d2ce74443e4ec947d2bafc33a8b0698390bb9265a00dfb0 |
| Tornado Cash Depo 12 | 2024-09-25 8:29  | 100  | 3400    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xd7f08754064d7b154807cd034f9e1ad51491f610de285dd4f42219820d6ff27e |
| Tornado Cash Depo 12 | 2024-09-25 8:32  | 100  | 3500    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x5a4f1f990f5e0da11ea5902630694b0084573530a04e69b66e187510c8733208 |
| Tornado Cash Depo 12 | 2024-09-25 8:35  | 100  | 3600    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xc66f0ad15f1d44262461a0e43c98187f05a5739362668c2e5f8f862f5dfd9c99 |
| Tornado Cash Depo 12 | 2024-09-25 8:38  | 100  | 3700    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x454f238ad4364a7f17ae5c3b62b65d8ea86c5a839e54f6532b7ce32b0136901f |
| Tornado Cash Depo 12 | 2024-09-25 8:39  | 100  | 3800    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x543882bf7eefce585401268f44d036aa9abda9ee699cba23a44d0a3d21be51e8 |
| Tornado Cash Depo 12 | 2024-09-25 8:41  | 100  | 3900    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xa10b103b0331b1924927b35e79df739e130dc8b74c89ec7e9609d0d0907596fb |
| Tornado Cash Depo 12 | 2024-09-25 8:43  | 100  | 4000    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x4682d2379920c538186c94a7480c34a6d772d7d423d9d2d92936bc1434302123 |
| Tornado Cash Depo 12 | 2024-09-25 8:46  | 100  | 4100    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xfe51b506df2ece62c617e2d2d8384856574b7388688a2878af32c6b18c9b0d3d |
| Tornado Cash Depo 12 | 2024-09-25 8:48  | 100  | 4200    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x4ef59b3267ef2c09084ed82ad58d10fffa321fdddd31ce1fd48f46469dffdddc |
| Tornado Cash Depo 12 | 2024-09-25 8:51  | 100  | 4300    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x08d6cddbf10e677e904523a3f809768194e4d1872468bc46ac0220d56ced50f3 |
| Tornado Cash Depo 12 | 2024-09-25 8:53  | 100  | 4400    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xf9a95980e34c8745c4ef7a667726b69222e8d4219ea009bd36968ff38e10827f |
| Tornado Cash Depo 12 | 2024-09-25 8:54  | 100  | 4500    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x89c2c0c29498e5459ed6388a137a12ab103fe3d1dc24a382a7e7d8de06b986ad |
| Tornado Cash Depo 12 | 2024-09-25 8:56  | 100  | 4600    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xbce0eca412a7412ef1acd81173a304ee094683b638255043cd1e496d51168a08 |
| Tornado Cash Depo 12 | 2024-09-25 8:59  | 100  | 4700    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xaafe0107c1277acc19cd1a8a79fa300010a9fabee52a02463d067449619fe5fe |
| Tornado Cash Depo 12 | 2024-09-25 9:02  | 100  | 4800    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x50f74568228208b95b29121c783ea2f7c35cf35ea20904e50d1b7a7b2a1afe4a |
| Tornado Cash Depo 12 | 2024-09-25 9:06  | 100  | 4900    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x8156208512f18a49af7367d028446eeb1771c1e5debab5c900e5e05f121f8350 |
| Tornado Cash Depo 12 | 2024-09-25 9:08  | 10   | 4910    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x58910106d482a72cf347ac40a3192990abaf692b380491af1ff5a3a7561fe2e9 |
| Tornado Cash Depo 12 | 2024-09-25 9:09  | 10   | 4920    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x53a02f489ce614021ec7669caae89472ae1bab7cc376d86597dae0ebad4ee8fa |
| Tornado Cash Depo 12 | 2024-09-25 9:12  | 10   | 4930    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xeb43dfdcd4f19ba229f29060ffafb914e750bbf5a75611eac9dafb40ca335218 |
| Tornado Cash Depo 12 | 2024-09-25 9:13  | 10   | 4940    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xdaacd81a1f066c0bcd1cfb619e8c57a977bcbc66cba680a30f18fe53f7aed7af |
| Tornado Cash Depo 12 | 2024-09-25 9:15  | 1    | 4941    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xe1c4a32056ceec98e8fe3e301e446553c430ae25e40a4c31676300839295dc04 |
| Tornado Cash Depo 12 | 2024-09-25 9:16  | 1    | 4942    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xfca8a702168197e03bec8cd9da2e6416110c980f2fdc036daa2ffc790ff8b5fa |
| Tornado Cash Depo 12 | 2024-09-25 9:18  | 1    | 4943    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x21a4697b273ca4574064dbf6cb8b4672c10da24f2dc6132bf1e5089e64786817 |
| Tornado Cash Depo 12 | 2024-09-25 9:20  | 1    | 4944    | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x77c5c494ee807b27072bc1e0462efa60e26ba9407954e3b7695c4cc9fea30e1c |
| Tornado Cash Depo 12 | 2024-09-25 9:22  | 0.1  | 4944.1  | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x2ce30328e8d2eea4d6c2c3ceea256f4fbdeb1c62c503e75c1fdc55406e508bc3 |
| Tornado Cash Depo 12 | 2024-09-25 9:24  | 0.1  | 4944.2  | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0x1d3acf4ea577f8ad2d8935428043e288c8d30400cf68d37bc662a1c1125475ea |
| Tornado Cash Depo 12 | 2024-09-25 9:26  | 0.1  | 4944.3  | 0xa6e894326214535916bf0b7d879cccc734b6120e | 0xafbac4b68f8074bb400fcbc5f1aefadf2b795a01704c9a7ebcb2dae9b826df6d |
| Tornado Cash WD 11   | 2024-09-25 13:03 | -100 | 4844.3  | 0x493df6ff837a19215740139c7255a0ad5d006f7f | 0x27a6306a6a3ae4061763d989687df5235b4c361830d43562d7daba0c329a28eb |
| Tornado Cash WD 11   | 2024-09-25 13:15 | -100 | 4744.3  | 0x65c2ac2f177206c77f66865adfb0c8b456bb97d1 | 0x6bd0ab2893ddaa4eecbff364fe0c46395ccea2b002dfafd5871d9af1825b9126 |
| Tornado Cash WD 11   | 2024-09-25 13:24 | -100 | 4644.3  | 0x3ef060fecac4114d50fecd35ae3523bdc1b3a42f | 0xcc247d55f2bc36f2b43dd9253bb1c5ef938dec797c477844de38e58c1c6d3325 |
| Tornado Cash WD 11   | 2024-09-25 13:32 | -100 | 4544.3  | 0xe9a5d423336e40799d0a71bbf13b21350d2096f2 | 0xd1fd4ee037aa71a0c7adca8b80c779786fa43dcff95b673b869655b6608ac2ce |
| Tornado Cash WD 11   | 2024-09-25 13:39 | -100 | 4444.3  | 0xd797b5899247adc43aeb1dcad7cd0537eca98e1e | 0xd8c874a93c827b237df0cadd23858ef8f139c10d574dcede1f45aee995224ed8 |
| Tornado Cash WD 11   | 2024-09-25 13:48 | -100 | 4344.3  | 0x464c008378d6aa59fc3bb91548f2a752ac655c9a | 0x8f3d695d262ac291b7bb7e75ded170b7d564787d77b4aa258aa500525e6fbd69 |
| Tornado Cash WD 11   | 2024-09-25 14:19 | -100 | 4244.3  | 0xf9d9aa61c2d571d7719445f8dabb4c5396ede553 | 0xc5987e12b5d75e6a8da9f8ff69b2d9a469887349073f8bf0824c89fc24eb4700 |
| Tornado Cash WD 12   | 2024-09-25 14:37 | -100 | 4144.3  | 0x8aa57238c1503bab045bc7a81bb34f7454d1802e | 0x87c3fe30bbd619b3985cf74d66a3fbe0c4f20bdf6e9f5ae582c881c7cb8c1f6a |
| Tornado Cash WD 12   | 2024-09-25 14:44 | -100 | 4044.3  | 0xa4244f2f9e486f20d925336867cd95973152ecff | 0xb2d05b794d33bebb0f857a1228b5aca325522e957965826166f1a95f55e1fd65 |
| Tornado Cash WD 12   | 2024-09-25 14:54 | -100 | 3944.3  | 0x93ca1dea6a6969fdb26d7611e674dec9ccdfe5a7 | 0x8ffa5122abad95802344d9cbc8bef8ae299602b1ab115d76e3f81b79fbac14c8 |
| Tornado Cash WD 12   | 2024-09-25 15:12 | -100 | 3844.3  | 0x8ac97d0f70c2b05cc03b617ec7fbb8b7dfd3c942 | 0xb92b8c48d57780c07151550ebc7d07722809d2d77d398b05bd4db699551ac3fd |
| Tornado Cash WD 12   | 2024-09-25 15:25 | -100 | 3744.3  | 0x42ac9dbf33d29506e84697a1092a8a9ec767e31c | 0xf2c506a25c2b0d026dca46ae9d7952a4c2df054f8bb4ca77ec33e6c9ac028d4c |
| Tornado Cash WD 12   | 2024-09-25 15:40 | -100 | 3644.3  | 0xaab5f9042d89ed0d9896ba89b9dc6cda3de3a27b | 0xc282962c2c3b0bf9427ee85dbfa58f47922138874511e84838ee8835f5908382 |
| Tornado Cash WD 12   | 2024-09-25 15:49 | -1   | 3643.3  | 0x2d868a20da8b5e07f79184eccfe1aead35132dac | 0x82915f68a9e76bb047ea3059be8cf318e3dfe2e707ea5f4c3a6a5adb9f761771 |
| Tornado Cash WD 12   | 2024-09-25 16:06 | -100 | 3543.3  | 0x2d868a20da8b5e07f79184eccfe1aead35132dac | 0x5f6b4b23ab8664501f4803b45cb164b81768484b07307ae431c2c705acc150f4 |
| Tornado Cash WD 12   | 2024-09-25 16:25 | -10  | 3533.3  | 0x73300fb6169972f11acda1bc128f8460bfade0cc | 0xabb5cd77b6868f9e3866eae916c59b600e863609b291a956f0cb4954472329f4 |
| Tornado Cash WD 12   | 2024-09-25 16:41 | -1   | 3532.3  | 0x73300fb6169972f11acda1bc128f8460bfade0cc | 0x1b561000a80702d42e34036fbbde95389abad0fba44072c05e168578502638e8 |
| Tornado Cash WD 12   | 2024-09-25 16:57 | -100 | 3432.3  | 0x472bb4e25ad8304345a12139866ed566e2c3e48f | 0x30c6e9abc17087f496ca869d653d0df7a48e9d36031c6b6d62d6b9470273ef8a |
| Tornado Cash WD 12   | 2024-09-25 17:05 | -100 | 3332.3  | 0xc41793bfc82ba230bae10ce9e4a8d13fc3272122 | 0xe0e0ebfbdc2f66a757346ad4c38a6fc4f5c9bc6d205c1bc5949fea6c56ff3553 |
| Tornado Cash WD 12   | 2024-09-25 17:21 | -100 | 3232.3  | 0x85e2f944349190a15af8eadc4f975406d1dc6a4b | 0x6e8eb1f92df5b98888adbce9be2df532e41f3b77c5f2a7429f6e8de78c96ce6e |
| Tornado Cash WD 12   | 2024-09-25 23:51 | -100 | 3132.3  | 0xd7619b8e2538b0aae7e8d3b2a9087ea256801d0d | 0x6d347459c47d5289ebff1390da08788bc1b236d93f40443df22355e74f55134f |
| Tornado Cash WD 12   | 2024-09-26 0:04  | -100 | 3032.3  | 0x10149d5d89d0d78d4b5b1bbfb8817b9e8e4067a0 | 0x5ee5fda933aebe39ca1ce9fac1879ce70292757d129d6b8ac4876f912b4cd03d |
| Tornado Cash WD 12   | 2024-09-26 0:14  | -100 | 2932.3  | 0x71eb2ef4a2916a442072177f91b7ef0bcf1b7f38 | 0x501a0bd6ba810ae4ecf2c0e87d2ab5c93aae3a2f3f2c0bd2f2a8d8c06c6a76c1 |
| Tornado Cash WD 12   | 2024-09-26 0:24  | -0.1 | 2932.2  | 0xda63e2cc9f541ee5af64927ffcb0c512fb18338e | 0xa2ce5491b117d82186fa24d839f3fb152453db1695f9558d0a5720f64cd39a77 |
| Tornado Cash WD 12   | 2024-09-26 0:37  | -10  | 2922.2  | 0xda63e2cc9f541ee5af64927ffcb0c512fb18338e | 0x233746da1d9d4f70279323d5a1c14f96681639cdbc37efe2cc0fbd6d62947390 |
| Tornado Cash WD 12   | 2024-09-26 0:51  | -100 | 2822.2  | 0x3034723fd7151aee449e8166bbf61a7b1a62c3fd | 0x927e37b0cd8684818c1f7039e50e6113a66267fe0f4b4dc2ae7dc062442fb6a6 |
| Tornado Cash WD 12   | 2024-09-26 1:04  | -100 | 2722.2  | 0xbba5456403279295e7dea5e3683ea434997c5c21 | 0xc4a29b68675c397ff93927428d24197b2f1b1b2443d6ebe2591a9a9b6af038c3 |
| Tornado Cash WD 12   | 2024-09-26 1:15  | -100 | 2622.2  | 0x46a5f010497435ccfb5f0e0de5a3fbefa435630e | 0x105d4c8de31fd6b3d6b11efd3095bc64b7beec5b2d9fe6363381bf37ea55e6c3 |
| Tornado Cash WD 12   | 2024-09-26 1:32  | -100 | 2522.2  | 0x18b431580b7a12a9cb898d9fa2fb5e76370a7e72 | 0x7438d61e2c11da802c55a085226b29c515f8a5e454b30b566841a09906d2eabe |
| Tornado Cash WD 12   | 2024-09-26 1:40  | -100 | 2422.2  | 0x8920c2c8c1b4b97840fb3f7e5f2225c4fff28451 | 0xdf21ed3754a7594e073163c0e9b927bdadc2d72aa621144164354c2a376e7f07 |
| Tornado Cash WD 12   | 2024-09-26 2:00  | -10  | 2412.2  | 0xa2a465e9c96fa703e3298996d194dff561a1ec22 | 0xd1e0324e833238bd2dd9f5d7822d6fdbd57ff2f2a6293dd7656b0824bd0cbb0d |
| Tornado Cash WD 12   | 2024-09-26 2:21  | -1   | 2411.2  | 0xa2a465e9c96fa703e3298996d194dff561a1ec22 | 0x1a1dcbfa086699f8ca7d32741bfc883717e689bc459ce67b2a857ae34f3aaeaa |
| Tornado Cash WD 12   | 2024-09-26 7:04  | -100 | 2311.2  | 0xf25004359443c93465f9f1a6601151bfd7af6adf | 0xe0f2f5bf0efcb601167ee87d7f2b8db123812eb9fd513f7f6a67806a0cb22248 |
| Tornado Cash WD 12   | 2024-09-26 7:11  | -100 | 2211.2  | 0x79a815975c8c4c7adc1dd0d13549681cc87b4ca6 | 0xe5dfa583e367d480eb26e92e655dbd92794a7fc3c32c58c384f53ec036f3d316 |
| Tornado Cash WD 12   | 2024-09-26 7:27  | -100 | 2111.2  | 0x8d1fecebb93c735eee9fc06b0cd227c7508bf797 | 0x9de797487a03268c30b87a2e7a5ad4e22c18fb8cba73bc07593b081fa90b239f |
| Tornado Cash WD 12   | 2024-09-26 7:43  | -100 | 2011.2  | 0xecf637b2c5cb141e55c2ed63c51c20767664f4b3 | 0xe1e6aa04ba8223240f39c97fe4029d3850f2ef8e817904f8b57b698ac163b71d |
| Tornado Cash WD 12   | 2024-09-26 7:55  | -0.1 | 2011.1  | 0xde46b18b295a783b010436cc8e2ba8bb3feea875 | 0x22b96056c67369cbe2a62f5c7de8d48b3ed0731f34090681a0ce82bb8481d7be |
| Tornado Cash WD 12   | 2024-09-26 8:04  | -100 | 1911.1  | 0xde46b18b295a783b010436cc8e2ba8bb3feea875 | 0x196b3393730b0453772f023b01e6b2034b09e246b2442a0ee1b4769daff1fb01 |
| Tornado Cash WD 12   | 2024-09-26 8:12  | -100 | 1811.1  | 0x8dc81ed6508b714db2e60e4ea04219b5358937bf | 0xf46059de44d34aadef8afe16ffcec5dec7bb4cde7929ae015e7ff7e3327fcf0e |
| Tornado Cash WD 12   | 2024-09-26 8:22  | -0.1 | 1811    | 0xf4d162231c426c9111951803c5c155e77759c16e | 0xc50c38534b2a6f071d32a518bd7efb880336e2bcddac755f8b7fe34e0e75edca |
| Tornado Cash WD 12   | 2024-09-26 8:31  | -10  | 1801    | 0xf4d162231c426c9111951803c5c155e77759c16e | 0xa917141b9750a7fccd21799c372471e0025fd77ca191338f489b9b92daf59126 |
| Tornado Cash WD 12   | 2024-09-26 8:41  | -100 | 1701    | 0xbd61efb21f9bc6c3b7b267ad5b39dcc4f9c2a823 | 0x705dfb324f4f1f53dc6a43da97ad183c6ac16c4b84a0e29fc7526ee80ece9c85 |
| Tornado Cash WD 12   | 2024-09-26 8:53  | -100 | 1601    | 0x96e5f679e8c324c8e2b710d2524bd5104ea75e06 | 0xe26d36e46e1d123da40fe3435e3d00474218f5f7188939eb1e1901448f0d5365 |
| Tornado Cash WD 12   | 2024-09-26 9:06  | -100 | 1501    | 0x2313b42888eddfffdf84e4bb38c647e466b7e4b6 | 0x9ce9a86bf7dde50a58d363eeb9b526c284c788d02524f9372fc800b7e9a2f917 |
| Tornado Cash WD 12   | 2024-09-26 9:23  | -100 | 1401    | 0x993e97026b39ae1e1f7d297cd1160d6cfbe390d0 | 0x4b59c13c7becc7629db8334abb215236281b93b61f8b3181fab94745cc76dbb3 |
| Tornado Cash WD 12   | 2024-09-26 9:40  | -100 | 1301    | 0xd6dde4491bf614d282d71fc7bdcefa7cee97e3f4 | 0x6f1293158c8abad71ff2387fd35466e231a774b5a573f2ddd8ffa38194fa3bd9 |
| Tornado Cash WD 12   | 2024-09-26 9:48  | -100 | 1201    | 0xc82c9287cb6cb69c1e3092af5709be3377c7ba98 | 0xa06ac2edc609b35b4876fe9e1ab8f5a815b4c61bdc86156a29786144a3c27a4a |
| Tornado Cash WD 12   | 2024-09-26 9:56  | -100 | 1101    | 0xc697e4a47b8368fae14f7a2566e038c41518d14c | 0xd43d43b40b1aa5e33d1ad852b7a376487a5fe42b374734cec3de2ea6694e64a0 |
| Tornado Cash WD 12   | 2024-09-26 10:09 | -1   | 1100    | 0x297ebb0d16928af1f80f9f0a5c0326ab3cfd509e | 0x4481d665852a9802f821985c106e92d9eb12626a4134aed2a281066bfb1a90fa |
| Tornado Cash WD 12   | 2024-09-26 10:26 | -100 | 1000    | 0x297ebb0d16928af1f80f9f0a5c0326ab3cfd509e | 0x29591fa3ddbecd7d824407a37e80979e167ade1a84e9456e2eefc8be198259ac |
| Tornado Cash WD 12   | 2024-09-26 10:42 | -100 | 900     | 0xdd1e1fb176e3aa266ec0cd73f1289a77ff642544 | 0xba7abe61daac4c04f1f82eddc039f54ee25affe06e5ea49ebb758ebb0284a009 |
| Tornado Cash WD 12   | 2024-09-26 10:53 | -100 | 800     | 0x38277a71e67a74898ef21306dc84390cfdfa8a45 | 0x5c0d1c5271076cabd4b232ff4056f148644b7c02ac91f2f3d96fd69a56228517 |
| Tornado Cash WD 12   | 2024-09-26 13:11 | -100 | 700     | 0xa917ddc3458964088f99dee861e43da7ed72584f | 0x59feef6e7e02fc791a0c2af6cd94ee1872eaa676d7c5b16b5f4ee779c1f84052 |
| Tornado Cash WD 12   | 2024-09-26 13:15 | -100 | 600     | 0xdf7af4e6c8e381780fdeb6e0cf70b4babe9be28d | 0x80aeb8947eaa8fab5892886abfd0467bf3220533c57e64af11e45243f1345912 |
| Tornado Cash WD 12   | 2024-09-26 13:24 | -100 | 500     | 0x16ee72d6e7c34d9e1644b3273416a96fac87c6bb | 0x1360454b6f75191701fe6d1f23ac351f27b2fcb796fabc3255aaaa6ff6dbc18a |
| Tornado Cash WD 12   | 2024-09-26 13:38 | -100 | 400     | 0x2aaf509194dd1ad0df98fda25564a6fb7f01beb6 | 0x4bc2557c82ceecee517650060f369d2f9d64d9bccf6e7d52bbea65c000c7d0b0 |
| Tornado Cash WD 12   | 2024-09-26 13:52 | -100 | 300     | 0xe233de0c3b076bc463e1b19a4ee88666c87ac2f1 | 0xfa5c94908f682e6b80313cd6f788d661a010c72497c5d46868db6ae6cf25cf9f |


300 ETH remain missing. I found them one day but I forgot to note them. Rip.

