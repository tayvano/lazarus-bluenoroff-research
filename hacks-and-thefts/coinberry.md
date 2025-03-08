# Coinberry

Date:: August 24th, 2020

Amount Stolen: $200,000

Tags:: 🔑

---

## Details
  
> "On August 24th, 2020, "there were no withdrawals processed from Coinberry's hot wallet for about 17 hours." It "[h]asn't been publicly reported yet. 8.33 BTC stolen from Coinberry's hot wallet & sent to 1KcTk7kJMjYaCV3FXo5bzpjaZs2aK18ntz. I guess they can't say they've never been hacked anymore."

- [Source](https://quadrigainitiative.com/casestudy/nothinghappenedatcoinberry.php)

> "So another Canadian exchange appears to have been hacked a couple months ago. Hasn't been publicly reported yet. 8.33 BTC stolen from Coinberry's hot wallet & sent to 1KcTk7kJMjYaCV3FXo5bzpjaZs2aK18ntz. I guess they can't say they've never been hacked anymore #coinberry #quadriga"

– [CipherBlade, Oct 29, 2020](https://twitter.com/cipher_blade/status/1321862599433089025)





## Onchain

- 0xA06957c9C8871ff248326A1DA552213AB26A11AE - Primary Theft
- 1KcTk7kJMjYaCV3FXo5bzpjaZs2aK18ntz - Primary Theft


### BTC

- bc1qffjuzkld2jp2hf5apg9trz3ucpqt4rzj5rvvwv
- 37iW4CUhBXwUkoxNDgG6Ta4LdQmibb4KqS
- 38AhhMN9Sg9hnKT4gps8hrJPMyfgMY3nZ5
- 1GcHyFLYSMvr4XSySYdZUWB2LLGvu4QjVr
- 1DTjz8QWughcPekZaFdTdrrNxp9TEkZFWN - Attributed Lazarus Group
- 15K6ZmcnkqEXJpVpfqnk18fYGxRbDXAZr4 - Receives from multiple known DPRK victims
- Laundry @ 0xbc8d089824461048a06d300dff88bb7357d88b3b (Connects Coinberry, Coinmetro, Fetch.ai, Unibright, LEAD, Nexus Mutual, EasyFi)


### 0x94cf84daa641b499cf518ad49f8463fd39f4e579
- 0xa06957c9c8871ff248326a1da552213ab26a11ae receives 143 ETH (~$60k) from Coinberry on Aug 24, 2020
- 0xa06957c9c8871ff248326a1da552213ab26a11ae sends ~$60k to 0x94cf84daa641b499cf518ad49f8463fd39f4e579 on Aug 24, 2020
- 0x94cf84daa641b499cf518ad49f8463fd39f4e579 sends ~$60k to 0xbfc560a48619e2ff496adcd76f5974a5d4236f6b on Aug 24, 2020
- 0xbfc560a48619e2ff496adcd76f5974a5d4236f6b sends ~$60k to 0x94cf84daa641b499cf518ad49f8463fd39f4e579 on Aug 31, 2020
- 0x94cf84daa641b499cf518ad49f8463fd39f4e579 sends ~$663k to 0x99739fa525c0a98384430235d278fd08938997f9 on Aug 31, 2020


### 38AhhMN9Sg9hnKT4gps8hrJPMyfgMY3nZ5
- 0xe1cfc33ed7efc7e432a2214276fff6b71f09d493 via Ren Bridge
    - txn: e6fc336da02fa2de878bc90f466407bee6fc186df66e636b1adb0da4f1f81cde
    - txn: 0xa23f39446a7d7378755a06f460b5cd456feef4ca8e1c319e4b46a333277f2e97
- 0xe1c receives 0x990924d51c6ea6e212cce6e811b380ffd44ac350 (Coinmetro + L2 Theft)
- 0xe1c also sends to September 2023 Dust Collector 0x99739fa525c0a98384430235d278fd08938997f9
- 0xe1c also sends $5.8m to 0x7026b25422821473f7856ec03b0a3d58fee10100 which sends to 0x31499e03303dd75851a1738e88972cd998337403 (direct and via a back-and-forth Ren Bridge) which interacts with EasyFi exploiter 0x83a2eb63b6cc296529468afa85dbde4a469d8b37



### Laundry

Funds from thefts such as CoinMetro, CoinBerry, Unibright, and individuals were transferred through intermediary wallets before consolidating in `0x0864b5ef4d8086cd0062306f39adea5da5bd2603` in early January 2021.

3000 ETH was deposited to Tornado Cash by `0x0864b5ef4d8086cd0062306f39adea5da5bd2603` on January 11, 2021 02:54–09:14 UTC.

After 1814.49 ETH was transferred from `0x0864b5ef4d8086cd0062306f39adea5da5bd2603` to `0x1031ffaf5d00c6bc1ee0978eb7ec196b1d164129` and 17 X 100 ETH was deposited to Tornado Cash on January 11,2021.

An additional 112.1 ETH was deposited to Tornado cash by `0x1031ffaf5d00c6bc1ee0978eb7ec196b1d164129` from January 14–16, 2021.

45 X 100 ETH was withdrawn from Tornado Cash to `0x05492cbc8fb228103744ecca0df62473b2858810` beginning January 11, 2021 14:35 UTC thru January 14, 2021 23:52 UTC.

All Tornado Cash withdrawals for the month of January 2021 were reviewed and no additional withdrawals were found which shared similar characteristics. Additional comfort is gained with the demix as the Tornado withdrawal destination address connects back with the original theft address.

![TRM forensics graph](https://zachxbt.mirror.xyz/_next/image?url=https%3A%2F%2Fimages.mirror-media.xyz%2Fpublication-images%2FmDZpreD7D-Brv2SeNgSKi.png&w=3840&q=75)

Through a series of transactions, the funds sitting in `0x05492cbc8fb228103744ecca0df62473b2858810` were transferred through intermediary addresses and consolidated with funds from other Lazarus Group thefts before USDT was deposited to the P2P marketplace Paxful via deposit addresses `0x246569f8b420c8d850c475c53d0d59973b3f08fc` and `0x593dc5e1ad81667bbfc90739dd2c09c926920e3b` beginning in July 2022. 

In April 2023 they began using Noones deposit address `0x2e1155cf5374cba058a04fd03ebd0ba19afe580d`. They continue slowly transferring USDT in batches until November 2023.

Additionally, in 2021 multiple transfers were made from the 0x9973 address to [Wu Huihui](https://sanctionssearch.ofac.treas.gov/Details.aspx?id=42496), a China-based OTC trader. In April 2023, an [indictment against Wu](https://www.justice.gov/opa/pr/north-korean-foreign-trade-bank-representative-charged-crypto-laundering-conspiracies) was unsealed alleging that he facilitated payments for DPRK and he was added to the OFAC SDN list.

- Source: https://zachxbt.mirror.xyz/B0-UJtxN41cJhpPtKv0v2LZ8u-0PwZ4ecMPEdX4l8vE#:~:text=CoinBerry%20Incident%20Summary


## URLs

- https://financialpost.com/fp-finance/cryptocurrency/software-glitch-allowed-users-to-acquire-3-million-in-bitcoin-without-paying-coinberry-alleges-in-lawsuit
- https://coindesk.com/business/2022/09/08/canadian-crypto-exchange-coinberry-files-lawsuit-against-50-users-after-losing-120-btc/
- https://biz.crast.net/coinberry-loses-3m-due-to-software-glitch-files-suit-for-recovery/
- https://news.bitcoin.com/canadian-crypto-exchange-sues-users-for-return-of-bitcoin-misappropriated-during-software-glitch/
- https://protos.com/glitch-sees-users-pinch-3m-in-bitcoin-from-crypto-exchange-coinberry__trashed/
- https://techstory.in/coinberry-sued-its-users-for-stealing-bitcoins/
- https://crypto.news/coinberry-crypto-exchange-files-lawsuit-after-losing-3-million-in-software-glitch/
- https://cryptopotato.com/coinberrys-software-blunder-costs-3m-in-bitcoin-report/
- https://quadrigainitiative.com/casestudy/nothinghappenedatcoinberry.php
- https://zachxbt.mirror.xyz/B0-UJtxN41cJhpPtKv0v2LZ8u-0PwZ4ecMPEdX4l8vE#:~:text=CoinBerry%20Incident%20Summary