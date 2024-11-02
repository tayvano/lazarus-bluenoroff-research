# Swamp

Amount Stolen: $490,000

Date:: May 22, 2024

---

Network: BTC, ETH

Swamps protocol hired an external developer who manipulated with protocol contracts leading to unauthorized access and withdrawal of locked funds for around $490,000


https://swamps-explorer.tc.l2aas.com/tx/0x759eca9ce4017b185ff6d30a2656861aebd13fd413811c536f9c3202a253649e


0x759eca9ce4017b185ff6d30a2656861aebd13fd413811c536f9c3202a253649e

Addresses to be blocklisted
bc1qjcp5hmxj2h3prgldz00n9zutfuusdqdz8gudux
0x7273a4cAEd4E3CccE1354B47De03772f20dDd243

Addresses which were used to pay salary
0xfb74172Ee18f16f0517b204A6da44B515BA4e513
0x862f6C9A00BB344a710601D8033FF06D6166833C






# 🚨 Swamps Security Incident Detailed Report 🚨

https://twitter.com/Swamps_L2/status/1793662825178538058

Yesterday, a significant security breach was executed by a former developer, leading to unauthorized access and transactions within our network. We are committed to full transparency in our community and will detail each step of the exploit:

Initial Proxy Manipulation (May-22-2024 03:36:13 AM +2 UTC): The exploiter initiated the attack by creating a new Locker contract to gain ownership rights over it.

Specific Action: As the owner of the proxy, the exploiter created a new contract, giving us ownership of the contract but not the proxy itself. We believed we had full control as it was also confirmed by another developer, who, in reality, was colluding with the exploiter in this scheme.

Evidence of Breach: https://swamps-explorer.tc.l2aas.com/tx/0x21c3ddeae3bfa436a9731d689fed3cce7761fc22b595ced579e46759d012f99c

Contract Swap Fraud (May-22-2024 03:45:43 AM +2 UTC): Stealthily switched the implementation of the proxy to the malicious contract, crafted to siphon funds.

Contract Change Details: https://swamps-explorer.tc.l2aas.com/tx/0x543f36c7c1512e4bf3194b2554e3f2d3e92d5744c1d6d43267a9800a58e1b465

Introduction of Malicious Withdrawal Function (May-22-2024 03:47:53 AM +2 UTC): The exploiter Installed a function, called "Xxx" in the new contract to unilaterally transfer all contained funds on the proxy.

Function Execution: The function was called to withdraw the entirety of the locked funds to a wallet controlled by the exploiter.

Unauthorized Withdrawal: https://swamps-explorer.tc.l2aas.com/tx/0x759eca9ce4017b185ff6d30a2656861aebd13fd413811c536f9c3202a253649e

Massive Token Transfers:

First Major Transfer (May-22-2024 03:51:29 AM +2 UTC): 
Diverted 173,871,089 GSWP to an external wallet, initiating the large-scale theft.
https://swamps-explorer.tc.l2aas.com/tx/0xe6d00d7876c2e71a62f4168a33d7e1d3b4f212383308d054aa206a1e5c9a2892

Second Major Transfer (May-22-2024 03:57:35 AM +2 UTC): 
Further transferred 100,000,000 GSWP, consolidating the stolen assets.
https://swamps-explorer.tc.l2aas.com/tx/0x1c43608b0394dcd45348d00d9890af365eae2c8719cf476ddea1f062e30a9a3b

Liquidating NakaChain and Uniswap Pools:

The exploiter bridged funds to NakaChain and Uniswap and then sold all tokens into pools.

On NakaChain (May-22-2024 04:16:18 AM +2 UTC):
Tx 1:
- Amount: 173,870,890.75789896 $GSWP
- Details: https://explorer.nakachain.xyz/tx/0x253996828c28d7a6016140ac728c0421baf86ec2b4462dfae00f98534787e5ae
Tx 2 (May-22-2024 04:17:20 AM +2 UTC):
- Amount: 99,999,791.37263154 $GSWP
- Details: https://explorer.nakachain.xyz/tx/0x5a77138157c2580023d6e32b714696f723636ca2bc350e24bfd8784c198b5d16

Then he bridged those funds to the Bitcoin network (May-22-2024 04:18:14 AM +2 UTC):
https://explorer.nakachain.xyz/tx/0x18c641f863057fabcaea5aebeb031941bd1fef21dde598fb6724813be417a9fe
Receiving transaction on Bitcoin Network: https://mempool.space/fr/tx/4166a3eaddb40fe69b911acc3bd2673646ba4850c0accc399849ef091292519b

On Uniswap:
Tx 1 (May-22-2024 04:26:35 AM +2 UTC):
- Amount: 29,999,998 $GSWP
- Details: https://etherscan.io/tx/0xa1099b537cdec6e7b2eb978c36a116da38bc7bbf9a15d083df656575a6a0eb44
His address (same used to exploit our pools and Locker contract): https://etherscan.io/token/0x15ecf5e2766d214db1bdb5e3d47a0e52c601e064?a=0x7273a4caed4e3ccce1354b47de03772f20ddd243

Exploitation of Liquidity Pools (May-22-2024 04:06:57 AM +2 UTC): Used non-disclosed, non-verified contracts to drain liquidity pools initialized on Swamps DEX.

Mechanism Used: Deployed a hidden smart contract to manipulate pool transactions, allowing unauthorized siphoning of funds.

Liquidity Exploitation example: https://swamps-explorer.tc.l2aas.com/tx/0x700baf5705e19ccfabb96ae81ae4aaca6579e888965761c669776c2e33d71830

Asset Bridging and Liquidation: Systematically moved the stolen assets across networks to his EVM address: 0x7273a4cAEd4E3CccE1354B47De03772f20dDd243

Bridge and Liquidation Strategy: Used cross-network bridges to transfer and subsequently liquidate the assets for Ethereum and Bitcoin, reducing traceability.

First Bridge Transaction (May-22-2024 04:08:17 AM +2 UTC): https://swamps-explorer.tc.l2aas.com/tx/0xe09ae9855f58ff1fed69d58315be5a3b5286020a1e0a187d882c170bded8c87c

We are actively working with cybersecurity experts and law enforcement to address this issue and recover the funds. New security measures are being implemented to strengthen our system and prevent such incidents in the future.

We appreciate your support and understanding as we navigate this challenge. Continuous updates will be provided to keep our community informed every step of the way. Your trust is our top priority, and we are dedicated to restoring and maintaining it.
