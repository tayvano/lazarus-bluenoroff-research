# Bitmart Hack

Amount Stolen:: $240,000,000

Date:: December 4th, 2021

Tags:: Unknown

---



## Details

- SimpleSwap, ChangeNOW, NRBio, Tornado Cash, Wasabi

- Sat for 3 years before Wasabi

- No one demix'd the TC, likely due to lack of attribution and the fact these fucking imbicles didn't publish their addresses so they aren't tagged anywhere

- They were rekt for a couple weeks 😳

- Total BSC: 56,690 in 575 Txns - Dec 04–Dec 05

- Total ETH: 34,372 in 379 Txns - Dec 04–Dec 06

- Plus ETH: 1x100ETH + 6x10ETH - on Dec 19

- One article provides the IP address: 119.91.93.28 (Discovered in Dec 2021) and 38.102.175.100 (Discovered in Dec 2021)

- I'm not sure where they came from, take with a grain of salt tbh.

- https://hackenproof.com/programs/bitmart-post-incident-forensics-bounty-hunt




## Roman Storm Trial

- No additional details came out (lmfao, but seriously, they wouldn't even say how much they got fucking hacked for)

The AI summary of the court transcripts provide the following:

- BitMart experienced a hack on December 4 and 5, 2021, resulting in a significant amount of cryptocurrency theft. This was described as a "pretty sizeable hack".

- Joe Evans, representing BitMart, stated that an investigation, aided by crypto tracers and experts, identified some of the stolen assets as going to what they believed was Tornado Cash. (NOTE: dunno who investigated bc these addresses literally aren't tagged in Chain or TRM)

- On December 14, 2021, Joe Evans sent an email to hello@tornado.cash (which he believed was associated with Tornado Cash), attaching a letter and seeking information about the exploits incident at BitMart. The letter claimed that their investigation revealed assets were transferred to and remained at Tornado Cash, demanding that Tornado Cash "immediately take all possible action to ensure that the assets are frozen and returned to BitMart" and requested all associated information.

- The letter specifically identified 211 separate 100 ETH transactions and seven separate 10 ETH transactions, originating from a digital address ending in 7091 and going to a Tornado Cash-associated address ending in 6967, between December 4-5, 2021.

- Special Agent DeCapua's tracing analysis confirmed that criminal proceeds from the BitMart hack were transferred to Tornado Cash. This included 219 ETH deposits and 575 BNB deposits, totaling approximately $102.9 million, made by the "BitMart hacker" on December 4th and 5th, 2021.

- The BitMart hack contributed to the highest single-day volume Tornado Cash had ever seen on December 5, 2021, with 54% of the ETH volume on that day traced to the hack.

- Roman Storm's Google search history included a search for "BitMart hack" on December 4, 2021.

- Despite the communications and requests, Tornado Cash did not provide assistance to BitMart. (NOTE: They told them to hire Chainalysis and ping Infura+Etherscan for IPs. They didn't hire Chainalysis, clearly. They should've. Binance also proactively froze some funds which is partially why I am inclined to attribute this to DPRK.)

- While the sources extensively detail the hack's impact on Tornado Cash's volume and the efforts to trace the stolen funds, they refer to the perpetrator only as "the hacker" or "BitMart hacker", without disclosing any specific names or affiliations of the individuals or group responsible for the hack.







## Onchain


| Chain               | Receiving Address                          | First Active     | Deposit Dates          | Notes                                   | In (USD)     | Out (USD)    | To TC (ETH/BSC) | TC Depo Count |
| ------------------- | ------------------------------------------ | ---------------- | ---------------------- | --------------------------------------- | ------------ | ------------ | --------------- | ------------- |
| ETH                 | 0x39fb0dcd13945b835d47410ae0de7181d3edf270 | 2021-12-04 21:31 | 2021-12-04, 2021-12-05 | Direct from BitMart                     | $62,555,223  | $421,252     | 100             | 1             |
| VeChain             | 0x673B380f1667b2f9A216Fd1eBB6225Ee75cC7d55 | 2021-12-04 21:33 |                        | Direct from BitMart                     | $1,352,846   | $1,352,846   | -               | -             |
| THETA               | 0x8cbcc75678cd88e3d450941dcd3d27b560a6ecba | 2021-12-04 21:35 |                        | Direct from BitMart                     | $136,328     | $136,328     | -               | -             |
| TRX (2,100,000 TRX) | TL1NRNDe3babg3zZywe8PC1tTMta1mqkTX         | 2021-12-04 21:42 |                        | Direct from BitMart                     | $684,500     | $684,500     | -               | -             |
| BTC                 | 3Nsop3FW7jjjTKd6MkLc6qjyWuAm9XLU81         | 2021-12-04 21:44 | 2024-03-30             | Direct from BitMart, to Wasabi Mar 2024 | $50,688,977  | $59,344,735  | -               | -             |
| AVAX                | 0x59E55AC0cb34358B9511bbB3f3C1327BD40523E5 | 2021-12-04 21:45 |                        | Direct from BitMart, Dormant            | $37,957      | $37,957      | -               | -             |
| BNB                 | bnb15r4fzmhjv54ncf4f0cvmjvadjgwffd93gf56qv | 2021-12-04 21:46 |                        | Direct from BitMart                     | $173,316     | $173,900     | -               | -             |
| BSC (shitcoins)     | 0x25fb126b6c6b5c8ef732b86822fa0f0024e16c61 | 2021-12-04 21:47 | 2021-12-04, 2021-12-05 | Direct from BitMart                     | $1,038,230   | $17,943,934  | 31700           | 317           |
| ETH (shitcoins)     | 0x4bb7d80282f5e0616705d7f832acfc59f89f7091 | 2021-12-04 23:45 | 2021-12-04, 2021-12-05 | Direct from BitMart                     | $5,301,519   | $87,905,552  | 21170           | 218           |
| BSC (shitcoins)     | 0x13795c1622edc054778104ffc4cac34f77b8a620 | 2021-12-05 01:47 | 2021-12-05             | Direct from BitMart                     | $0           | $14,145,707  | 24990           | 258           |
| ETH                 | 0x132f8ceefe9ea00e1dbc06b32f625864ba21d66c | 2021-12-05 06:51 | 2021-12-05             | Direct from BitMart                     | $1,611,001   | $3,462,036   | 820             | 10            |
| TRX (475k USDT)     | TBTPmRe7Lpjka6Koxr2v7CrAocCNGZKsW5         | 2021-12-05 08:37 |                        | Direct from BitMart, to SimpleSwap      | $475,848     | $475,848     | -               | -             |
| ETH                 | 0xa9e4332448318da58cdd398286c0809684ed9bd4 | 2021-12-05 11:31 | 2021-12-05, 2021-12-06 | Direct from BitMart                     | $26,341,951  | $35,994,814  | 8602            | 88            |
| ETH                 | 0xaf631c6eebfc5ff3a267788bafa52a18670d577c | 2021-12-05 17:00 | 2021-12-06             | Direct from BitMart                     | $5,295,572   | $8,776,377   | 2105            | 26            |
| ETH                 | 0x8eafee3d0df538a1e04487a43239c1c73b50032d | 2021-12-06 04:37 | 2021-12-06             | Direct from BitMart                     | $1,436,213   | $2,143,197   | 525             | 12            |
| ETH (shitcoins)     | 0xc47a987521e2e646423ac92b1eb0b3cb2193625d | 2021-12-06 05:09 | 2021-12-06             | Direct from BitMart                     | $1,844,400   | $3,462,076   | 850             | 22            |
| ETH                 | 0xb4f8abad5d64f7132c74013569d55a6ac9bbaa1d | 2021-12-06 05:52 |                        | Direct from BitMart                     | $96,330      | $96,330      | -               | -             |
| ETH                 | 0xf082af2426ee0d626c75597649f8f8fe0b5fbeee | 2021-12-06 07:32 |                        | Gas/Sweeper                             | $37,500      | $37,500      | -               | -             |
| ETH                 | 0x402be63f5d8189f8027d429b8588df4f0aec9f53 | 2021-12-06 13:54 |                        | Gas/Sweeper                             | $163,200     | $163,200     | -               | -             |
| ETH                 | 0x6723736dd131c0baed60d712d8e569fe6e9509b0 | 2021-12-06 14:10 | 2021-12-06             | Direct from BitMart                     | $724,560     | $826,488     | 200             | 2             |
| TRX                 | TWupvrfs2oS3X4yk3xRqeApYM8XbhtuVoF         | 2021-12-07 15:36 |                        | Int, to SimpleSwap                      | -            | -            | -               | -             |
| ETH                 | 0x041afe8c155997de612d69f3ff0287ae58504246 | 2021-12-10 01:55 |                        | Gas/Sweeper                             | $22,000      | $22,000      | -               | -             |
| ETH                 | 0xe68a520f67c0225b7856bb9496dfc6b476217256 | 2021-12-10 02:39 | 2021-12-19             | Direct from BitMart                     | $257,482     | $642,885     | 160             | 7             |
| VeChain             | 0xbb3fd383d1c5540e52ef0a7bcb9433375793aeaf |                  |                        | Binance                                 |              |              |                 |               |
| VeChain             | 0x6f39fa0096b075becdb2c46c62976e92f03ca104 |                  |                        | NRNB/Binance                            |              |              |                 |               |
| TRX                 | TA6kBqs1sXuCS9cyNfs9k9gmoVc8doZxhD         |                  |                        | SimpleSwap/CHN                          |              |              |                 |               |
| TRX                 | TU2d7VinYqHRg2WqbT1BVyBRe26N5ZFZnU         |                  |                        | SimpleSwap/CHN                          |              |              |                 |               |
| TRX                 | TFGo3mFeK2b6tyL3nsARBQrXCLzBpZaJAa         |                  |                        | SimpleSwap/CHN                          |              |              |                 |               |
| TRX                 | TBfs47m9pwN8SGBaCCAV4CiMDhJZU2wdC9         |                  |                        | SimpleSwap/CHN                          |              |              |                 |               |
| TRX                 | THr92Qi9GgvYxCGbn8B2NKWZA1jKFnsFfh         |                  |                        | Unknown Depo                            |              |              |                 |               |
| TRX                 | TGScTPMkm3MDF8T3xpUzb7u3jXUV4qcBYm         |                  |                        | Binance Depo                            |              |              |                 |               |
|                     |                                            |                  |                        | **TOTAL**                               | $160,274,953 | $238,249,460 | 34,432 ETH      |               |
|                     |                                            |                  |                        |                                         |              |              | 56,690 BSC      |               |
|                     |                                            |                  |                        |                                         |              |              | 1049.79 BTC     |               |








## Tornado Cash

- A selection of ~2500 txns sent by the hackers: https://dune.com/queries/5552894/9040174

- Only the Tornado Deposit Raw Txns: https://dune.com/queries/5553763

- By Address: https://dune.com/queries/5553901/

- By Hour: https://dune.com/queries/5553636/9041331

- By Day: https://dune.com/queries/5553010/9040364


| Depositor                                  | Dates                  | Amt ETH  | Count ETH  | Amt BSC  | Count BSC  |
| ------------------------------------------ | ---------------------- | -------- | ---------- | -------- | ---------- |
| 0x25fb126b6c6b5c8ef732b86822fa0f0024e16c61 | 2021-12-04, 2021-12-05 | -        | -          | 31700    | 317        |
| 0x13795c1622edc054778104ffc4cac34f77b8a620 | 2021-12-05             | -        | -          | 24990    | 258        |
| 0x4bb7d80282f5e0616705d7f832acfc59f89f7091 | 2021-12-04, 2021-12-05 | 21170    | 218        | -        | -          |
| 0x39fb0dcd13945b835d47410ae0de7181d3edf270 | 2021-12-04, 2021-12-05 | 100      | 1          | -        | -          |
| 0xa9e4332448318da58cdd398286c0809684ed9bd4 | 2021-12-05, 2021-12-06 | 8602     | 88         | -        | -          |
| 0xaf631c6eebfc5ff3a267788bafa52a18670d577c | 2021-12-06             | 2105     | 26         | -        | -          |
| 0xc47a987521e2e646423ac92b1eb0b3cb2193625d | 2021-12-06             | 850      | 22         | -        | -          |
| 0x132f8ceefe9ea00e1dbc06b32f625864ba21d66c | 2021-12-05             | 820      | 10         | -        | -          |
| 0x8eafee3d0df538a1e04487a43239c1c73b50032d | 2021-12-06             | 525      | 12         | -        | -          |
| 0x6723736dd131c0baed60d712d8e569fe6e9509b0 | 2021-12-06             | 200      | 2          | -        | -          |
| 0xe68a520f67c0225b7856bb9496dfc6b476217256 | 2021-12-19             | 160      | 7          | -        | -          |


- Total BSC: 56,690 in 575 Txns - Dec 04–Dec 05

- Total ETH: 34,372 in 379 Txns - Dec 04–Dec 06

- Plus ETH: 1x100ETH + 6x10ETH - on Dec 19

