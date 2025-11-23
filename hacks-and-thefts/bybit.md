# Bybit

Date:: 2025-02-21

Time:: 14:16 UTC

Amount Stolen: $1,500,000,000

Tags:: 👛 TraderTraitor

---

## Details



> Bybit ETH multisig cold wallet just made a transfer to our warm wallet about 1 hr ago. It appears that this specific transaction was musked, all the signers saw the musked UI which showed the correct address and the URL was from @safe. However the signing message was to change the smart contract logic of our ETH cold wallet. This resulted Hacker took control of the specific ETH cold wallet we signed and transfered all ETH in the cold wallet to this unidentified address. Please rest assured that all other cold wallets are secure.  All withdraws are NORMAL. I will keep you guys posted as more develops, If any team can help us to track the stolen fund will be appreciated.  https://etherscan.io/tx/0xb61413c495fdad6114a7aa863a00b2e3c28945979a10885b12b30316ea9f072c

[Source: @benbybit](https://x.com/benbybit/status/1892963530422505586)


> At a high level, the hack involved the 4 broad group of events:
> 1. Attacker deployed a trojan contract and a backdoor contract.
> 2. Attacker tricked signers of the upgradeable multisig "cold" wallet to authorize a malicious ERC-20 transfer to a trojan contract
> 3. Instead of transferring tokens, trojan contract replaces the master copy of the actual Safe multisig implementation contract with the backdoor contract, which is solely controlled by the attacker.
> 4. The attacker called sweepETH and sweepERC20 to drain the wallet of all its native ETH, mETH, stETH, and cmETH tokens.

[Source: @dhkleung](https://x.com/dhkleung/status/1893073663391604753)



## Further Reading

- https://x.com/pcaversaccio/status/1892976342649466916

- https://x.com/LefterisJP/status/1892984150665187375

- https://x.com/WatcherGuru/status/1892996938544431399

- https://x.com/WatcherGuru/status/1892993874043240562

- https://x.com/WatcherGuru/status/1892990693779427537

- https://x.com/jconorgrogan/status/1892967018841743410

- https://x.com/benbybit/status/1892963530422505586

- https://x.com/dhkleung/status/1893073663391604753

- Attributed in [MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities](./pdfs/2025-10-22_MSMT-Report.pdf)


### Reports 

- [Bybit Incident Investigation Preliminary Report - Verichains](../pdfs/2025-02-24_Bybit-Incident-Investigation_Preliminary-Report_Verichains.pdf)

- [Bybit Interim Investigation Report - Sygnia](../pdfs/2025-02-24_Bybit-Interim-Investigation-Report_Sygnia.pdf)


### Podcasts

- Unchained w/ Tay + Jonty (Feb 25 2025) - https://x.com/laurashin/status/1894432376870375694

- Unchained w/ Mudit Gupta (Feb 28 2025) - https://x.com/laurashin/status/1895474240813433094


### Dune Dashboards

- https://dune.com/tayvano/bybit-thorchain-shitshow

- https://dune.com/beetle/bybit-hack-tracing





## Onchain


### Malicious Txn

- [Safe Txn JSON](../malicious-shit/bybit-safe-tx-71.json)

- https://etherscan.io/tx/0x46deef0f52e3a983b67abf4714448a41dd7ffd6d32d32da69d62081c68ad7882

- 0x1Db92e2EeBC8E0c075a02BeA49a2935BcD2dFCF4 - "Bybit Cold Wallet 1" (Safe)
- 0x1F4EB0a903619ac168b19A82F1a6e2e426522211 - Signer 1
- 0x3Cc3A225769900e003E264dd4CB43E90896BC21A - Signer 2
- 0xe3dF2cCEAc61B1aFA311372ecC5B40A3A6585a9E - Signer 3


- 0x0fa09c3a328792253f8dee7116848723b72a6d2e - Exploiter EOA

- 0x47666Fab8bd0Ac7003bce3f5C3585383F09486E2 - Direct Theft


#### Helper Contracts

0xbdd077f651ebe7f7b3ce16fe5f2b025be2969516 - Helper Contract (used in the attack, deployed by 0x0fa09C3A328792253f8dee7116848723b72a6d2e)

0x2444c026EbE6d476e97bAeB003071bea9C13A953 - Helper Contract (no sneaky slot 0, deployed by 0x0fa09C3A328792253f8dee7116848723b72a6d2e)

0x96221423681A6d52E184D440a8eFCEbB105C7242 - Helper Contract, deployed by 0x0fa09C3A328792253f8dee7116848723b72a6d2e; see 0xbe42ca77d43686c822a198c3641f3dadd1edcb5fde22fbc1738b3298a9c25ddb


#### 3/6 Test Safe 0x19C
2025-02-18 19:16:47
2025-02-20 12:32:35

0x19C6876E978D9F128147439ac4cd9EA2582cd141 - Safe Contract

0x5C6120BA4C5B5E18DDcb9589e649e86EE6d540dD - Deployer of 0x19C
0xe8b36709dd86893bf7bb78a7f9746b826f0e8c84 - Signer on 0x19C, Executor
0x7c1091cf6f36b0140d5e2faf18c3be29fee42d97 - Signer on 0x19C, Executor
0xc1ce312f9519f8ba42bc0656b61c2aa33500e3e3 - Signer on 0x19C, Proposer
0x539b4adbfa5c7c75f80455ff939ca6401c8093a6 - Signer on 0x19C, Executor
0xd5fc69e41df2d910b98e4b1fb444a3a3a37613b5 - Signer on 0x19C
0x815cb309ad0cb26a3bfe35f2de8a5a222de827ed - Signer on 0x19C
0x0fa09C3A328792253f8dee7116848723b72a6d2e - Executor

https://safe-transaction-mainnet.safe.global/api/v1/safes/0x19C6876E978D9F128147439ac4cd9EA2582cd141/multisig-transactions/



#### 3/6 Test Safe 0x509

2025-02-18 18:24:59
2025-02-18 18:31:23

0x509b1eDa8e9FFed34287ccE11f6dE70BFf5fEF55 - Safe Contract, called by 0x0fa09c3a328792253f8dee7116848723b72a6d2e

0x5C6120BA4C5B5E18DDcb9589e649e86EE6d540dD - Deployer of 0x509
0x5C6120BA4C5B5E18DDcb9589e649e86EE6d540dD - Signer on 0x509, Executor
0x174496BC1835c3A55a45542e504E9757b12e55B6 - Signer on 0x509, Proposer
0x21af673A128F3210D1CF023D7Eabd6A95B564A45 - Signer on 0x509
0x6fDa06737CA8908069a0E8b10daCE694d0660CEe - Signer on 0x509
0xee4cDE3B8a24AFB65B0B299d414939C7EFe0de9A - Signer on 0x509
0x9FFbc585aFbb1b4c1426FC5d0e691b21416708fa - Signer on 0x509
0x0fa09C3A328792253f8dee7116848723b72a6d2e - Executor

https://safe-transaction-mainnet.safe.global/api/v1/safes/0x509b1eDa8e9FFed34287ccE11f6dE70BFf5fEF55/multisig-transactions/


### Addresses

- 0x19C6876E978D9F128147439ac4cd9EA2582cd141 - Testing Contract
- 0xe8b36709dd86893bf7bb78a7f9746b826f0e8c84 - Testing EOA

- 0x96221423681A6d52E184D440a8eFCEbB105C7242 - First Contract (unused)
- 0x2444c026ebe6d476e97baeb003071bea9c13a953 - Another Contract (no sneaky slot 0)
- 0xbdd077f651ebe7f7b3ce16fe5f2b025be2969516 - Malicious Implementation Contract (used in the attack)
- 0x0fa09c3a328792253f8dee7116848723b72a6d2e - Exploiter EOA

- 0x1542368a03ad1f03d96d51b414f4738961cf4443 - Withdrawing cmETH

- 0x47666Fab8bd0Ac7003bce3f5C3585383F09486E2 - Theft - 401,346 ETH + 90,375 stETH
- 0xa4b2fd68593b6f34e51cb9edb66e71c1b4ab449e - Theft - 90,375 stETH + 8,000 meth + 1 ETH
- 0xdD90071D52F20e85c89802e5Dc1eC0A7B6475f92 - Theft - 98,048 ETH Moved Feb 21 to Tranches - Remaining 8,048 Balance moved Mar 03 for laundry

- 0x36ed3c0213565530c35115d93a80f9c04d94e4cb - Moved Feb 22 (10,000.00 ETH)
- 0xaf620e6d32b1c67f3396ef5d2f7d7642dc2e6ce9 - Moved Feb 22 (10,066.60 ETH)
- 0x3a21f4e6bbe527d347ca7c157f4233c935779847 - Moved Feb 22 (10,003.61 ETH)
- 0xfa3fcccb897079fd83bfba690e7d47eb402d6c49 - Moved Feb 23 (10,013.48 ETH)
- 0xfc926659dd8808f6e3e0a8d61b20b871f3fa6465 - Moved Feb 23 (10,026.48 ETH)
- 0x83c7678492d623fb98834f0fbcb2e7b7f5af8950 - Moved Feb 24 (10,000.00 ETH)
- 0x96244d83dc15d36847c35209bbdc5bdde9bec3d8 - Moved Feb 24 (10,015.45 ETH)
- 0x83ef5e80fad88288f770152875ab0bb16641a09e - Moved Feb 24 (10,000.00 ETH)
- 0x51e9d833ecae4e8d9d8be17300aee6d3398c135d - Moved Feb 24 (10,143.00 ETH)
- 0xcd1a4a457ca8b0931c3bf81df3cfa227adbdb6e9 - Moved Feb 25 (10,082.10 ETH)
- 0x1eb27f136bfe7947f80d6cee3cf0bfdf92b45e57 - Moved Feb 25 (10,017.41 ETH)
- 0x52207ec7b1b43aa5db116931a904371ae2c1619e - Moved Feb 25 (10,096.51 ETH)
- 0x09278b36863be4ccd3d0c22d643e8062d7a11377 - Moved Feb 25 (10,086.70 ETH)
- 0x23db729908137cb60852f2936d2b5c6de0e1c887 - Moved Feb 25 (10,028.06 ETH)
- 0xb72334cb9d0b614d30c4c60e2bd12ff5ed03c305 - Moved Feb 26 (11,243.47 ETH)
- 0x2290937a4498c96effb87b8371a33d108f8d433f - Moved Feb 26 (10,021.55 ETH)
- 0xb172f7e99452446f18ff49a71bfeecf0873003b4 - Moved Feb 26 (10,000.00 ETH)
- 0x6d46bd3aff100f23c194e5312f93507978a6dc91 - Moved Feb 26 (10,000.00 ETH)
- 0x30a822cdd2782d2b2a12a08526452e885978fa1d - Moved Feb 26 (10,000.00 ETH)
- 0xb4a862a81abb2f952fca4c6f5510962e18c7f1a2 - Moved Feb 26 (10,000.00 ETH)
- 0x140c9ab92347734641b1a7c124ffdee58c20c3e3 - Moved Feb 26 (10,257.74 ETH)
- 0xcd7ec020121ead6f99855cbb972df502db5bc63a - Moved Feb 27 (10,023.91 ETH)
- 0xf0a16603289eaf35f64077ba3681af41194a1c09 - Moved Feb 27 (10,031.25 ETH)
- 0x40e98feeebad7ddb0f0534ccaa617427ea10187e - Moved Feb 27 (10,078.92 ETH)
- 0x959c4ca19c4532c97a657d82d97accbab70e6fb4 - Moved Feb 27 (10,166.51 ETH)
- 0x0e8c1e2881f35ef20343264862a242fb749d6b35 - Moved Feb 27 (10,042.57 ETH)
- 0x8c7235e1a6eef91b980d0fca083347fbb7ee1806 - Moved Feb 27 (10,040.81 ETH)
- 0x1bb0970508316dc735329752a4581e0a4babc6b4 - Moved Feb 28 (10,262.35 ETH)
- 0x660bfcea3a5faf823e8f8bf57dd558db034dea1d - Moved Feb 28 (10,061.51 ETH)
- 0x5af75eab6bec227657fa3e749a8bfd55f02e4b1d - Moved Mar 01 (10,022.98 ETH)
- 0xbc3e5e8c10897a81b63933348f53f2e052f89a7e - Moved Mar 01 (10,089.03 ETH)
- 0x4c198b3b5f3a4b1aa706dac73d826c2b795ccd67 - Moved Mar 01 (10,000.19 ETH)
- 0x9271eddda0f0f2bb7b1a0c712bdf8dbd0a38d1ab - Moved Mar 01 (10,000.01 ETH)
- 0x684d4b58dc32af786bf6d572a792ff7a883428b9 - Moved Mar 01 (10,104.12 ETH)
- 0xbde2cc5375fa9e0383309a2ca31213f2d6cabcbd - Moved Mar 02 (10,060.59 ETH)
- 0xe69753ddfbedbd249e703eb374452e78dae1ae49 - Moved Mar 02 (10,077.61 ETH)
- 0x9ef42873ae015aa3da0c4354aef94a18d2b3407b - Moved Mar 02 (10,004.38 ETH)
- 0xd3c611aed139107dec2294032da3913bc26507fb - Moved Mar 02 (10,017.80 ETH)
- 0xe9bc552fdfa54b30296d95f147e3e0280ff7f7e6 - Moved Mar 02 (10,153.56 ETH)
- 0xbca02b395747d62626a65016f2e64a20bd254a39 - Moved Mar 02 (10,094.12 ETH)
- 0xf302572594a68aa8f951fae64ed3ae7da41c72be - Moved Mar 02 (10,062.36 ETH) - stETH
- 0x21032176b43d9f7e9410fb37290a78f4fed6044c - Moved Mar 02 (10,044.40 ETH) - stETH
- 0xd5b58cf7813c1edc412367b97876bd400ea5c489 - Moved Mar 02 (10,186.86 ETH) - stETH
- 0xa5a023e052243b7cce34cbd4ba20180e8dea6ad6 - Moved Mar 02 (10,000.00 ETH) - stETH
- 0x723a7084028421994d4a7829108d63ab44658315 - Moved Mar 03 (10,207.50 ETH) - stETH
- 0x1512fcb09463a61862b73ec09b9b354af1790268 - Moved Mar 03 (9,997.09 ETH) - stETH
- 0xeb0baa3a556586192590cad296b1e48df62a8549 - Moved Mar 03 (232.07 ETH) - stETH
- 0xf03AfB1c6A11A7E370920ad42e6eE735dBedF0b1 - Moved Mar 03 (10,000 ETH) - stETH
- 0x55CCa2f5eB07907696afe4b9Db5102bcE5feB734 - Moved Mar 03 (10,000 ETH) - stETH



### Indicators

- 212.30.33.XXX - 2025-02-21
- 163.5.241.XXX - 2025-02-21
- 194.5.53.XXX - 2025-02-21



### Annex 6: Bitcoin Addresses Controlled by Hong Kong Trader

[MSMT: The DPRK’s Violation and Evasion of UN Sanctions through Cyber and Information Technology Worker Activities](./pdfs/2025-10-22_MSMT-Report.pdf)

> While DPRK cyber actors often facilitate the laundering process themselves, they also outsource laundering to third parties. According to blockchain intelligence company TRM labs and information provided by an MSMT Participating State, DPRK cyber actors likely outsourced some of the laundering of stolen funds from the Bybit heist to Chinese intermediaries, as they have done for prior thefts.
> Outsourcing to third parties allows DPRK cyber actors to expand laundering operations and launder higher volumes of cryptocurrency.161 As of September 2025, all of the stolen funds from the Bybit heist have likely been cashed out.162
> While reliance on Chinese facilitators is common practice, the sheer volume of cryptocurrency stolen from Bybit likely required DPRK cyber actors to expand laundering and cash-out responsibilities to include a wider network of the DPRK’s overseas apparatus and more third-party facilitators than smaller heists have required.
> The DPRK is primarily expanding its laundering and cash-out operations through Russian intermediaries. According to information and blockchain analysis provided by an MSMT Participating State, DPRK actors worked with a Russia-based broker to cash out at least $60 million in cryptocurrency, including some of the stolen funds from the Bybit heist.
> DPRK actors also coordinated with a Hong Kong-based broker to facilitate the cash-out of over $100 million in stolen cryptocurrency from the ByBit heist as of April 2025. The Hong Kong-based broker used the wallet addresses in Annex 6 to receive funds (See Annex 6).
> DPRK actors also utilized networks in Cambodia in the cash-out process. DPRK actors worked with a Cambodia-based DPRK national to transfer funds to cryptocurrency wallet addresses in order to stage funds for cash out in other locations, including Hong Kong.

1. 322BLHv1BNQ9mJfZERtsN1a7MrwnyTDF9U
2. bc1p7tr3xyj7mmmpptmr58gne9jfs77a692me69wzq9zwr2nk6d7dyaq9a203t
3. bc1pwd8l8j6mp9ktn03y67eftkkunwv7amcgeevc04y4gtzke950aggss330qw
4. bc1qr03n9c07p3w434w99uclf5dzyfgp3glz9suqnk
5. bc1q7mapml4sfc5nk0ra5723a782vzsmmv9eg7kff0
6. bc1qgd2xy0w55ktdfhvapqh4ger8rpmp4rz22dunfd
7. bc1q2ncyspvrh05h2vngk64um02aumyz0z9jghyunv
8. bc1qp8dnaga0depn4tjtudm42malcav5ztawv5qn43
9. bc1q6cwt5vsgp0s0p224syrpzmedqrqaa382vpx402
10. bc1q2g0mnxp779ckulhf0qrk6an59afr42t5s6r8ka
11. bc1pm87lqhktgwhk4j9hhs328tardmexf4lpjwkde36w62qrv8sw05cq6vprvq
12. bc1p0n6tchu6uu8fvz00ap8ng9fsnl3y0f4z8d4muzrumnxk20jdadlq3w6jpf
13. bc1qf4dnd26e2nsmr9a4d64stn44g3kkaynu7evyj2
14. bc1q5j3j6z7plxjuj82ew46a3kl8c3qw3rnh9vth6y
15. bc1q8cdap23tq5v6fzlhn9a9kufd8fjkehhlpehhaa
16. bc1qp6rxf3sl9c2e32zfzzjq29d258rzpzhlhpz0dd
17. bc1qkdj5gktdfsn5hf4yt7wjfpzgz5g04jygtf07aj
18. bc1qlhd4gqtk867nj7e5e8hryyv0uq829n4m8tj0hf
19. bc1qfj4jsmkg4u4zech0ft8q827lw3sfpurl9rutyj
20. bc1pz5eadcgvwwyad7ea9myd2ftfg68rl798e7vhn5v8yl0cz84wntzqnwxe5q
21. bc1pzs9ey6sugzvweks3u5u9scxzllc0vyew54hun8ed68dn7sfwgcwq72hfx4
22. bc1qjmgp7t34z63qm4l6umzqdcucd8umvmkszd8g4d
23. bc1ptzxl8kqgktrj9znjyw7p4nlc053e0hzap6cenfux6mgg25wydj0sv0m8gc
24. bc1ql0pj0m9m4zv2tj88s5qmkdm9gp8mgejkzgymmc
25. 35Ksf3WFVSgmMwNqWfFnCEkfmD7bHfi3uW
26. bc1px4m5zuedlf79zsl4hlp8p2svdm303fcax2z5uyrqtsaeknhrc5lss7c007
27. bc1qj0rsus3lmr9nrz7uhz7r2tzgwhm974nsrm9pcd
28. bc1qdqpdd4pfey05kv2j8tvym6rdu4ysl27z6qxje7
29. bc1qkuka43ywd0cnnmvxgklwuvp3dc4w7ahh202jjw
30. bc1qaek3t2e2uttc2ax78t3823hmfp9s9c4uqfdxhs
31. bc1qf5pwnlpjlrmtp9y20cmyquhzhr0ukcvcxfcevx
32. bc1p3efhp7vdk3fpktvwyrjjv7xwt5uaunecv9kr0n6cchwehvahl58q473v6j
33. bc1qek4yslqnplcg92mljpml0we46eus6ygg7uyrk4
34. bc1qs0r7e4t7wvmwzgsvv8nflqgtcy35c6cfdrynuu
35. bc1p82xjnlgghflgmgfjfwufxlp7wj58jsmctevnn75pwt7pmf2ydggqgq8trs
36. bc1qs08hklgy2mc4srshcmxuy4zcm2l7paz3qjmqsg
37. bc1p09ndd295tascvcas5ta8fzxxkalks8dvjnx9273k9zka45hl09gqnljkuf
38. bc1pkseyk4vymvk94ncm5c4a0mtydl5egzwx0gfyx77u9ff9a9apjdwswxdeka
39. bc1pkd74e687fvvt54yktxdrqqf2d3e5jqmk883kftkth2cryfve425sva6mjh
40. bc1p6fy8lzhlj97q0ne6hljaj7f53kmtxys8zctv0jxd82smtr6tmtpqpd07c4
41. bc1pzy2w6dhkrr02lhwgwxhp98s7rp9fe2xqk7cvgxscx44arazllr3swgxnll
42. 3F2Ukje3xqY52tm7o3CpuuTJmVg5bAWfde
43. bc1p0djqslc4zq9wph3n570ms2u95ehn9ghqz83ryllw8kpr67jtg9yq0r78k8
44. bc1pz84htvgtywk40x7w5sqtf372cnvs9z94sjm0vf7nm4vdq9kcld8sue7mwu
45. 3GH3o1U8JyuHoA3HG4p2LNZwko7AXMXEDr
46. bc1qz0tfke7le0qjfpes53eknwyfdh23hu4g7cf6qe
47. bc1qknc6rk3nzkh0zksuvdus5tz64z7s43r083vhx5
48. bc1qx0zcj7tjduyq92m0f078nuzlvxg3mxa2galtnc
49. bc1ql7987q80yjl7lh592pvxjlfz0r9yw396wzeleq
50. bc1qjgrys6mptskym9zq2tv806x99c3nmq8wsglulq
51. bc1qljjt8dsnd8v7uqj3y4awvdv6z70gq22dajvhjr
52. bc1qfy8u6p9usm3epetk6wnv0axfklrwcg4r9adrqc
53. bc1qh55527ce2l7h36t9a74dj9747076rnjul28xhu
54. 1CfixayZ7bba6fF9pDyX7e7wNmV7hZaCA8
55. bc1qm780f9296mqva5mz539z0xxd48kg96jd9dgqtj
56. bc1qgw0xhmc6ajgxdsmj6r6v6np633xll5s2d6rrq3
57. 145YnCwFBAsYRXp7HTxJHtwxLL1Q7Khwiu
58. bc1qwdzqzrtl5npnadrjv0kamgkpltvjjtkqdchvzq
59. bc1qfg8r0xgl9ks26qlh4rwejgw8ns3mzztljvhmss
60. bc1qw5r3uf3sz7pgpee92p562hxc2ymuwu7vu3qgmz
61. bc1qypytt8pyqllhl0r28yljweuardsrpptgvuw5zh
62. bc1q3ege9e9ggajzm86ych53wm9dmq2z8szsyx63kv
63. bc1qttm8z0vnsn0kzj2xethulcmhgk70rtu3sy2m9p
64. bc1q8k5u7mq4kq54cm3tq7hsn7p28xpu5c3kutlqq7
65. bc1qwh70nxfd4lgajl959rs2qgevv33fvc4tw9sawr
66. 3HU41jQJ6MFoAYzVsTBxG1tpKdmYpYaMsz
67. bc1qe0p8xppkzt8yuzjkxln6gjw8xktg8rtrx0n0my
68. bc1qa5j4ydcs2g2casakj3t725wkreywccefxff3vc
69. bc1p3xpgvzdp3ns8wnw7a93
69. bc1p3xpgvzdp3ns8wnw7a93nzgaeems73m800j4gwcmsrej0j696es5qwsl4x4
70. bc1qjfw89cuge0q7veqnge47507nka57x43l3mgx6r
71. bc1qt2lqelvrv7afv04pj4ju53vn230h9ee290jpuj
72. bc1pencs6wngluvk4aayypk7jrpg7w7hn3766hvu7vwdkleue6cl63sq6najw8
73. bc1q8agwcy55pw99zsuw0eqtc7vuvfwtrn7lp3yxx4
74. bc1qr6c0a303xne4lp9tnkdcet9raymylaw7ef02ap
75. bc1qd80kmf2fjmqt0ay6ntls38kpytsje8y539s6w4
76. bc1q7d4tdvz8eewtdyjqcrfst6tejjulgejtgldc0f
77. 13nPTovCdyhTo5Rb8xGEB8mBobEtFrfB73
78. bc1qrtyddqcrdtpp72j7p7qre2zt7nxxz8gduwpxu2
79. bc1qzkae9d9y9cexvjegyx5kdj22fplsx4pna3qgpd
80. 1B6b6YPdp7HMtLC5453SiKckax2K6LVJta
81. bc1qmp53xs8xw6q4hpnq3842le0mlqtpe0whzfjy54
82. bc1q5l2ym4pjda3l5pqvh2zntx53s8plusmuj5qeeu
83. bc1qv0d69hwjg7tjdgxt47fwz5rcmlfpmwwvl7t4qf
84. bc1q9r2262mfannwrscel8qn7hqr0usk2735tragas
85. 14sdAQW1Y4eLSsFCD2PAShUG9aXCtAXf5Z
86. bc1quawf7457ra2s7r7khre2v8s08gncwhwhksvnpa
87. bc1qmql48w6h5wf0pfvjz0pwcd87r45mfpzcg2dpgx
88. bc1q5jy334z2t6nlhrmhcuagjw2y4yj0xve63trvwj
89. bc1qqr3wpnaxx9ugzt33dma4xwfg82t0lx2wnnvzte
90. bc1p8myp4tlfadptv8lh93tavreqhq7wvk5mmk9a36y7nt0lcw6mr0asts700l
91. 1H2ZnxA4es3LjpLzwpaB78tPqE8vjK8ThS
92. bc1qzjx99lz06vcetv6hrm62lmcldnpkj0dsqnckcs
93. bc1qazcmu3ce6pjr9du63ef6g4d32pzjmk8hpdt47n
94. 12kTcTqc2BPKfQVAHeSNEmwp8LQmKeVYCq
95. bc1q9am8qe0yth4cv5wq9r3r5znyqw05ay8v7f6fqe
96. bc1qtrk0laxd2z20eyddvnxkj2g6yq2c3nznfpz6ak
97. 16oke474qNDWkNfC4816yPVJ29uZNvcDET
98. bc1qfgvgh33n5d0jynkr24kr4udtlvf0zwqmcy5fzj
99. bc1q57t94f7j8hkuygrttc5re854pmyen6xhnlwrud
100. bc1qlu05kadxzahuc9gw3hcxwrkd8wauq7mrcqv7xr
101. bc1qy3qlxt5jyyuzluufvfnwapyqe67huscv66ezl4
102. 15HTDWCdpoxzXZtVfd1eAZRezS9gs82XFB
103. bc1qljwnu9p9uasy6q8qdacdgpu05fjfg2y3tugjuy
104. bc1q29aexqflszm932sw8qes3nzyjac8psz2g2xsvm
105. bc1q2r6lh6fc8gt6jhuxw97hh8vh237hppr9xrzd6x
106. bc1q0sugc483t3uum3v994aavddwqrgd4rmtenmt0m
107. bc1q8968vcg8340kf0w2darjd426xt6k5dpzu4x60d
108. 1PsRqgkFVCdqPrv5Lfd7wqABfYViQ3zj1d
109. bc1q5dmexndr3pfn905xd5j0hf988f5y7gkmdvu5aq
110. bc1q6aysh2c4lg2gv8srg2nu2q27as3s25j0xc8233
111. bc1q4kdphehrjhtchch4z8e5myfszarallqlljzg6h
112. bc1qax5g5fdusqxu0crh86j8zn3ahtecdt7et6ffpm
113. bc1q9mlgnyzlstf9ktj708hqnp6mey2xdfmeteh72h
114. bc1q4s9ndgfulqf92hdjt7zs4528xtp3sm8k34j4hc
115. bc1q288z494hkyvqahrv07lsmr7twwnlkqfah95s4w
116. bc1qdnpaj6wfxyhay03zuk7ca68q0pcg0c6kv3nu73
117. 17Tv4RudV9yS3JdXrT77gTzWzcd8ic8PRo
118. bc1qtr5me2ftvdp280alpdvalw7gdwuwj5ukdtwkp0
119. bc1qghm2svadn66ld0kepgjxu33w5egatwv2ud3y60
120. bc1qd87pacd3p29zp4ywqwc2wyamdaf55rajj3pmg5
121. 194gvN72YYP2vQ34uuM3KMo6yeKQKgpZJ1
122. bc1pdsxfnycwd57nk8vaq32qeq5472xev7y5vkdzrvdawk2gns7nt2yq9j43lq
123. bc1q5jg2l94acj72ltrnkvdp3h6r90epk4jrn3z420
124. bc1pdedc4mxnengwdxalfxzl2vxky8n53s9nqk3qwlcyhvn673qzqhyqzrz0q0
125. bc1q4l9mck0rezs5vl2te44s20f680xef4x0rkr39h
126. bc1qykeur8l6kxwhrvlkvc26ayqfagh6k6ymhzdz4u
127. bc1qlcw4zah8pphzct9cjuymmv02y9avl2skveldck
128. bc1q3dnglj255dpwtya3q830zjte3g43dlg0sedzp5
129. bc1qkv5jdtwgm82xae3g2672v3ltk72xm44yzxfe30
130. 16VJRzDvVzRUihBWcU9DUGcYeYLiUaB1xc
131. bc1qxpawgw2mnh76a4hlc9lgphughkrlaqcs8jge89
132. bc1qrphhxrklmfq9nw6ggmw6d3cy5zfpe69md5cu09
133. bc1qtyqj5zsj79llms309zl0ccw798yt0maw2mmfwa
134. bc1qax7tewc67ucyyy6vdkakpl87ejgxze0h2fzucl
135. 1FYmCpHkbaFrNutHrsXwJ67a5r35tv8kpJ
136. bc1qhkhj0tux8hpuz77krycs8chhft27mg8kdp40pd
137. bc1qstewk22dp7q9mtzcrp70d3hxy50t7qt28vctpj
138. bc1qqdwdkja3y4znpdkek9tj35z67d5dsqap5xcqr6
139. 1Aroc9ytmWKdcUroA22m9Bo2QcoGRmjjGU
140. bc1qu25609maxwalmesa0rd7408hpls7vhcg057k4l
141. bc1qn5w5mxeuhwwms7tf3c5tnxyswp65326v54n7nv
142. bc1qg7yhdkw0hjnhu7t4npye66g045uxxt5frzqk9z
143. bc1q9zlldgsjm2cdc3ejjj0sd6n82yw6apmxs557he
144. bc1q8x80urzdd67g6pd9j9uz0mfv8hhdqyz9ejhr86
145. 1NbtsYFzpHqhfrFjXmidT9kXSmS5frX4ub
146. bc1qd6n6jpcd4sr8a93s2whuaamqcz60e84n492pk0
147. bc1pa73rg25ytwjvear3hu65v74m8prgxpvmnj4jzdu0gr5g4cacmqzs0m6wa6
148. bc1q7m98m862ke6r9fp5ydzx8nk9jx3u4sghsnt5t9


