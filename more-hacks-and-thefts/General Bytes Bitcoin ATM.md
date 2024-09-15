# General Bytes Bitcoin ATM Platform

Date:: March 17th, 2023

Amount Stolen:: $1.8M

Compromised via 0-day to take over individual ATM machines 

General Bytes, a maker of crypto ATM machines, that got so thoroughly hacked that they are now shutting down their cloud service offering. Poolz got hit with a now rare integer overflow exploit while ParaSpace narrowly avoided a $5M hack if not for attacker messing up transaction gas fees allowing BlockSec to rescue funds at risk!

Leading Bitcoin ATM maker General Bytes disclosed that hackers stole cryptocurrency from the company and its customers using a zero-day vulnerability in its BATM management platform. The hacker exploited a zero-day vulnerability tracked as BATM-4780 to remotely uploaded a Java application via ATM's master service interface and run it with 'batm' user privileges.

Approx. $1.6M was taken in BTC ($1.5M) and ETH ($39k).

The attacker was able to upload his own java application remotely via the master service  interface used by terminals to upload videos and run it using batm user privileges. This resulted in:

- Ability to access the database.

- Ability to read and decrypt API keys used to access funds in hot wallets and exchanges.

- Send funds from hot wallets.

- Download user names, their password hashes and turn off 2FA.

- Ability to access terminal event logs and scan for any instance where customers scanned private key at the ATM. Older versions of ATM software were logging this information.

As a result, GENERAL BYTES is shuttering it’s Cloud service. It is theoretically (and practically) impossible to secure a system granting access to multiple operators at the same time where some of them are bad actors. You’ll need to install your own Standalone server. GB support will provide you with help you to migrate your data from the GB Cloud to your own Standalone server.

Please keep your CAS behind a firewall and VPN. Terminals should also connect to CAS via VPN. With VPN/Firewall attackers from open internet cannot access your server and exploit it. If your server was breached please reinstall the whole server including operation system.

Additionally consider your all user’s passwords, and API keys to exchanges and hot wallets to be compromised. Please invalidate them and generate new keys & password.

The largest manufacturer of Bitcoin ATMs, General Bytes, disclosed that attackers had stolen more than $1.6 million by exploiting a vulnerability in their software. The company released a statement on March 18 disclosing the breach, and urging operators of their ATMs to immediately upgrade their software to patch the devices.

In addition to standalone servers, General Bytes' cloud service was impacted, and the company announced that it would be permanently shuttering it. "It is theoretically (and practically) impossible to secure a system granting access to multiple operators at the same time where some of them are bad actors," wrote the company in their statement explaining the decision, apparently unaware that this is something software companies find themselves doing all the time.

This exploit was the second breach suffered by General Bytes this year, after hackers exploited a vulnerability in August 2022 that allowed them to steal customer funds. It's unknown how much was stolen in that attack. The company also patched multiple hardware and software issues in their ATMs in September 2021, after Kraken Security Labs discovered issues including poor security practices that would allow attackers to "walk up to an ATM and compromise it".

### On-Chain
- IP Address:: 123.204.4.202
- IP Address:: 172.104.237.25
- bc1qfa8pryacrjuzp9287zc2ufz5n0hdthff0av440 BTC
- 0xAE0aC391b8361B5Fc1aF657703779886a7898497 ETH BIZZ EURS FTO GQ HATCH HT JOB LMY MKR NXT PAXG REP SHIB USDC USDS USDT ZPAE
- 0x3d1451bF188511ea3e1CFdf45288fD53B16FE17E ETH BAT
- 0x7a0e7d41658f409c11288e0a2988406f2186a474 ETH
- 0xD5173d215551538cebE79C4e40A4C54Fb751DD83 ETH ANT BCH BTBS
- 0x8A9344be2BA8DeAA2862EAb0Aab20C7cC36c432a ETC
- 0x7A0E7D41658F409C11288E0a2988406f2186A474 ADA AQUA BTX BUSD DAI
- 426FQDKF9rbHZLbNgisRKU2m2CVfnoNpFL7ZsAoDQBHP1eRDUKaj64zDtnFychJqSg1W6eskoFqdkG4gX8BSvWvkQr8oxVc XMR
- dgb1qgea3hzw62zl6req06k708swtv5xc53sdp85jzn DGB
- DN1bKoV7BbuYBeysnYNT8EFj8BGTSeyLCc Doge
- erd1w7n54rlzrxe6jl8xpmh0de4g9jhc028zeppsjdme9g45gsnhw53s4vhgsg EGLD
- grs1qhckdwm8dqt8pfdu2d6e649qs5jrqn6sslzlyhw Groestlcoin $GRS
- ltc1qvd5usunrpgsynyeey9n46xucy7emk62ycljl0t LTC
- nano_1rrqx4esqbfuci7whzkzms7u4kib8ojcnkaokceh9fbr79sa4a36pmqgnxd4 NANO
- rDkoXVLChaDvc8SHFoTNZEDzcbtFNwF977 XRP
- TDjFvfcysNGaxnX7pzpvC6xfSmCC5u8qgr TRX USDTTRON
- via1quynq6wweqz0pk9wygv82qg83tk5zu47yqweht5 Viacoin
- Xi4GstuqKFTRo3WB6gFpPnB6jiWtLSHJDj DASH

### Links
> zachxbt, [3/18/23 6:38 PM] I missed this one ~56 BTC sitting here smaller amounts in other addresses bc1qfa8pryacrjuzp9287zc2ufz5n0hdthff0av440
https://blog.kraken.com/post/11263/kraken-security-labs-identifies-vulnerabilities-in-commonly-used-bitcoin-atm/
https://generalbytes.atlassian.net/l/cp/rVRVe1x9
https://generalbytes.atlassian.net/wiki/spaces/ESD/pages/2885222430/Security+Incident+March+17-18th+2023
https://twitter.com/generalbytes/status/1637192687160897537
https://bleepingcomputer.com/news/security/general-bytes-bitcoin-atms-hacked-using-zero-day-15m-stolen/
https://bleepingcomputer.com/news/security/hackers-steal-crypto-from-bitcoin-atms-by-exploiting-zero-day-bug/
https://web3rekt.com/hacksandscams/general-bytes-1511
