# Coinshift (aka "C8 theft")

Date:: August 16th, 2023

Amount Stolen:: $2,900,000

It appears an individual had multiple keys compromised and drained, including at least 2 of their Gnosis Safes. NFTs were sold and all proceeds were consolidated and sent to Tornado Cash.

Based on laundering and co-mingling with other identified thefts, including the Steadefi hack, it's likely the result of malware via malicious Google Drive phishing.

Individual appears to be a long-time leader in the same, founding his own Web3 company and active both Onchain and on-Twitter prior to the theft and since the theft.


## Onchain

### Compromised (Victim) Addresses:
- 0x9e68d31fa10ab3702495c77bb2fb5263975b2625
- 0x5970892478ac8987b7069819ee307d0c255528cc - Gnosis Safe
- 0xbd3496fe269aa8bbf685836b63b3cadedbe2eb56
- 0x83d592be9606663538adcad6f4bc39b22c2eb9d3

### Theft Addresses:
- 0x979ec2af1aa190143d294b0bfc7ec35d169d845c
- 0x68c4a151d436ec1c5448d225a97bd19cce4dfed0
- 0x4c7c2b39e3d642d452adfca632939a60b1baacf7
- 0xbcd5b968a79a04bf2bb942a449f10c20a7121ed8

### Tornado Outputs:
- 0x9F8941cD7229Aa3047F05a7eE25c7ce13cBB8c41
- 0x4E75c46c299ddC74BAc808a34A778c863BB59A4E

### Post-Tornado Laundering
- 0x5d65aeb2bd903bee822b7069c1c52de838f11bf8
- 0xa34500c4be803a608b226e8e6cdadcdfea1f8c96
- 0x4272200ef626d409e9bac681aa0efdb653a9ef0b - Noones Deposit 
- 0x246569f8b420c8d850c475c53d0d59973b3f08fc - Paxful Deposit 
- 0x0258c2af4fe694df026cca55d17feebd5b361acc - Paxful Deposit
- 0x3af55ab7edbca175f80f3a7ddeac5dabf611347b - Paxful Deposit


## Laundering:

### 9 Deposits of 100 ETH were made to Tornado Cash from 0x68c4a151d436ec1c5448d225a97bd19cce4dfed0:

- [2023-08-24 6:50:59  100 ETH](https://etherscan.io/tx/0x815b4c6078dba652d9a1433038e1a7b84e622e0762150ea5cab3f30bb7531a37)
- [2023-08-24 6:49:47  100 ETH](https://etherscan.io/tx/0xb1b2cd6625d2dd48a64e31f2de34526c1bc87b93ce381ba33564d3366db7742b)
- [2023-08-24 6:29:47  100 ETH](https://etherscan.io/tx/0x8305049c3f307fdd2cd39db53ebd7d1fdf5a09f96e828d10937d774e4239f55d)
- [2023-08-24 6:24:47  100 ETH](https://etherscan.io/tx/0xea23678f217f6d5521fa4b724f417bbb204cc173dd6d4e91783f016f71ec4865)
- [2023-08-23 15:08:35 100 ETH](https://etherscan.io/tx/0xf156df23d5e362746327265983bfc77eea8394992d0c98a64678dc81c7276a0e)
- [2023-08-23 15:08:11 100 ETH](https://etherscan.io/tx/0xc19f6e22279a945e2aeec6af5a74ce9c1366a5d060f3a203b8f66f8389cbfeef)
- [2023-08-23 15:07:35 100 ETH](https://etherscan.io/tx/0x057272ac9f1b9f90f802b1845bd1190c1f2a86c80588b94c60216945a63d3d77)
- [2023-08-23 15:06:47 100 ETH](https://etherscan.io/tx/0xe1f199fed6223634f2e9785114dd9aecafac9ed3ba4639b5123cdabc9884c8db)
- [2023-08-23 15:06:23 100 ETH](https://etherscan.io/tx/0x4350fd8e07054313fdc4a4d0367975bad1dfc217750c0a9ba65dd609ac218298)

### The most likely outputs for these 9 deposits are:
- [2023-08-24 6:17:47  0x9F8941cD7229Aa3047F05a7eE25c7ce13cBB8c41](https://etherscan.io/tx/0xae4f5a05724f045f7bcc720c9f88ddab5dd024e08b8f04ebe8789cd4bfd542a0)
- [2023-08-24 6:30:47  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x7c89734cb0003b0cfea8a5f24222d2357a07f4ac5634f5cbb1d13653c0a93313)
- [2023-08-24 6:34:59  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x8f93ea6db99d8a4a979931b7adb61551d1077aba33611e4b7092d25899824ea7)
- [2023-08-24 6:45:11  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x750daa582a682be4d1912c6a87d49e954d89900a1eac0cf124a6c295f1700914)
- [2023-08-24 6:58:47  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x6cdb391b2f3cc82129bbe38bcee21c33d7701e92135c167192f4bb2e6cccdbf0)
- [2023-08-26 0:28:23  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x05ed749eab53d1111867ca646a8cd2e10128cf19392a007e3489ced182f5646d)
- [2023-08-26 0:30:47  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x95f09f1eea597fcff5910fa0ca00194d0989b472c8afec8f42da8a184045145a)
- [2023-08-26 0:55:47  0x9F8941cD7229Aa3047F05a7eE25c7ce13cBB8c41](https://etherscan.io/tx/0x015cd6b0209fef494cec051248a43f88784f8a246633df430ec81f30f86375eb)
- [2023-08-26 2:38:11  0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0xac714a7159996e756d44f544333b19e05f4eb9eec23855330b15c24268f614dc)


