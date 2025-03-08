# BTC Changers

Date:: March 21, 2020 – April 14, 2021

Amount Stolen:: Unknown


## Details [🔗](https://blog.group-ib.com/btc_changer)

Lazarus BTC Changer - Back in action with JS sniffers redesigned to steal crypto

In July 2020, Sansec published an article about the attacks on US and European online shops with the use of JavaScript sniffers (JS-sniffers). The researchers attributed the “clientToken=” campaign to the North Korean APT called Lazarus (aka Dark Seoul Gang, HIDDEN COBRA, Guardians of Peace, APT38, APT-C-26, Labyrinth Chollima, Zinc, Bluenoroff, Stardust Chollima).

The Group-IB Threat Intelligence team looked deeper into these campaigns and identified another campaign involving the same infrastructure. The threat actor went back to the old habit of stealing crypto using a never-before-seen tool. Lazarus attacked online stores which accept cryptocurrency payments through crypto skimmers: JS-sniffers modified for the purpose of stealing crypto currency. Some victims, identified by Sansec, in fact, didn’t fell prey to the clientToken= campaign, but to a different, previously undocumented Lazarus campaign, codenamed BTC Changer by Group-IB researchers. Group-IB’s TI&A team identified BTC addresses used by Lazarus and have analyzed the transactions. Group-IB found additional evidence of Lazarus involvement in the campaigns.

Like all traditional JS-sniffers, Lazarus BTC Changer detects when users are on the checkout page of an infected website, but instead of collecting bank card details, it replaces the BTC or ETH address owned by the shop with an address used by the hackers. A snippet of such JavaScript code is shown in Figure 2 along with the BTC address used by the attackers (1MQC6C4FVX8RhmWESWsazEb5dyDBhxH9he) and the ETH address (0x460ab1c34e4388704c5e56e18D904Ed117D077CC).

The fake form (Figure 4) asks that the payment be made directly to the BTC address controlled by the hackers (1MQC6C4FVX8RhmWESWsazEb5dyDBhxH9he). Despite the fact that the form mentions one particular target (Realchems), the attackers used the same fake form in the samples injected into the source code of the other two target websites.

Group-IB analyzed the transactions associated with the BTC addresses controlled by Lazarus and discovered that the adversaries most likely used CoinPayments.net. An analysis of money transfers from the attackers’ BTC addresses, extracted from the Lazarus BTC Changer samples, to the address 35dnPpcXMGEoWE1gerDoC5xS92SYCQ61y6 revealed three transactions to BTC wallets allegedly owned by CoinPayments.net. CoinPayments.net is a payment gateway that allows users to conduct transactions involving Bitcoin, Ethereum, Litecoin, and other cryptocurrencies. As such, Lazarus may have used it to facilitate cryptocurrency exchanges and transfers to external cryptocurrency addresses. The website’s KYC (Know Your Customer) policy could theoretically help identify individuals behind these attacks.

At the time of withdrawing cryptocurrency from the extracted BTC addresses, the attackers transferred 0.89993859 BTC ($8,446.55 at the moment of the transaction and $52,611 as of April 9, 2021). The two main BTC addresses (1Gf8U7UQEJvMXW5k3jtgFATWUmQXVyHkJt and 1MQC6C4FVX8RhmWESWsazEb5dyDBhxH9he) used to steal funds received 43 transactions while the Lazarus BTC Changer campaign was active.

The address 1DjyE7WUCz9DLabw5EWAuJVpUzXfN4evta was not active during the Lazarus BTC Changer campaign because there were only one incoming and one outgoing transactions associated with this address on January 7, 2020, two months before the Lazarus BTC Changer campaign began. The ETH address received 29 incoming transactions, with a total profit of 4.384719 ETH, ($9,047 as of April 9, 2021). This ETH address had been active since July 11, 2019, however, and could have been used during other operations conducted by the hackers. It is therefore impossible to determine the transactions which resulted from the Lazarus BTC Changer campaign.


## URLs

- https://sansec.io/research/north-korea-magecart

- https://blog.group-ib.com/btc_changer


## Onchain

- 0x460ab1c34e4388704c5e56e18D904Ed117D077CC

- 1Gf8U7UQEJvMXW5k3jtgFATWUmQXVyHkJt

- 1MQC6C4FVX8RhmWESWsazEb5dyDBhxH9he

- 1DjyE7WUCz9DLabw5EWAuJVpUzXfN4evta


