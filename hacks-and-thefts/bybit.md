# Bybit

Date:: February 21st, 2025

Time:: 14:16 UTC

Amount Stolen: $1,500,000,000

Tags:: 👛 TraderTraitor

---

## Details

> Bybit ETH multisig cold wallet just made a transfer to our warm wallet about 1 hr ago. It appears that this specific transaction was musked, all the signers saw the musked UI which showed the correct address and the URL was from @safe. However the signing message was to change the smart contract logic of our ETH cold wallet. This resulted Hacker took control of the specific ETH cold wallet we signed and transfered all ETH in the cold wallet to this unidentified address. Please rest assured that all other cold wallets are secure.  All withdraws are NORMAL. I will keep you guys posted as more develops, If any team can help us to track the stolen fund will be appreciated.  https://etherscan.io/tx/0xb61413c495fdad6114a7aa863a00b2e3c28945979a10885b12b30316ea9f072c

— [@benbybit](https://x.com/benbybit/status/1892963530422505586)


> At a high level, the hack involved the 4 broad group of events:

> 1. Attacker deployed a trojan contract and a backdoor contract.

> 2. Attacker tricked signers of the upgradeable multisig "cold" wallet to authorize a malicious ERC-20 transfer to a trojan contract

> 3. Instead of transferring tokens, trojan contract replaces the master copy of the actual Safe multisig implementation contract with the backdoor contract, which is solely controlled by the attacker.

> 4. The attacker called sweepETH and sweepERC20 to drain the wallet of all its native ETH, mETH, stETH, and cmETH tokens.

—[@dhkleung](https://x.com/dhkleung/status/1893073663391604753)


## URLs

- https://x.com/pcaversaccio/status/1892976342649466916

- https://x.com/LefterisJP/status/1892984150665187375

- https://x.com/WatcherGuru/status/1892996938544431399

- https://x.com/WatcherGuru/status/1892993874043240562

- https://x.com/WatcherGuru/status/1892990693779427537

- https://x.com/jconorgrogan/status/1892967018841743410

- https://x.com/benbybit/status/1892963530422505586

- https://x.com/dhkleung/status/1893073663391604753




## Onchain

## Malicious Txn

- [Safe Txn JSON](../malicious-shit/bybit-safe-tx-71.json)

- https://etherscan.io/tx/0x46deef0f52e3a983b67abf4714448a41dd7ffd6d32d32da69d62081c68ad7882

- 0x1db92e2eebc8e0c075a02bea49a2935bcd2dfcf4 - "Bybit Cold Wallet 1" (Safe)
- 0x1F4EB0a903619ac168b19A82F1a6e2e426522211 - Signer 1
- 0x3Cc3A225769900e003E264dd4CB43E90896BC21A - Signer 2
- 0xe3dF2cCEAc61B1aFA311372ecC5B40A3A6585a9E - Signer 3


## Addresses

- 0x19C6876E978D9F128147439ac4cd9EA2582cd141 - Testing Contract
- 0xe8b36709dd86893bf7bb78a7f9746b826f0e8c84 - Testing EOA

- 0x96221423681A6d52E184D440a8eFCEbB105C7242 - First Contract (unused)
- 0x2444c026ebe6d476e97baeb003071bea9c13a953 - Another Contract (no sneaky slot 0)
- 0xbdd077f651ebe7f7b3ce16fe5f2b025be2969516 - Malicious Implementation Contract (used in the attack)
- 0x0fa09c3a328792253f8dee7116848723b72a6d2e - Exploiter EOA

- 0x1542368a03ad1f03d96d51b414f4738961cf4443 - Withdrawing cmETH

- 0x47666Fab8bd0Ac7003bce3f5C3585383F09486E2 - Direct Theft (401,346 ETH + 90,375 stETH)

- 0x36ed3c0213565530c35115d93a80f9c04d94e4cb - moved feb 21/22 (10,000 ETH)
- 0xaf620e6d32b1c67f3396ef5d2f7d7642dc2e6ce9 - moved feb 22 (10,000 ETH)
- 0xfa3fcccb897079fd83bfba690e7d47eb402d6c49 - moved feb 23 (10,000 ETH)
- 0xfc926659dd8808f6e3e0a8d61b20b871f3fa6465 - moved feb 23 (10,000 ETH)
- 0x3a21f4e6bbe527d347ca7c157f4233c935779847 - moved feb 23 (10,000 ETH)
- 0x51e9d833ecae4e8d9d8be17300aee6d3398c135d - moved feb 24 (10,000 ETH)
- 0x83ef5e80fad88288f770152875ab0bb16641a09e - moved feb 24 (10,000 ETH)
- 0x83c7678492d623fb98834f0fbcb2e7b7f5af8950 - moved feb 24 (10,000 ETH)
- 0x96244d83dc15d36847c35209bbdc5bdde9bec3d8 - moved feb 24 (10,000 ETH)
- 0xcd1a4a457ca8b0931c3bf81df3cfa227adbdb6e9 - moved feb 25 (10,000 ETH)
- 0x09278b36863be4ccd3d0c22d643e8062d7a11377 - moved feb 25 (10,000 ETH)
- 0x1eb27f136bfe7947f80d6cee3cf0bfdf92b45e57
- 0xd3c611aed139107dec2294032da3913bc26507fb
- 0xb172f7e99452446f18ff49a71bfeecf0873003b4
- 0xcd7ec020121ead6f99855cbb972df502db5bc63a
- 0xe69753ddfbedbd249e703eb374452e78dae1ae49
- 0x2290937a4498c96effb87b8371a33d108f8d433f
- 0x1bb0970508316dc735329752a4581e0a4babc6b4
- 0x52207ec7b1b43aa5db116931a904371ae2c1619e
- 0xb72334cb9d0b614d30c4c60e2bd12ff5ed03c305
- 0x4c198b3b5f3a4b1aa706dac73d826c2b795ccd67
- 0x30a822cdd2782d2b2a12a08526452e885978fa1d
- 0x660bfcea3a5faf823e8f8bf57dd558db034dea1d
- 0x6d46bd3aff100f23c194e5312f93507978a6dc91
- 0x8c7235e1a6eef91b980d0fca083347fbb7ee1806
- 0x140c9ab92347734641b1a7c124ffdee58c20c3e3
- 0x0e8c1e2881f35ef20343264862a242fb749d6b35
- 0x9ef42873ae015aa3da0c4354aef94a18d2b3407b
- 0x40e98feeebad7ddb0f0534ccaa617427ea10187e
- 0xbca02b395747d62626a65016f2e64a20bd254a39
- 0x684d4b58dc32af786bf6d572a792ff7a883428b9
- 0x23db729908137cb60852f2936d2b5c6de0e1c887
- 0xbde2cc5375fa9e0383309a2ca31213f2d6cabcbd
- 0xe9bc552fdfa54b30296d95f147e3e0280ff7f7e6
- 0x9271eddda0f0f2bb7b1a0c712bdf8dbd0a38d1ab
- 0xbc3e5e8c10897a81b63933348f53f2e052f89a7e
- 0xf0a16603289eaf35f64077ba3681af41194a1c09
- 0x5af75eab6bec227657fa3e749a8bfd55f02e4b1d
- 0xb4a862a81abb2f952fca4c6f5510962e18c7f1a2
- 0x959c4ca19c4532c97a657d82d97accbab70e6fb4

- 0xa4b2fd68593b6f34e51cb9edb66e71c1b4ab449e - 90,375 stETH + 8,000 meth + 1 ETH
- 0xdD90071D52F20e85c89802e5Dc1eC0A7B6475f92 - 98,048 ETH (moved feb 21) (8,048 ETH Balance)
- 0x55CCa2f5eB07907696afe4b9Db5102bcE5feB734 - 10,000 ETH
- 0xf03AfB1c6A11A7E370920ad42e6eE735dBedF0b1 - 10,000 ETH
- 0x1512fcb09463A61862B73ec09B9b354aF1790268 - 10,000 ETH
- 0x723a7084028421994d4a7829108D63aB44658315 - 10,000 ETH
- 0xEB0bAA3A556586192590CAD296b1e48dF62a8549 - 10,000 ETH
- 0x21032176B43d9f7E9410fB37290a78f4fEd6044C - 10,000 ETH
- 0xA5A023E052243b7cce34Cbd4ba20180e8Dea6Ad6 - 10,000 ETH
- 0xD5b58Cf7813c1eDC412367b97876bD400ea5c489 - 10,000 ETH
- 0xF302572594a68aA8F951faE64ED3aE7DA41c72Be - 10,000 ETH

## Indicators

- 212.30.33.XXX - Feb 21
- 163.5.241.XXX - Feb 21
- 194.5.53.XXX - Feb 21


