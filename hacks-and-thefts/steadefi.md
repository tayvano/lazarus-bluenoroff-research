# Steadefi

Date:: August 7th, 2023

Amount Stolen:: $1,140,000

Tags:: "Inside Job"

---


## Details

Steadefi, a DeFi service built on Avalanche and Arbitrum, faced a $1.14M hack. The deployer's account was compromised.

"The attack vector is that our protocol deployer wallet -- which is also the owner of all vaults in the protocol -- has been compromised."

"The exploiter had transferred ownership of all the vaults (lending and strategy) to a wallet they control, and went on to take various owner-only actions such as allowing any wallet to be able to borrow any available funds from the lending vaults."

"Currently, all available lending capacity has been drained by the exploiter on both Arbitrum and Avalanche, assets swapped to ETH and bridged to Ethereum."

"The exploiter has also paused the farms contract, which means that if you (and the majority of everyone is) has your svTokens or ibTokens deposited in the farms, you will not be able to withdraw them as well. However, the exploiter is also unable to withdraw them."

An Onchain message was sent to the exploiter's wallet address for negotiation: https://etherscan.io/tx/0xdfc31c31e07f9007a15680e9c98a4d523cc440d4349515cebf22196086c889d4

> Steadefi would like to discuss a bounty with any parties who were involved in the recent Steadefi exploit. We are offering a 10% bounty of any funds stolen, which are yours to keep if you return the remaining 90%.

> You will have no risk of us pursuing this further, no risk of law enforcement issues, etc. If you choose not to partake in the voluntary return and complete the process by 10th August at 0800 UTC, we will expand the bounty to the public, and offer the full 10% to the person who is able to identify you in a way that leads to your conviction in the courts. We will pursue you from all angles with the full extent of the law.


### From Page 540 of [The 2023 UN Report](https://documents.un.org/doc/undoc/gen/n24/032/68/pdf/n2403268.pdf?token=Lnb4xBoncpFwgtMIpl&fe=true)

- The attacker(s) took control of the private keys of the hot wallet that had ownership of the contracts.

- Prior to the attack, an employee’s Metamask wallet seed phrase was copied, providing access to the employee’s personal wallets as well as the Steadefi hot wallet. The attacker(s) then approved an attacker-controlled wallet (0x9cf71f2ff126b9743319b60d2d873f0e508810dc) to be an approved borrower of the lending vaults, and “borrowed” all available assets from the lending vault to the attacker(s)’ wallet.

- The attacker(s) obtained access by reaching out on Telegram to a Steadefi employee in midJune 2023, pretending to be from “@manuel_trojovskky” (“Head of Crypto Investments & Research”) of the Spirit Blockchain Group, a cryptocurrency fund looking for projects to invest in (note: as of mid-January 2024, the telegram user’s name had been changed to “ceo_shima,” “Shima Capital Founder,” and photo had been changed) (see Figure 9).

- After establishing contact, the “fund manager” sent a malicious file that purported to be a presentation about the investment fund (see Figure 10). The file may have been a keylogger. A few days after the exploit, the attacker(s) deleted the Telegram conversation messages.

- The attacker(s) converted the stolen funds to Ether (ETH), bridged the ETH to the Ethereum mainnet, moved the ETH to another wallet (0xe10d4a5bd440775226c7e1858f573e379d0aca36), and eventually moved the funds to the Tornado Cash mixer.

- This attack is likely part of a broader Lazarus Group campaign of spearphishing on Telegram, targeting the cryptocurrency industry (see figure 11 and see para. 188).


## Onchain

- 0x9cf71f2ff126b9743319b60d2d873f0e508810dc Exploiter 1 

- 0xe10d4a5bd440775226c7e1858f573e379d0aca36 Exploiter 2 

- 0xc884cF2fB3420420ED1f3578EAECBDe53468f32E Tornado Cash Output 

- 0x4E75c46c299ddC74BAc808a34A778c863BB59A4E Tornado Cash Output 

- 0x9F8941cD7229Aa3047F05a7eE25c7ce13cBB8c41 Tornado Cash Output 



## Laundering

6 Deposits of 100 ETH were into Tornado were made from 0xe10d4a5bd440775226c7e1858f573e379d0aca36:

- 2023-08-12 08:27 100 ETH

- 2023-08-13 01:50 100 ETH

- 2023-08-14 08:38 100 ETH

- 2023-08-14 08:39 100 ETH

- 2023-08-23 15:02 100 ETH

- 2023-08-23 15:03 100 ETH


Additionally, 2 x 10 ETH, 4 x 1 ETH, and 3 x 0.1 ETH were made:

- 2023-08-29 02:40 10 ETH

- 2023-08-29 02:40 10 ETH

- 2023-08-29 02:42 1 ETH

- 2023-08-29 02:42 1 ETH

- 2023-08-29 02:42 1 ETH

- 2023-08-29 02:43 1 ETH

- 2023-08-29 02:44 0.1 ETH

- 2023-08-29 02:44 0.1 ETH

- 2023-08-29 02:45 0.1 ETH

## Outputs

The most likely outputs for these deposits are:

- [2023-08-13 01:35 -> 0xc884cF2fB3420420ED1f3578EAECBDe53468f32E](https://etherscan.io/tx/0x499dae0411931bdb396a704894ac824f434e7b4c6f8828a8872db151a0fa7dd8)

- [2023-08-14 01:02 -> 0x4E75c46c299ddC74BAc808a34A778c863BB59A4E](https://etherscan.io/tx/0x6c7c233bd39ddfd920e0b04ac23a935c19be332a46e0d82cf75f43eb4ac209a2)

- [2023-08-16 015:26 -> 0xc884cF2fB3420420ED1f3578EAECBDe53468f32E](https://etherscan.io/tx/0xb589962b62c59ed2e8c5977ba614ce94bfc9d107015ad67a1e9391122a03e849)

- [2023-08-17 23:36 -> 0xc884cF2fB3420420ED1f3578EAECBDe53468f32E](https://etherscan.io/tx/0xf23aa066bbaaaec2cd34b850791314d6a070148e1fb4440cad1d5a8ceb4e811b)

- [2023-08-24 05:30 -> 0xc884cF2fB3420420ED1f3578EAECBDe53468f32E](https://etherscan.io/tx/0xa23628410e99c908ebd3839e7d928f72b7a896c80714f3e1e1321f057f573a2c)

- [2023-08-24 06:02 -> 0x9F8941cD7229Aa3047F05a7eE25c7ce13cBB8c41](https://etherscan.io/tx/0xbf61cd7e50303f3602220e28298d6f98b211073d42d8245dd3c20e910d3be191)

These withdrawals were co-mingled with the Coinshift theft from August 16, 2023 and were subsequently laundered through previously identified deposit addresses at P2P marketplaces.


## URLs

- https://rekt.news/steadefi-rekt/

- https://twitter.com/steadefi/status/1688638572608552960

- https://twitter.com/steadefi/status/1688619454178144264

- https://twitter.com/h2jazi/status/1661528861211860993

- Page 540 of [The 2023 UN Report](https://documents.un.org/doc/undoc/gen/n24/032/68/pdf/n2403268.pdf?token=Lnb4xBoncpFwgtMIpl&fe=true)

![](../images/steadefi01.png)

![](../images/steadefi02.png)
