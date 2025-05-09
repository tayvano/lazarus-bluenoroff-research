# Bitcoin DMM

Date:: May 30th, 2024

Amount Stolen:: $305,000,000 (4,502.9 BTC)

Tags:: 👛 Trader Traitor

---

## Details

### FBI, DC3, and NPA Identification of North Korean Cyber Actors, Tracked as TraderTraitor, Responsible for Theft of $308 Million USD from Bitcoin.DMM.com

https://www.fbi.gov/news/press-releases/fbi-dc3-and-npa-identification-of-north-korean-cyber-actors-tracked-as-tradertraitor-responsible-for-theft-of-308-million-from-bitcoindmmcom

> The Federal Bureau of Investigation, Department of Defense Cyber Crime Center, and National Police Agency of Japan are alerting the public to the theft of cryptocurrency worth $308 million U.S. dollars from the Japan-based cryptocurrency company DMM by North Korean cyber actors in May 2024. The theft is affiliated with TraderTraitor threat activity, which is also tracked as Jade Sleet, UNC4899, and Slow Pisces. TraderTraitor activity is often characterized by targeted social engineering directed at multiple employees of the same company simultaneously.

> In late March 2024, a North Korean cyber actor, masquerading as a recruiter on LinkedIn, contacted an employee at Ginco, a Japan-based enterprise cryptocurrency wallet software company. The threat actor sent the target, who maintained access to Ginco’s wallet management system, a URL linked to a malicious Python script under the guise of a pre-employment test located on a GitHub page. The victim copied the Python code to their personal GitHub page and was subsequently compromised. 

> After mid-May 2024, TraderTraitor actors exploited session cookie information to impersonate the compromised employee and successfully gained access to Ginco’s unencrypted communications system. In late-May 2024, the actors likely used this access to manipulate a legitimate transaction request by a DMM employee, resulting in the loss of 4,502.9 BTC, worth $308 million at the time of the attack. The stolen funds ultimately moved to TraderTraitor-controlled wallets.  

> The FBI, National Police Agency of Japan, and other U.S. government and international partners will continue to expose and combat North Korea’s use of illicit activities—including cybercrime and cryptocurrency theft—to generate revenue for the regime. 



### Theories:

LOL no DMM wasn't address poisoning.

I get why people are saying it but the vector of this attack looks much more like a private key or system compromise.

1. That 0.1 BTC fee on the theft txn. No way. They would never (and had never) before. The attacker wanted to expedite confirmations / didnt give a fuck.

2. That suspect address poisoner (1B6rJRfjTXwEy36SCs5zofGMmdv2kdZw7P) wasn't even Onchain prior to the attack.

3. They would still need to want to send 4503 BTC for some reason and just fucked up the address portion. Based on history, this makes no sense.

The weirdest thing that points to maybe not your classic key / system compromise is the fact the full balance was not taken. 343 BTC were recovered from the compromised wallet by DMM only 50 short minutes after the theft.

### Looking at the theft txn and prior transactions:

- That big April 4, 2024 txn was probably the transfer that gave the attacker an idea of what the balance was on the wallet. 

- The theft transaction could’ve been pre-constructed based on the assumption that the wallet balance would be at least 4500 BTC and each input could be as much as 500 BTC.

- Which then enabled DMM to be able to salvage outputs from that txn that the attacker couldn't be sure were not already spent (even those that weren’t actually spent)

    - For example: DMM salvaged one of 10 BTC outputs that was unspent. But another 10 BTC output had already been spent.

    - It’s plausible that the attacker noticed this and formed their theft transaction to simply exclude the 10 BTCs.

    - Or they didn’t see it but still decided to just take the 500s + one 503 BTC output that they knew wasn't already spent. Basically, choose to eat the 10s or whatever to increase the chance of getting the 500s.

- Further, the 343 BTC transfer to salvage the remaining funds was co-spent with an internal change address that was also on the multisig key. But the theft transaction did not require co-spending from that change address.

- It’s possible they got the raw keys and figured they had one shot to shoot and so they constructed the transaction in that way, I guess?

- It’s also possible, I guess, that they didn't have 2/3 correct signatures for that exact 343 portion of the balance in that wallet. Like if there were two 2/3 multisig configs??

- They had access to both signers but not the actual key. They trick each signer to sign.

    - This assumes they were secure and used hardware. As they’ve been around for a while + Japan, this is actually a pretty reasonable assumption.

- They got access to one signer but not the other. Then they…

    - Pre-constructed the transaction -> signed it with signer key 1 -> submitted it for signing to signer 2. Race is on bc if real signer 1 comes online and is like “?????” then attackers could be rugged. But so long as signer 2 signs & sends….

    - Pre-constructed the txn -> somehow tricked signer 1 to sign -> real signer 1 sends to signer 2 for signing. Only once it's in the mempool do alarms go off.

Regardless, for some reason they couldn’t or didn’t have 100% confidence in what all funds were / would be available and were making an educated guess.

They had to pre-construct the txn for whatever reason. They didn’t just have full, unfettered access to everything they needed.

The attacker had those two required signatures for a short window of time—they probably expected it would be detected immediately for whatever reason.

So they construct the largest, lowest-risk txn they could figure, crank the fee to 0.1 BTC to expedite confirmations and….rip.




## URLs

- https://elliptic.co/blog/dmm-bitcoin-loses-308-million-in-unauthorized-leak

- https://twitter.com/CryptoEvgen/status/1806831622848922014

- https://rekt.news/dmm-rekt/

- https://twitter.com/zachxbt/status/1812466959109521649



## Onchain

- 975ec405ac9dc9fa5ab8009d94d6a1fe31dff8a8127ea90d023104e52754e4d7 - Theft Txn

- 1B6rJRfjTXwEy36SCs5zofGMmdv2kdZw7P - Direct Theft

- bc1qegcazuxnp5wxxxamdqvjv345fpve6656vpjln4 - Initial Tranches

- bc1qgcv2j80009apvjekph40wagwutfu6l3gcm2fw0 - Initial Tranches

- bc1q2u9m2eqy8glvrjeqr5sceqngpad6dnxrtyxlf3 - Initial Tranches

- bc1q2tu4dxyvnaquar96mj99yqjanfzgg3fv4gzytd - Initial Tranches

- bc1q7p3atj3v95k4pd7qxnnqlhjwu843ty2hqn9gy0 - Initial Tranches

- bc1qr4vnu4f4tl3gwfxt6a5hgt6vuusgsd0j2cnz74 - Initial Tranches

- bc1q3ur23g02rq5w0x6y8vek3xradjgs080nzksfje - Initial Tranches

- bc1qrtltlc7zjzj3knde2tqjt7tl2p5l2keh4l2uka - Initial Tranches

- bc1qx6jpnnfjrfcx9ehhdmj7qqyzpyd8pek00trrq7 - Initial Tranches

- bc1q7pdecv2raf3x84unxlv9ghtpjfpwlam6dx27xd - Initial Tranches

- TNVaKWQzau7xL9bcnvLmF9KSEQkWEs4Ug8 - Huoine, frozen by Tether with $30m+ in it




## More Onchain (Zach's Work)

