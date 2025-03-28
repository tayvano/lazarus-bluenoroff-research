# NiiFi / Nahmii

Date:: September 19th, 2024

Tags:: 🎙️ Contagious Interview

---


- 0xcc8d82f6ba952966e63001c7b320eef2ae729099 - Victim

- 0x852e5427c86a3b46dd25e5fe027bb15f53c4bcb8 - Victim NiiFI

- 0x042469a11d763b8a91f5322fa9b4bad7ee72a204 - Direct Theft

- 0x286bbb823874121e7a7d2cb92d8897ba20e4a933 - Laundry

- 0xb787a7bce056c65690fcc4682ba276bbbb323241 - Laundry, Scallop Hack

- 0x69d91e56ca80f2a4d7b808b59053ea5c5505ffe2 - Tapioca Hack


# Security Incident Update: NII Token Reissue and NIIFI Token Swap

https://medium.com/nahmii/security-incident-update-nii-token-reissue-and-niifi-token-swap-9e54b08bfe48

Following the security incident on 19th September 2024, the Nahmii team have now completed our internal audit. Today’s update will cover the root causes of the attack, impact assessment and next steps. **This update includes important information about the NII and NIIFI tokens**.
# How Did The Attack Happen?
The root cause of the attack was a compromised private key for the ‘nahmii Deployer’ [wallet](https://etherscan.io/address/0xf05179bac3d1fbef58a2fcd7ad0f769840027cc6). This wallet had previously been used to deploy a number of Nahmii-related contracts, including the now-decommissioned Nahmii 1.0 protocol in 2018 and the Nahmii (NII) and NiiFi (NIIFI) tokens.
We believe that the private key for this wallet was compromised in early August 2024, after the key was accessed and used as part of a manual deployment within Nahmii. The same wallet was also used to make a withdrawal from Nahmii 2.0 shortly before this deployment, which we believe to be unrelated to the attack. The attacker was able to gain control of the deployer wallet using this key. On 12th August 2024 the Onchain ETH balance of the wallet was transferred out in this [transaction](https://etherscan.io/tx/0xf7b4c8d572e0656336d66c498131835eb87f6808f7fc35ef9f4c734b3cab8dc4); this was the start of the attack.
Next, three ETH transfers were made into the compromised deployer wallet. We believe these funds were most likely from other compromised wallets, including from other wallets on the developer’s machine. The attacker then called the ‘[Disable Minting](https://etherscan.io/tx/0x775db5f1bd890a191680f3e33ee15bf42fe1afb097094ca2bdb45699a67cf0b6)’ function on the NII token contract, which was also under the control of the deployer address. Minting had already been permanently disabled for the NII token.
After moving ETH back to one of the three potentially compromised wallets that had earlier transferred into the deployer wallet address, no further transactions were made by the attacker for 37 days. This initial set of transactions was not detected by the Nahmii team. At this stage, only the initial wallet balance of approximately 2 ETH had been stolen.
# ‘RevenueTokenManager’ Contract Attack
The primary attack came on 19th September 2024. The attacker used the deployer wallet to withdraw 8 billion tokens from the NII token ‘RevenueTokenManager’ or ‘time-lock’ [contract](https://etherscan.io/address/0x4fa70e4143cc38dca0a2101e522d8c0d3f040128), which controls the release of NII tokens. This required eight transactions, releasing one billion NII tokens each time. The remaining 50 billion NII tokens in the time-lock contract are also under the control of the attacker, but these tokens are time-locked and will only release at a rate of 1 billion tokens per month.
Using a clean [wallet](https://etherscan.io/address/0x042469A11d763B8A91f5322Fa9b4baD7EE72a204) funded by ETH from other addresses that we believe to be compromised, the attacker then sold the 8 billion tokens across both Ethereum-based exchanges and NiiFi on Nahmii 3.0. This crashed the price of the NII token across all exchanges, including Gate.io. It is impossible to determine whether this attack was performed by the same individual or entity behind the previous wallet-draining transactions 37 days earlier.
# Nahmii 1.0 Attack
The attacker then used the deployer wallet to attack the ‘[Client Fund](https://etherscan.io/address/0xcc8d82f6ba952966e63001c7b320eef2ae729099)’ contract of our now-decommissioned Nahmii 1.0 protocol. A small amount of ETH and approximately 12 billion NII tokens were held by the Nahmii 1.0 Client Fund prior to the attack. First, the attacker called ‘Register Service’ on the ‘nahmii: Balance Tracker’ contract to add the deployer wallet as a service in this [transaction](https://etherscan.io/tx/0x026f247fb2f4fb07723bc628a88405787de07919bc8e1631e8465b18e2bd78c6).
Next, they called the ‘Set’ function on the same contract twice. The first transaction increased the amount of [ETH](https://etherscan.io/tx/0x371c09a619dbfe910a9cac24aed4526b8e473b0935329b283e6d64838bce78f0) that the attacker could withdraw from the Nahmii 1.0 Client Fund from 0 to 1.29788. These funds were then withdrawn from the Client Fund [here](https://etherscan.io/tx/0x8a27b3239d1635140e73d5afcf6b316ad10f31fb0eb34905a0b9286dae53d2de). A day later, the attacker repeated the ‘[Set](https://etherscan.io/tx/0x02bd0130cc13208288564c3c974215bc9604067202ecfac533aab795f72bd369)’ and ‘[Withdraw](https://etherscan.io/tx/0x11670f100747a3a694a9e07a4c4f694ad6e6bca2f75d846287949fd39a3c213c)’ transactions to transfer over 12 billion NII tokens to a different address.
The NII tokens taken from the Nahmii 1.0 Client Fund were subsequently deposited into Nahmii 2.0 and [sold](https://explorer.n2.nahmii.io/address/0xf05179bAc3D1fbEF58A2fcD7AD0F769840027cc6/transactions) using the Nahmii 2.0 version of NiiFi.
# Other Contracts
In addition to the NII token time-lock contract and Nahmii 1.0, the compromised deployer wallet is also linked to a number of product and token deployments. The attacker was able to take control of the Nahmii (NII) and NiiFi (NIIFI) token contracts through the deployer wallet, giving them the ability to rename the tokens. More information about the NII and NIIFI tokens is provided below.
Other deployments were also linked to the deployer wallet. We have regained control over these contracts.
# Impact Assessment
In keeping with industry best practices, we use multisignature (multisig) wallets for all accounts containing company funds. This policy was not followed for the deployer wallet, which was controlled by a single private key. When this key was compromised, the impact was far more severe than an equivalent single signature breach on a multisig wallet.
A key lesson from this attack is that all core company contracts, regardless of whether they contain funds or not, should use multisignature protections. While **Nahmii 2.0 and Nahmii 3.0 were unaffected by the breach**, we have increased security on both networks.
The most immediate impact of the attack was 20 billion NII tokens being released onto the market at once. A further 50 billion NII tokens are held in the time-lock contract, which is under the control of the attacker. Control of this time-lock contract has been lost; **therefore, we have no choice but to reissue the NII token**. We will take a snapshot of NII balances on Ethereum and Nahmii’s networks from immediately before the primary attack started, i.e. one block prior to the first compromised transaction on the RevenueTokenManager contract [here](https://etherscan.io/tx/0x66839601c0c00f62c8a1b9a4fb5fecd8538e0f7efb209a1bf06d355f74dfeb10).
We will use the following blocks for the NII token snapshot:
* Ethereum: 20780057
* Nahmii 2.0: 44510
* Nahmii 3.0: 12731
We will also work with Gate.io to arrange for the same token swap. More details about Gate.io balances will be provided at a later date.
The situation with the NiiFi (NIIFI) token is slightly different; the attacker has taken control of the NIIFI token contract but there is no equivalent ‘time-lock’ which will provide them with saleable tokens. As such, the attacker can only rename the token or change its symbol. Nevertheless, this is still an unacceptable risk for the product and token, so **we will offer a 1:1 swap for the NIIFI token **with a new token under our control.
Important note: we reserve the right to exclude any address from the NII token reissue or NIIFI token swap.
# Liquidity Providers and Traders
Liquidity providers in NII-based pools across all decentalised exchanges were affected by the attack. The attacker sold over 20 billion tokens, almost 30% of the unlocked supply, effectively draining all non-NII tokens from the NII-based liquidity pools. Arbitrage traders and opportunistic traders also tried to take advantage of the sudden price change, attempting to profit from the ongoing attack.
We will not be compensating liquidity providers for their losses as a result of the attack, nor will we recognise the artificially inflated NII balance of traders who bought tokens after the snapshot block.
# Attacker’s Funds
This incident was a failure of private key management, not Nahmii’s core protocols. Given that both Nahmii 2.0 and Nahmii 3.0 continued to function as intended, the pending withdrawals from the attacker’s address will be processed as normal.
We are investigating potential legal options to track and potentially reclaim the attacker’s funds.
# Summary
More information about the NII token reissue and NIIFI token swap will be provided in the coming days. Gate.io deposits for both tokens will remain suspended, as will trading of the NII token.
We appreciate that the events of the past week have been concerning for our community. During this period we have received many messages of encouragement, for which the team are extremely grateful. We will continue to work tirelessly to deliver on the potential of the Nahmii protocol and our products. Thank you again for your support.