- https://chainabuse.com/report/7a1ce276-3347-43d2-8b16-c1a7cf2bfaf3

- https://twitter.com/zachxbt/status/1812466959109521649

- TXNdzqFtG6P6rgC1QRTUkCinJFkPV5ghti
- TLk8xMroBtfktfhbEQRjukAYiKfpZZZZZZ
- TSgszvfFoqqGAsTDrFnKBpNVTaz98TaJxw
- TQ5ZCEt62YfLUij5rc2cq4A8f33mTF6qeu
- TRDM9BCs47p3LASdwiuG6oM5WXjdTNUZPy
- TTifUomA2r3Bin29pKDJsfSvB8Mt13rrDr
- TReLpqj3oN33v18R9DfG9Gf18mDvQcppa8
- TFVU1AbTVFD93WKRYxvaYjgeDXGPdyWn3Z
- TLUrkCxPcD5RkyzL9sPbBYBnG7EWYCtr2c
- THQRFHs4YMpfSNA5nKWB9gwjwJXfKfXHT1
- TW8mvzScL9AhdXbUoe3aAQXeiA5J119gG3
- TR5F41LPNNkwud1GzEtETV68Jb9iet3Riu
- TRcw1TFSjS1VH1tH6YUyKsX1NoXazdzTg6
- TN76dtj2WvhFJTpnTaR9T3PZUAS5athZGb
- TAGyt16oKEAJftkZU2JVNrBvUsMMgCRcvJ
- TY1QugSpyVprAC4hHryeThoF1YHVKkF9Q7
- TYAVj8ipf15Ft3VVgb4BQHNZpzc3K4Mjao
- TFkAdM1qPBh7X5h6ScBeyn8Xi8veLN9abD
- TY9rSBDK57iQuky2fiutV3ZVwTiPC2f2Wc
- TGyt1wXv3vjz2zzjXYDg9SJA7TBno7VL9v
- TCcMwSB59W98zqTBknUupqY8FBW2oPDyxF
- TRkqkPM59NWrqddvfXQkzWgsjzxdz1puwx
- TKzUt87AdH7cbTnUtSFdVDsHnpp4wZVHsn
- TAiwbr5R2twbsoGDb7q2Z8MDiRdoKuahfX
- TDdGgKL8PbFU9nWFEjQzxWn3yM3hk53YNi
- TSTK7R3d6EAFkEw9sMPhBUPSGmcGqqhsit
- TDkzNmoq7BPkZUJvhYkLJayMwToaJ3JBFP
- TFSY2dz4c9dK2G4f9B95FuQCyukyCXg5TJ
- TNSE27563e3ehkbD3gQMXYTrxRMuBadQCr
- TJZsK7ekdqTTwryEzG5v7v1Jv4Pi3WyHNs
- TD8MtkWQu8rVYWyaxyVmKpBqhmRhHUQAb2
- TWQAodyxW4z6UKfbggk8s767VedawVYpNw
- TSFTBH7YE6S7uob8y41KPkqZnCQNqmTzuA
- TSS7ja5JdnG6LwVgs2j3LdvyG49z2qEPPo
- TNfbZXDyex4KKhqvP4Y49oGfSXMwGocDnd
- TNUFCRpwWwhdokGtRBiQSzSyg479yiYwbU
- TESGPwEfQrvdq3BS5hLSzVer5rGZPEAE7A
- TMUDRdBztLo3Go6FqbS1ei7ni1GpBJm376
- TJLjDddig7CjtyQnACbddox5DdKF4mr68F
- TPvEw2P1SthGwYcjffRthcYnbYRHSwfUEV
- TApxWJjMfeBmRfWVgXRcZwvsSX2wAYzqHq
- TK3kgnpUAgGRGdJLxPKiYcUvkNnsdG5qkj
- TAx2HjnGAb9TJPQmtZt1j5KXXV4y5nT45Z
- TGxoppR8X28WRNTkRsRzKhx7beTt86oAEM
- TN3dHwEKbAAiBXh4LZQWSn7BoKMeCNMJKb
- TFGw4ZSjHTwuCej2HNvtQLWAgPxQMELRq8
- TPq1e9gda22ppk7BSGw3Y6AF9awTTNAEba
- TNADSkMgZ6AfKKjZzxmEiTWs4ethheknoL
- TB6gEPaMwLVCgZn9E24PiEfC9g5vy7B9yP
- TQTGU3Kt6xFYm7L3CfAYTzXn662znwD324
- TUUHdAZZFnTz5NPk9NwB31BhLYY14CfQRV
- TNLvM3nnAbhGW9aCpKnPHmuxbswR36d7XG
- TBkKaPWbpUCG7zA8yPNxFsqPoFw7AikQnA
- TE19qEJmuhDELFiJfpJcLvnQ3uXo5hbj1j
- TCQDU7P3tZ3T5RytfKXsgyDWJgTZgRiQvM
- TJbchEgFC38Hh1YAxBRPsi9XgZcjJcZbgn
- TUUCQ9f4EB3rKN3g18D6Nnrfyx99cKwWd7
- TBpzJjqT8oB3TuFRTaee9T7vNiXBeXQN9p
- TBCViJW4XqmHaFnt6Jmvn3QTUvpUy9RRko
- TWU4R4UB6SMX2KSBMnW7QCfsDHCDdBDEpF
- TZ3ZQaFXBK3bRrudXGyhVmgPDfJ8iev84E
- TPWQTUEogVGA8PujWRmQ7Yict2hfEdXAtD
- TDqa97fq94pFhE6PbdtR3cooTFry9TsLjc
- TA3qk3tqTc3FD8pjCpBPL35soBT3fwk57M
- TJD44h4yjid6okMn4htAh9GQZ1KFGtqBDa
- TYNgrhfA4AhZSUpHs4urVy1kpDgQxdsbzg
- TJFhfu3Lve9SAq17uVrch581DVDuz9bFUa
- TB8VRHxxwF6B6hJ86pweKuekvFyajZ9WHV
- TNs8qWhe4BN4pJ13AYoyySP9G58Lo9sow3
- TF7QF4LZtBGSvaKkyASbBTqYCWCDr62r7o
- TP6AhStKSWESbFZajnMi4A2Jn5eW7s3qga
- TGLiNxAocqTbWWdnXDD11RahiQg1THEQmq
- TLPNfFjEK8y9WCYhiBT3VkLmmQw1Q69yiw
- TAM65qYbCKYTrA2cgMY5LvUvhLmtk8pjSW
- TLD5CUvuxNsWe1bvSHPzXDaDREUsw5F9hq
- TVvvPPq7tjo9RnAeXFxwU5wTrLyxxVVhQJ
- TSDMo2ZDE4oRczEh1w3S9UVbYNmmhebXkU
- TF6Rf5bmtTsVD3HF4Ggqk9ShyzWrzSmmLH
- TK24HMTSjxEvS6oPieLm7XrTGR4W4rCj3v
- THfFBDaFVr5cLJkjnkWdRmYEb7n9pvsUuK
- TFweU92H4uZiC8uS6imQsMyhFwmbfRrxWq
- TGbmLVNeazJm1JsKyNMF5jvm2NQYoTLjiH
- TYSGPajNmRUCUQd7psXV5cUaXMtD3F7UkU
- TCXP2UQj3c9XH6jBRbbKtPTbA2MTYAhjCT
- TNPPGzf4zAqk7yjZ71e95GYAe9f5pgK7Q5
- TE8sHdZxK1G3FipTEnpBMnt4cPaM7LvdaB
- TRVtvP4FnxwSmTrE14QxAMobP2oHtiYdyX
- TTKvn3SparXSMEyYS8a1jfhTfa5iNtMQSw
- TKCtNLUei9ec4hjy3sMgkhN3QUxkxiHnKA
- TQHM84wA9RyuLwtg1EcLpMFAtVE4paiXwk
- TLfzWNZctafNcSZd9DjyY3rhesBSVkxVgT
- TTdZ5GuoBCb1kX6DNXNpvAwnys6GntERWK
- TZ3YiExPCwSurd3LjHQqFfRfTtegchEvoi
- TCR9TaF17R5p6MxZCcW6mdMx52UpngMKJF
- TLzdMTCFVVYS4tkTuTceNXZQgQXrNbak1u
- TG2ntEzUvQbdjvVgUQQgRXZg6sxGAtk6C6
- TXqYZVrhtkgJH1D244MSxeBkcRJPeyXDo6
- TYee8oGPhyCXTQ383oXqP7H18ecah7KHVd
- TP7VrpdELeNNG1un2VzSoSUfDN5prvid7i
- TJ5z7SRVLDu2bD2BC9TRVRStaFP9EDem7Q
- TWkf7KnaS8FcCXeMMDuMfVMg6rtihqeTUD
- TTNYv4BxJi2NHPyG22sh8ACdpz4NBKRrvK
- TVQsWUzkXKYJciS9wbCj39tQhPKcqs5iVy
- TSNWamSLZvs8WJMxviRemcSbzTuUA2S4MS
- TSzJZ2ahFjQYT3fT5ctZoMBfNneK2u9Kr6
- TFtfiJ8EgoatNpNr4cp7L73zdWVigZZk8D
- TKjNq7qRyxS2ZgUiWSyENvNMXSngBLQKSJ
- TH48YH4aVVVzC1akLV8LtTJQs8GLCcct68
- TNwctsv1PU73KzpgCFWwasLB5vFRrHPe5n
- TDWQZ4BP2UnNttxktcuTgQKFQuVxAvmnym
- TPoAFeEtZvL41AWvtk5b5vBvVYXpZEvr4i
- TLShCnQz4pzw5kimTWJykEQ7pvjA3nbgrR
- TEYgKPg4i3z3msFxHrrem3jWsyH8QdjLLd
- TFu1YCC7StUa6GGGk256s7skZsFLMSReuR
- TUZ8ND439ViyybSFak29yUPxW25NANYiW9
- TRhMf9viVk1PSUnfL5enawyMVZzB8MkJjy
- TXPBdLtnLNsaHyfSs1YQfviwt8uUxypsL3
- TQvcSHycR5x22qxZ7xSLWirSCzz1dETVEQ
- TMrSHaWBbPqkKVfSdGj6kZ6xPJH3EnMntr
- TLTnrjg5Ux3CVcwHrnXsu23XfAqfD3qEuj
- TRpXF3yHc5wTX3iRdMKLvEP9ABsV5Qk8un
- TNoNfGrpf6EZFJpNTyCJCRFaHusS7StRZN
- TEi5jAkVjaFVWPyix5YJTpMUDm3kioeXfL
- TNEJg83wWnYCZM7J21gEeHYu6YNL5C1vuK
- TYku5HrnkcKMUTYJauSVmohpm4NjFxc6MG
- TDrV3nMFf19yTtX8UPywxJ2JKktmHUUQx9
- TLEDRKjL9RnvAdGXYRTKrKG6dMs5SmBaAY
- TDodB1teNnqPok3LvokzJeRVVzJ3kNbAUB
- TDcuQCCAU5EycxeK88nFiJ5GSJ9TdgGHAa
- TFBYiia4yHAy7xbL6DMVZqrHwbMrqZFYYm
- TAwKU9sxFUnuwNecenKEotGzRYd2Wbuh7a
- TEUUZuL8UGrZa3aKF1yPY5TJMsciD3oCAi
- TG6LbLRfnG3WoH5rdhAATHr4zhf8cEBHGD
- TBz34btrJPEDEritH6GWxAnXoG1ukGJoem
- TPyadBVkhuewTXx14Y6ceGmLykCRKxxXko
- TDcryFQgMtyFGrojyMAtPjNqQ24AYXARV8
- TKzzoRqYoFbX6BDB6qzqiUXKdFbAGHGiNc
- TSA87DxAKPvF9WpvsvEx2xeYf4bwqqVYeY
- THC1oBUp1YjcQrD8KmHE9sPeQK6RJ72zLi
- TJuLCrcpzjxuipkipTeymdGYUssnGq6kEV
- TPDdoyYESZuSbnsuFPtnWnm8GZXpp1neZs
- TVYkTAx5xnkXN6WyXbK1zZBtUdS9gB3Tcn
- TG1DEVNKwTLZJN1xcJo9obBun9jHtgixFP
- TT2PuYbiSZ2SnB6GEXLkqVEP7JKoaimFYf
- TJqMD3rh5VXVn2GsAhVJZ5p6KmJt7DDEqP
- TQo9bUtpAk6iCzT8Pujgv53CfpUaU8Kmcv
- TBuMktM6ECzTCVDjVF3zBpTDiQkKZW7tUK
- TAoiAhwzPvy5pmfGrqTKMh3HMfxFxbKoho
- TXQ9D7aJFJmPofxRmtR5FNN8vwPiV5v4tC
- TMJXsULQTwvb88bkEWWeKgHmTcYApvMomm
- TFVcUJHvNA5BxnEjroRvhKArWUm7BtaDzM
- TG9V8K6sGMfh3K26MMKrxmZHzy3HJnuHpu
- TQXU95jk1BgwD6bDGAwki3utcq5ZuXyiVN
- TNVaKWQzau7xL9bcnvLmF9KSEQkWEs4Ug8
- TQuFSvpct2FeBrKjRh8NDqtGAci2Z15RSa
- 0x4907cd89b1d637d4ad7a1b7b5083895c366ad8d1
- 0x265184cd695541d94619344c059bb4189b7a8169
- 0xde9a506483bb4ba84a5b0d54fc9b27d35a60b8e0
- 0xb5d52d33fc51209df574720cac8280f7e82596e4
- 0x467272e44ba99302764011e1d549bac1042a7fdb
- 0xdd3ceef807bb03baf2aecac0c257066d2e66b847
- 0x88ebdbb62e545c2bc12e17ef16b992481a9b92dd
- 0x5e49d4a1834004784128ee6f61068d163dd5eae2
- 0x0a0758fd51a366c5cf74f5c1f51e911a3d156f19
- 0x770c6168a598835ee63ca22b5c4c9f6ef009d02c
- 0xdbe71d533dc07bdcf0fe2732d3f58ffff82fa44e
- 0xc287bf99d85849bd59c9fde7681db87cb45eb769
- 0xf47f5557515ad8c1cbed968e7e726d6ffbe4245a
- 0x4e12a3ed9dde4bbd0672b5524789ce7b0eaa3f53
- 0xe192627af208640a136a4f4dd242857fc89ff00a
- 0x46ad680e53b36aecf105ceb0f5ca1bd722c37a27
- 0x4aa235295fa3b6f36831f58912c40c4e61603131
- 0xab0d24f80f33510df5095edfbde0fa090583509f
- 0x63db683fd61a320173ba7488070bf0770c5d3dad
- 0x1031214b080e0d92ca9b22756d96fe01a8f5f532
- 0x423841fa08c3cb8edb357835dad9c97e3e41cf7c
- 0xdab79cf1e6bcd59a4f42f0acdaa16dbe07bda508
- 0xca5aae49eacb6bfdccd7cde696b564fe43633512
- 0x46191e507dd73b0ed5962465914e6e0bbd35d9a7
- 0x6032a99d92955f24799f3b9776b8821045d9e87e
- 0x40fbb4699b4c83436f94c72907e182c8b31b1853
- 0xa195ac7bfc96e619e561318a49a93b818e4a3436
- 0xf435cd06859e1ca496b0ec5c297a08965b816617
- 0x0e20a6c78e3d142e8b67dc5b930f068d5c97ce47
- 0xf0735ba2dd4dbe021b6ff7d7166577e07906dd6f
- 0x43213584d2a21193f2f2b221389b533ef12b7c4a
- 0x3bb745926db205923e2b6ee340ad8af0493cd3ce
- 0xf2a9eaee751e9180412c1eae2826fa45f7b60592
- 0x80f580b5c2e0bd004414304f27984e799210e289
- 0xe4c9a9ca98df8174567af0367ee2d2c46c2a6287
- 0x67d4fbba31bed23a041b915c63b085dce3140e1e
- 0x047ff596d30e12a9f636c97eb0bad56a459b2927
- 0xf1b3e8a32f537accfdf1bf0915f97170f3ee58cd
- 0xe8683ce774a80f35a7c347acbae7a3ce8a20a3d3
- 0xa655e25f19f5c889b635f4124b2677335aadf0d2
- 0xf9eec396134237ec5a226ffe8e9875989c71344f
- 0x5e233701bbddc59b513798c456ac2a13d6b51f1b
- 0xf08d0cbbffa5ce44751aa057ae17b91cf716936c
- 0xbafc885a478d6ec3a1dcaedb3dfe020079af14c6
- 0x968877847426528002d77aa0a9443a0aaac39026
- 0x9bacf3cef9c1a56eb4610ee41073d97418fd1405
- 0xa193dcd56aaff0efa8e9520aae29e8bc5f09f4b6
- 0xd6f9c24a42b11dbac55af7cbcc10ef40aa47af3b
- 0xabe5eb9722b950231e11d2adb9559eaacdc45d90
- 0xad317def69cdb5891d0e0166c9dd46eca161e876
- 0xb4553f2a66f5b6454250ef9b59f771e232baf1ff
- 0xcc3394ebbed23b343bc31c4b032d4132f82b8b70
- 0xd90b147834769e408051e292f178bc2b18744e1b
- 0x79e3469803fd17b090b6dba9028452f20a2f7eee
- 0x779e60dec391d484ea832a3c9f65f30d4b3e032d
- 0xe5f42ea6800eb3ebb135488d672fb37ddee116ed
- 0x8c0a9fb9fe44028c2bea4a75dd5fabff18978f71
- 0x7d389a8899552d2c5cdd56d831a55732f83f9f2b
- 0xa6b018ef6423a255cd342a44f3f288f41c04c324
- 0xf7aeed0eb7ad9ea5c70846776d62d9b8b669e416
- 0xcdd5dff859deeb74991f2f6cd7a2fd50c2e9a2e9
- 0xac09c4713320b83fd287dbdd6242d5cf46a50e4a
- 0x1bf721a1a7c2e72dc6f4c4bf7b3334fd63432dee
- 0x30449e24707e4868702d23e3d7399beee21afcdf
- bc1qxajmxrl9q22dw2m42flqtqalcn5ajv7g2fxsdl
- bc1qy6jw9ajgzdqdglal5rc3qwvq3gka3tvv7yh5y9
- bc1qk8u8q7n0rgk77d4pqncruy04vnay4hwn7jjga6
- bc1qhlrj3l69hhs8jvtxqxyjnngrgaasnepstt7ffy
- bc1qly9xrzr2my87n9eq7prsr5phwqsngfddl2sgzk
- bc1qmjjg24cl2j8g8mgvva7ra7rspwvfgjaym4d6tr
- bc1qs622dxcu3hucgpe276e7nlz7xc2wvumnq8kadp
- bc1qadf3rnqatregumq087lazdq5vfjmpscktr23k9
- bc1qm47k776tszg4j0mh0af39w0tc6r34un5dnml0s
- bc1qzwg47h9t90ew65h9yvp5mk00lkhwufw97emrqa
- bc1qnnnfsx4wnw28nrhmvyk4kddd0wajdl6xkdvy53
- bc1qsk2spx2888l0pzt263vu0zthj9kps6f34nxw2f
- bc1qqy2q2ctuc658fpdgfxcf6l2nhghdfdxqwcw6dw
- bc1q870538akcyu0dfa5pzxjutvhthn2tr7epmsd35
- bc1q6ffcfgjagpt6zcpd0w9nkkhkqmyewnt7dr0klh
- bc1qkpsef4lzpwkdkcddswhxcksm85cny7ek7r9jnj
- bc1qp4z98s2szvzvwq7fyq39mhfply8qdjta62v9dg
- bc1qlne9gfx3tqvedc6pumqpqg8xn5qmv66eh27wmg
- bc1q3p4us3ajuj3kj28a83307nat595stt9chqd496
- bc1qex34ul2hcy26fn7vjkyf33jej4t9pecc7fqy3t
- bc1qgc89d2lwy854je9e79qkr7hz23fv2w0wvsjapl
- bc1q2hfa77ha0e3dn765lfujtq6vn09tyy4pl3zye7
- bc1q45asz2mgz8vj9650338x2kkhc98t757237rcwe
- bc1qushcsrw64dagrjtp7talq7u3pt25p2ctzy3hud
- bc1qtl9320dlpze6j60mnm0fh3ycpaa6f6a0h09e3y
- bc1qpxkrvyh68jxx67knq3y67maj2l4ffa7hcvs4cx
- bc1qje5xjn536vyswzyxy2nnw06uszklhv239qm77y
- bc1q6w6wfprgdd8tf4lr38jzj9tlfxj27rv28n6x9e
- bc1qdqktcuqch37lgpj9tm0z0phuklgfmxqtl2hh20
- bc1q66rgg028rv37ytmldt8r98sl0h3aqwp96ucuk3
- bc1qew39qzl20kfx55f8xa3epx6tgr99g2p6h5dlh6
- bc1q5y3dn6058ep7pqua4fph58zpeght9mfmzwvxky
- bc1q6vw0stdr6kvc5skj6unxpxhgrecr3wk88uptu3
- bc1q3xv6gkx0409muwh2e0jd6vgmhczczu3daj69ua
- bc1q6z9mpurs7awdgu49ept48uu2k6j9avkga0gpss
- bc1qdxfte2lz2emz450lfkkknq9paqn8ndd0h5zgfy
- bc1qmvupdm0u8yqxaq6dagxhq49hknmtqzcccxnnj2
- bc1q36qdrc5q2qk55f7v62t2n7a63mrzygu5cw3htm
- bc1qjgc26na34t34hmtu5yn4yr2g9aklurqlr0p4p6
- bc1q43ga6yhqucwgjewmegft8kpczzjlj0qvp4jwaw
- bc1q8gufljtuhceu7z4wjzd4vzkh0r92twh2kfn37s
- bc1qma8ewrkzulycd5wdzys2z4ldj7fxyqn9n646al
- bc1qz2kh6d2a3htvpys66cxss6s0sp53w9gj4ujdh4
- bc1qvfj0tllmnsnltgvl3nvuaz2vnwdwynfwfftrch
- bc1qy8327ttfw7vl793f6tu8xdsx8elc2v2wl6cyqr
- bc1q2nv72kyxcaxrsudqqemrgzdfunzqcdjsz7kgy6
- bc1q3exfjsmlv8c0vazjxljq7znjz65m6n4dajcsj2
- bc1qsmxlwrt0uer43u4spfr489w0ht7ak0gveqcx5z
- bc1qhdema3y4453hglutsfe4v0nj3cnkd7z3zgrr9e
- bc1q4eq3vknm3wunq9pqf5xdvmsng2k3dfj8lz9hly
- bc1qg82xddp5rdwm6h3nvfnpzqt4ytfw4d4uy2zc59
- bc1qrpwx7eknmm3z968kgsazf4qxpw0g9jp0cy0tag
- bc1q4y602kfq9ughkzfgnftvckapk7pdu6t602eqw9
- bc1qpcnq72427nqy8wrsr98al88jdea7qzjjx69qfc
- bc1qzffhelcl7qsks33a6gw0wmulu00yhvp29qthxh
- bc1qdgyym26gwlxae8xls2kd6ctalezw0qnctf2qk2
- bc1q4z38e04cs03kw54c5jxpx66a932zkxmjd838e4
- bc1qr72p694wz93na9guvzalqjgwaraq49v7v8lw2n
- bc1q9ss3r9cl6dfl4s6wvd7nagp3avrqez4z8edup7
- bc1q045gph75mpqj0ecmnksjrx6pyts5xg7tqpap5c
- bc1qmamqv492ymu68ym44cr3tywa2wjtypugxgjj4w
- bc1qhm5arpxycym0uer3cfud34gmj0j0nykhgfrpp5
- bc1qsx4sqxh809psk8sw2tskqcs7qdfv0n0lu6smfv
- bc1qkza3jl08a945x2env62unal6ad4kwz6xy9yw2q
- bc1qj0sjany482m59m44lugfep4hcdunt9f3r9a0ct
- bc1qzv2mak3250j7dqtwe0z97xsk28exl7alwgmumn
- bc1q962lh2thg229rcd6jgrjxv62j2j6f2r8crmfat
- bc1qydfm3hc07mu58dm3r5cvcqj2lwja3x49l8anxc
- bc1qf9e06wg4kdlcndr624vwk5jp00c9ru3gn2zv2x
- bc1q0fy8hnu5vzdxn60e8sqqq3880lwlwjjwm9yu6d
- bc1qlx6wgvp74s9f6q7tue934gedl70jrd6x22v8vz
- bc1qs6t7397rkj6um9zxf4rmekfxky5ufdfl7flp22
- bc1qdvvykcd7j8x0r8xthu65ktgyyuekatwjcnvwfa
- bc1qs5yxytfjas2uk365e2u5xttmxpts0ydq39uh54
- bc1qs3059p5lcatqdunvha2x64g2ppd5www3tufnu0
- bc1qkr39gnk28fmshgtp6pup903p482dn8z80zjngg
- bc1q6q9l6mt49ykf36ecc5t66j0p08xtuvdajnxzf3
- bc1qzfp3wd0nfd2063clrgxnpv6fjmq7lw5kj5mh2c
- bc1q39ppwsg9l4dth8dlt2dq4jzl0xfvq5jye6vfy0
- bc1qvglx702sya939k859gx74zf8ua73rudk0u049g
- bc1q6svjnmt6932mk4tv5g6nmpznwm3fky98gt4gdg
- bc1qe8p85tpwje6kza4dl0jmr0l7969l0yzl40lwr0
- bc1qhck29fjvl35pstqjgs7ns5x7jwphn3szqzzk2u
- bc1qnjlv2xpj0p5ravyqaprd7z8el3dcev3yjcuhsd
- bc1qp5ar5490g0g356dxzjh96lnshfgza8zj8ggmyr
- bc1qz4099eywkzlnmxs2a3xjm6rx03d50fcrcx8pnx
- bc1qdr6afcw2jrq6x2f9gtqqcs5s5y97z5tr0kfth7
- bc1qgsudkgcd0hhn2xv2vlenhmgr0n8vxyq7wf7p8v
- bc1qml8hunvzpnepwpaud0emkpxkcrtvelca9u4wcp
- bc1q3xwzxk5zg9tsz83nj2eal649rdstcxy0p4qn0a
- bc1qh3hxuy2ppcass06nlcw7de5pmss4wch8p2jd74
- bc1q9lcu5jyqz25n0qhlt09glg49lktznzwdywek64
- bc1q57y9rd6y6878qqfvz75lkgwa0p4z5dxvyfqlrk
- bc1qr9pq5ru553auaemtv5r73dax50seu4k348s262
- bc1qzeutqsvg7qnywn4xyjfqhzvjtdumkcee7qxzv2
- bc1qvyf4pl6svh5r0wcnpvz2damuzn9v6lnhrwey2w
- bc1qfkk0253dcdv57trav366lax09ntnl2ymmrwu8u
- bc1qapn5vawzqwyw5gaaezctp5j55mth32hatv48g6
- bc1q67axj5e2c7npmz0w3pgusyrvqkmjgk2fmfkwg0
- bc1qssmeulwwu9n4uam2zc06x26x9rfltpsxeu52z4
- bc1q7ae39qupstphc4mdp4ds6728kvlr0fcqh7z2fc
- bc1q8hd6y3dlwrmlhpkr63k0dk7sxzq3akcv07c6q8
- bc1qw59xw80lj6z5kkfez6n309eh9d46sgra6wahf2
- bc1q7tmprffwf6kddjqs9fnffnal5s5sw43lc2w52t
- bc1qnhfhxyy87prs5yk4qq5xhfdr4qyulezhslckvw
- bc1qzdzzjvce40808qsd8vxf5lk3en4agmseylej7r
- bc1qpk8m3udf8c7kujcwe0j8gc6ae2lujmzxyxk0fk
- bc1qnsrj4etdzkf2h6d38360hdfnqv0jax96ed5de7
- bc1qu0zk3r7x03x83mkav8zqq7e9cvdu0mm37yv30l
- bc1q2uxtmszvgcrufcdzc0jfvh22uvglj0qp22hykd
- bc1qwtjs5l87h6npr688j6tlc2w87gwa96zpam5q2j
- 1KDLAX9fYakfAyjh2tcHnMUrR99cCEMtZE
- bc1qqsskkgrvpt7pytagv6wjgqn8qeqd50fzztpcj2
- bc1q28n0nx8qfm2092r63484gyd957z9lcds7d83jz
- bc1quwpxzcakxlvfeafz4jaa6j7cfuxw5d2jy6edp6
- bc1qfj5f7q6dq0utdzecr0c6t4mjajzpmmqnv8nsz3
- bc1qtzr22qk3hxuu27g3hwk9r3k9c8vqufuqr54gjk
- bc1q3w58pxs92yz3hnlx7fv4xpcftuxca6kda6zwku
- bc1qgz7egx52w640caelfzugckjfnp2v47a0wn5sxy
- bc1qq6uf7epaq9kauj4cvyww2utqr0vfag506fkm2x
- bc1qjyxq6j4nex636pwlvuy6atymhr86mr6emu2e07
- bc1qmgkcyvgs5ykw45hcn3frefrceymwqesvynzkm9
- bc1q45vslpezr0f34uw0ema9xu4c8w80j2ltkwkc5z
- bc1qpan2kqkz9yc3effs6yzgmksccjvm45zu26rxh4
- bc1q3lycqf5d35kmnxdcd7z34jk5mnpa2fnr6sc2jt
- bc1q23eu5js6m7vuxjzhhmcdmxs35ccyuv5d7z00m6
- bc1q7jccexmkrhq87f7yu4d8a3gsvsq74s33sxk20c
- bc1q7k5lr57v0rp2wv72d8jsncpdtlr6r44jhc0t2j
- bc1qvwm980pqqq5eemphw77dl6dm4qjyhr43600nex
- bc1quwgkmp557jsl6dm2m07lsvvsvk4gyenw7wummf
- bc1q8rwund7gskjlha5thvufmgt8kslvxevjxg6nzx
- bc1qzcvlyljaqtnchc3hy8xu7eu55fn6n3a05a2uav
- bc1qzfvsjv20gg5jlkx2gqsd3a3ds3wce7mwedxlka
- bc1qegh8y2guy62ru8nnhkv4dmfszthrphlsgj85xv
- bc1qwjr2flhd8j7znyc8rv2kmpp662vwm3x0aecz6e
- bc1q55r6q9sekeduwqxzksqm2mra57esp89zltqs87
- bc1qva3n86906ty90f3mq907rk3nv3u2zk7rmykmzr
- bc1qqxhyc0cnaypkq6shzfprru7e8lkjdamg03he89
- bc1q9endytpf7fyde4a7pqf8nx8pdmq30fr92mg7y7
- bc1qujxgqd9qu334aukzlzlgljlgmy803guc79fz90
- bc1qk58cgas30f0jj9ks9n8wvggkj7m930xn8ndg7n
- bc1qplvjq40dp9wz26myxt9gykmuf72vwx95n8rulk
- bc1qyaqyvs69p0vvdw96x59emd33dkhpyeq4cgekkp
- bc1qhvxnlu7husa7m02fe9qkrznfultgc8wufyudd6
- bc1qrdlkkcckt56q60r3gc227v3rspr7vhlz3acvn7
- bc1qw63f8j75yw9mjgy35uxalcznpmltjn7k0raap5
- bc1qhpnp03ng80xpm2qtaaddxzhql4t97fw9cjnl23
- bc1qkxtcm0el2cwcgy7vl2fn90zgwmm9r7z6rkf6lp
- bc1q5c5tn4t8tngda9uf9sn5mzu7adqx4l2k6uycn5
- bc1qwjy89z29tjszcuqgfg42rwj42uy9xk2k7xlj93
- bc1qhjsgl2wjts5su5alpa99d97stsch85hyxjh5ak
- bc1qk845c0rfhppk3v5r3zx7yvzj4z6v9703y993qh
- bc1qj99886kplq46l9shwf0uy5fgluexk2wup7375k
- bc1qgernssgu8an4vcsl24n2getn6tckqrr6zakrda
- bc1qrhh954rqs2z3jc653ddr5hy2a26zprztdyhkj4
- bc1qkw750c7k6vjunlfy8cdz883gmgv03qxlkczptl
- bc1qqt6r658an4peclvaz5xxhr4enhcdkt33x2d4r8
- bc1qh2qkzrchtc0ltmn49gjfptgmhfulvqucfahkv3
- bc1q8vnscx4cp53220ug0m80chqt7cg8y4790qz38e
- bc1qlxg3f8nmrylrnh0fqj9ukc7atez7fkv74tlx2d
- bc1qhjngu4f4q436h2m5ghaq32qgwdk493k40egrpr
- bc1q5940xmqyx4f2def7l8zgt5x5z7wtqemndxr0a7
- bc1ql89hlrgaknjmvc7ge0lkttnfnkcel0pkjt478x
- bc1qlhw7u3fs8f282s50xxrgagw5x6qq0z94t2pk64
- bc1q5329twldrg3l3738up3s3sgzvkk70sqxeyuz9e
- bc1qx4jrrx4q0cuha30k5erzmnf7tfgq6eucxtdy4m
- bc1q4uh5jr98euu078j5ea9p9l5l4q8n0yuq5uduu6
- bc1q4dl2kg662mwr8y85j0eq9sxgvaypavmukyepc7
- bc1ql8euegjm03fztlneg6mr6fczfwkfw769s7amcy
- bc1qjm4z0k5gp4rfd7nsq2akdjne0afl0y669vgr0c
- bc1q3mjnd77kj83tqjq6l53wx50nmdz2q72aztl583
- bc1qj6rt5s5xma75kc0789zg9tv3gmqfwt0d4zu5lz
- bc1q9amrl000age7qzq4u3pxku6hwxvlxj4utwlnrp
- bc1qp047ju0tscj8adj9nc44p8xp07l0cl5s6xua4j
- bc1qk67argqpkn40ll7fe822ltnl0jc4fjklnqeqfm
- bc1q765m773gnpqqtg5w2wj5tv878ys8y26mmh4mzl
- bc1qhsv08hfzwrqkntcsvl8ze7vmlaghyl4kfu9nhy
- bc1qn5rv4tsg4l9gmq2q77udmndq8y94u4r3qaxmwx
- bc1q9n97c8xjhv2uvv0nw67jexgtkd3yzz5spanrlm
- bc1qm3znnhd5khx93qwev2cn0dxdd0ya0xr2juemrw
- bc1q5slepq048fvt6s8l3tt62dnrqvauamvxc7scvl
- bc1q8txc86r9tt2w8r0244gawe0q57q4pv6zcen92g
- bc1qefqvleepnn2tz40lmhn0yswt42nynmrdmm8ckf
- bc1qfjtkgwfhz806y3g8pvyrzn8cpduymxyfwmctwf
- bc1qmm3ggap8erze5aggar9ycnl98skea6htd0f2em
- bc1qz6l9fr6g82nenkt4lmfhpl63u8ldcxt2djkfm6
- bc1qsptuhydx23qhs9gtv3cl33y708fv4rn0pyrs88
- bc1qaj7um06rzajjtlz2vqn29n9qn92vdc7d2jln80
- bc1qu957wvstjd8q8gpau7tc8futxjpj4yaefyj7w8
- bc1qe75ctww67uqplzl8m4dvtf5x7dx4npamqu2nuk
- bc1qdpxjlrjwydq0t95vl72fnzgu4dl0qhy6crprym
- bc1qtyy3gvwx4krxw2r2y7z95z8m4j0gpeasavkr2e
- bc1qycjdtngncjs7syw552g500u5mcnptasypnlcld
- bc1qxjgjzdps8v0y29r8ev7etustlja3x2cq95zwf2
- bc1qg6lr7glxptccgjv0zfy3xqj7337mh679x2uf9d
- bc1q7txzwgnzk2w59xfkj7kwd48z0tvmf059hw7843
- bc1qru0nvhlvuks3fuw8jlm3aga0saqpe039fw348y
- bc1qc5wt434tudytna3uuazwcc86kuzt5h2dux2cn3
- bc1qttvspx0vcmhshnsy2he8a5tpzms2hsq4ep9rs2
- bc1qn0whdfq02scujetqs830flaupzjqqv00pswyx8
- bc1qe4gajzjxthenrs9q5a9cqdqr9zp5v9z49s7m30
- bc1q03ees6mpcv8ehtxx8c58usytjvwcj63ujcxw0g
- bc1qpnkktpza4cy7hk6n4p82qquqnehnp2k2xmenj6
- bc1q6egesdcfj9h3y7qvwaxrfvjkwk83j5yah23w6x
- bc1qp9rupdmgz4na73r5vf3d75exewerhhdt4ydp4p
- bc1q5cw4e5peql3c8tuap9y7vjxwy9jqqykk688hwc
- bc1qq00x0hcz2gqck8pja8axjrgyncgg5gsvusw9j2
- bc1qwwyvrfwjxrqy0e2rs4rpsuatm9awv2697akgny
- bc1qlv205mrkrce9flfwtnw4u00kzcv894xhs28re4
- bc1qmf92kw9h99t9d66taq5ztf803q3rqnzfddekv4
- bc1qqzlch7spkhv5c6aa6cxjp0fpukmczms3ypy6ma
- bc1quvvl63sg9f24277m6uxf83fss36lesr7tvmspp
- bc1qvc6lm6umup25f332krzya9nn8yvccfhdz08qgp
- bc1qnkxvzyhp7pqm9q7qtumdm6tjc4922vgmsm830d
- bc1qtvh9yt7wwpnc47yksh3smax02waul4lmxhcq3f
- bc1q5jlv7397xyrtskewemhjud845dsmt6k0tldwpm
- bc1q5shsqhsrsmxhdu7uaf05c73eh2dpj33eyvhaf6
- bc1qrntvpfzqfclt4kt0tdcjfl74q8q5veh2rel8t4
- bc1qk45a3szmvchzwg5kgr8k2lv9syulzwa5653pws
- bc1qmutjr2k0sc4hgv0wsv0saxlsgne8hpdwrrxd2t
- bc1qkskprldjn0v5x0lry9kj63zmatqhfwv0sdq7sc
- bc1q6vzayy5r674mp2tn6xnqf7zf5zj6fsgy4k65hw
- bc1qkyd92q8var5ysvxgnhml67hw54nc6ree3yr2q6
- bc1qrmcytq7af0x8fvnnm8f838flmgllh364pfwglq
- bc1qxhe9jyqjznfmsdf9wauw5ku00fjv86vkr2rkun
- bc1qp448spkfpude6rgs9zk7cess3nu07sr7kue8wk
- bc1qs7fcneeurv7j2eg5ksvm33a3ag34fnugulqqq6
- bc1q96gmw3pwyhuuew9vgu9xx47razknas0zuq5gy0
- bc1qkdp5nhxdq299v4f7tlrphpwshnw6frx72hyfr5wp4w2kaldc5knqdmx2c6
- bc1qudx97rc84uyw7nxcmyhfxfdf6xcaruux72xecf7gewad44whl28qdc84mr
- bc1qc27700fqd7we9ypwyw2emwwqn3srjssnq4gt8auw4uvkpc68sc8s9ckglq
- bc1qxdgk2te7xsuqcs92c5sgvwvv68qc3vs97xschmyl2eyjtn0yua7qcz987r
- bc1qev9dz2s062mzuf4la94n3fkxcvksdwn2xvzgnus36dxed65lv52sqxw9p4
- bc1q0fmgs8sze74trw7m3t6hjcvx6akkt5wwlqf2cpjkqn05p4av4uqs2cxmqh
- bc1q5c9uyqlfcwd5vfyvw05dj5ncznxnkxy3r6ynhrtr8k9g6awlpw8s6tjq4c
- bc1q3j6wyauz6fgh956z5c3ssjds032d0wdz5zv0frhyj7rgam8yt7wqus7vxg
- bc1q07yuyfpxk4qzl3vd254ucwerdpp6g0v9s2p3qp6hyjtuvnv729aqgmzljp
- bc1qasq2v7z83d4r4gc8a8xk6x456d4r9v532sc68mz0askrpqkfvv5s7uk8r5
- bc1q5wuz6vmdhw8pw05xyaxn5pkn7ryfe4av2tjw4wpf6n49fm8qy7zsdvemns
- bc1qudj7tfa0galrss584x2qfptnwjaepj7wtrnnjgr87aka5xu3x2jsa2j22y
- bc1qcuhuaa9c8lqfh88tc8ndj9clwmhc3h00w325tyh3ctl7daax6rvqqntpsc
- bc1qkldhrg6f80dkjy7fre8fda8ltc3mf5ypv5ucgr
- bc1qpnea88z7tnvkcs429sznkt4gdw8zrpkpkzx5g34kg0ukw0crzlgsvhzgfp
- bc1qw0pvnczfmkw5szvycfzyjmc5522qul75vfv2kj
- bc1qh0qhqamp67zsd7j78yea09k5p97eax5p0awehzv37dwehcl5yjssrhk4z7
- bc1qtv6g3z30mayswksengzl5ylsehmaemds9gk0e8
- bc1qx3dk3a89h8vswqkuvs3kdr2hjf8nuctlr44n96
- bc1q22ydt0z0tnad5n3m6re9u38zy6426n80c9nlp2
- bc1qp24qqp4652qslavy7q7a0l2uey9eqsjhcaesy9gffx3zw0zs5c7qv47qpy
- bc1q205z4d80ap07vjayy005sgws9jf4sq6vjhqtjnehm2ameu6lfhzqv27d6l
- bc1qhrkz0cnslg6dyndapjvvth3jcf4wzfxyduuhxghz4pj8qdytufpsgzu36q
- bc1qkp45gqzmcevfjd06gmku5sykl3u8ctl8fegdu4
- bc1qk7q8pscg2d7cadf43r64amf72yc8n7h8w4u527jsyxdq6k6wke3qhls0wq
- bc1q5nkl7e0avzlvrdk0reu0vpu0227mvh8xzcynfq
- bc1qa3k9wwh7d45mn78j6nzwf6fmp5dfr98cupf9y3
- bc1qrc04ajlns857cdmqwgf9du8w76yccllcqq45u8hqpr5ewnxq6ssq05zsdw
- bc1qgrq9spz04m0u5lfy3asujtlwds2gcwv7p2rtc3
- bc1q64wvwmptuxqvn0pw9dlhrsa4ccqkp9r4gcnpg3
- bc1q77tx3j3vnhtkd7yupkeay3eg0akev4guac5vqze3gj0jej2jgfcsl9dc0n
- bc1qkvgufev2zqz527q67c3m3acw9jzrc0lmpcwvux7kws9qsq8fry5qda5s0h
- bc1qj9qh5y9y6f0rgn04xszgjywzd02cvddwjgh2d4pm0ze7r8hn6tmsrywzew
- bc1q0s2s6f6vqcyjqspqkxfv5c2heeelczwupnnj5xxfmqkn5su3ktxq4v0q6d
- bc1qgty7fdeldugdeclfh93v5782wtwm05s5u83km7w37gwxaky8jdgq2k4zrt
- bc1qhflc0n8uauc8zdyn00nx09nnnjpzd7cy9s0tsgkx6ufee2e6usuq809pfz
- bc1qx3verazru3u7mhzc6smc67q5gqdtg7hmprxar3hdza7jzzz2stgs36heq0
- bc1qtz8k08ntjx8fspqgmlasjxv6m7jrzt9a4altc506qlj9nk6mh68q6tgcw9
- bc1qzshepuxqwarg202g8sesj5m6cj7698r6s8vlf0zzwcmm9c6du4dqg9mzwm
- bc1q339e9d07mk93mgfsfvgw7av4myg9snp24cxy9zqldfhd5j6ku54qkd5whg
- bc1qv93fe8fm6369hm5gv4w980zsc0x2ccznjympp7v5h657uxt6n4xqqu2h53
- bc1q4fymywekv844wnqqp7xckve2cwj38qq2k2efquaus60ce5la8gms72np99
- bc1q2and0qed5hnvu0ugxstw7n86myqa9kdufh2f3xhnlqmncyvczslqrt493f
- bc1qxc5vdf8qglr8pmaqc9vwqnsxtppamvfe9vsm6hsf77jpe3x3edwq2pfqym
- bc1q2p8l5wa7v5w4zveyzfj8vx4l887pqs2ufmg244kjmpkrdepaeccqva3vc9
- bc1qlxe7q9x60fm9sj7y9xzd84gw3cqdtnanlgz7cyzuxuud7vhpa3qs28r8xl
- bc1q3469hyfs3rlxujjlcxz82p6t9jga0fkct7pjz0zty5azzlhls54ss3fe8f
- bc1qfcfwh94pzzhk9peadhrsqq9dtcuzc37e73q3utry96uxwa4m4svqrhu6ze
- bc1qpp572y3nwpcql8rk53pp3w2gywhwehf4edkdx2
- bc1qh8e856mvs8r0whu3decyk2vu8dt9uzvuwwzfw650d4zqml4n6hyq9gf0ag
- bc1qrf0tudk37nse8whg5zqueec5lv2pkyjaetucxkrpyruyrkfnynrsj0g4py
- bc1q9tfyy05jdgns7309l35l84eat00eud04jyu5ceujapva59nxaf4s35pt75
- bc1q0d8dtqqlzccvk7qxqrvpxktyezrp0s8f5fl0s3
- bc1qgv64ycjlcvt89p6cu30m5shsmhngpjldcx0ckj
- bc1qcmf704xn4jqe5znmsfss5dkhxvwlthn24dh8jkz385wpywd4lf5q7jwjry
- bc1qqu90ljh7978q0j2xrjqyu8zsmzda3graen7myf
- bc1qt42vy05z3fxt3wynwpjkuzneag4rq6yd4vfz7u8cuxhrgm426z0qexmnjm
- bc1q0cu5s808f7qqt5mrjvj4y32jgnx6xfwz5qnl98r5nh4wef6876mqc660ft
- bc1q9kaswsutz276ply8dmuwacu0f9hc3dzexsgyhz
- bc1qeesfaeg22lc3h7jucdchxpmnleeqjfl0t3gm7z5fgmxy7xhsp2jqlqj30x
- bc1q5x43skfs9adc95y6w4tmxt0p8at4stvh9xfew6qdk5785xhrgp2q5ap6en
- bc1qawt8u8yj5wmv6g4gqylad7cgvt4320sg37ygk6
- bc1qmvrklqznxw29z536jr92azf3jtdjv8reszudpgh3j9u84e80d3aqj29pvd
- bc1qqx0767mfwfykf7gh6zzdg77lu3cprtltxasstake56zmjklsvglqlcsnva
- bc1q2wcaannsqucfrxnxs09wdjh4np5q8e43cpghtmu3w88g3gla88kqvreyvu
- bc1ql90kku3jfjeu9p3t5azl0wk8dnhgypctv06jgqjgrlw0ufuzjllss302dk
- bc1qhdu6ds3unm6klf9uvevtlzz4re7nlzs3zvt4kmgep2lfu6n9apmsejcp3c
- bc1q4v86w4xrle0sxd6rkt32fmnk3rj5030y84pw0xqgsg5pwr752vxsw6jx7y
- bc1qml0syausuckjls9z9ceent0pj9xur5vvk9ak75
- bc1qdkjug94mmmete45m2ptlmdqw6n6l403nn865r2
- bc1q8jjkyg7qgnq2k2ekzwfj2sul6hxw38903sn7je
- bc1qa2z9k0w993n82c3vj0rxa674h2vx4y6nayk34u
- bc1qngttvu0rz9cuqpaef9nytyjpp2dtay3fgzxv4f
- bc1qdr3mx4l39snxuhhax4jg5rrm9wckfptt3x27hy9je4gxag0aa4jqv5anj6
- bc1qka9cwt7tpfanp7u52vd5gdr22pu82p8he6z5ptk8wl6qmuxgn49qh9m77f
- bc1qfhxwy9qwzmmtc4ljud6q5xq9un3hyczs98wzzg
- bc1qxke9c5mut7jwknsrwe9c9np2c5jxrp29pw9r53
- bc1q5xk0542lc7yn73qtrm5rf9e54r94l3dh677f2netxna7utgj20sq623yvk
- bc1qyteejytqrug05du3q3hd80zy6dvtjk74ufl9dy
- bc1qh94mej6regcsqqh9l7zuhlmwuug8j8m2j2csjg
- bc1qjsw5909kd3vv0423mdmqwhn2gn45j40trq8lwgyuzxawnfn52xsqaxdvgs
- bc1qhteqxqua3zlqypgu8kmg7g3w7at0znjgwps9h37hp6fz704zhztqz33gya
- bc1qrn0wt6lyrqv2pzs7lz4ydu64hweawdq977u9j96fu2d40yd4sawsqj7ueq
