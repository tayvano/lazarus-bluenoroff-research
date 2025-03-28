# Various 2023 Rug Pulls

Tags:: 🎙️ Contagious Interview?


---


## Onchain 

- 2023-Mar-02 ARBI Token Rug Pull - $100,000
- 2023-Apr-22 Fashion AI Rug Pull
- 2023-May-22 LunaFI - $50,000
- 2023-Sep-14 We Are Cult DAO - $200,000


- 0x0d8b378203791dd6960e0d77a99bbda68f83bb49   Fashion AI Rug Pull

- 0xd2a984e4f03e2a542804a97cd009a7ee0f028fa8 - RVLT Attacker
- 0xcbcb15856ad070925bc91ee82c59520c0c6b9be8 - RVLT Attacker Polygon
- 0x6cd36b9459dfef332479d50bec129932285a1656 - Cult DAO Attacker
- 0x0d31a41c93e483a69e10d067e353a9c489962f67 - Cult DAO Deployer (Compromised)
- 0x4c2da9c9612b0ebde13b5eb7675f1d5975c21045 - AstroBot Society Deployer (Compromised)


## CultDAO Details

https://wearecultdao.medium.com/0xblock-exploited-5da3d0bbc00e#:~:text=It%20is%20worth%20noting%20that,transferred%20to%20a%20secure%20address.

- Not a medium I ever wanted to write, but unfortunately due to a hack some of our third party developers suffered, their hackers were able to gain access to the Cult & RVLT Deployer.
- It is worth noting that $CULT as a token & Cult DAO as a protocol is 100% immutable, autonomous & with all ownership functions renounced and as such is **unaffected**.
- Similarly, TRG and its related contracts are safe, and ownership of the smart contracts has been transferred to a secure address.
- However, as many in the community know, RVLT has had a lot of tweaks made in its governance and so the governance contract remained owned by the Cult DAO deployer.
- The Cult DAO deployer wallet was created by 0xBlock originally in order to deploy the CULT DAO contracts, before being transferred to ourselves via secret key, it remained attached to 0xBlocks now exploited wallet, alongside other projects who and where they had deployed contracts for before.
- As you can see by the below screenshots, a variety of projects have suffered due to this, as the exploit was not one of Cult or our ecosystem but was rather an exploit of some developers we have used in the past and as such has affected Astra DAO, TokenMetrics & many others who have also used 0xBlocks services in the past.
- https://etherscan.io/address/0x6cd36b9459dfef332479d50bec129932285a1656
- ![](https://miro.medium.com/v2/resize:fit:1400/0*sWQ-xbcb9WVv6tBw)
- Unfortunately this includes some of our Modulus based builders, at present we believe just MODS (Modulus Domain Service).
- In order to best support the ecosystem we had set up an incubation hub where projects who contacted us could receive access to our connections, KOLs & of course developers if needed. Not everybody needed all of that help but those who did take up our help on the development side of course may have been affected.
- ![](https://miro.medium.com/v2/resize:fit:1400/1*NhlFY4RbJDf9fwUmHS0O6g.jpeg)
- For the most basic of explanations. This was a planned attack as they deployed a new staked RVLT contract 3 hours before they began withdrawing funds.
- https://polygonscan.com/tx/0x9bf7c3cc27aee5ff16b02db845f294e493cbc2ee168f0bdbaea3419e1acc85a0
- The hackers gained access to 0xBlocks wallet (we are awaiting explanation from them on how) which held many deployers but with it, the deployer wallet for CULT and RVLT. All of CULTs contracts were fully renounced, so the only damage they could do was to dump 1% of all the TRG letters. 5 of which had 0 liquidity already.
- Due to the governance contract for RVLT being upgradeable and owned by the CULT/RVLT deployer, the hacker was able to upgrade the RVLT staking contract & did so by upgrading the proxy to point to a new implementation, where they had added the “WithdrawAdmin” function, allowing them to withdraw all staked uRVLT which they then dumped into the liquidity extracting significant amounts of the Ethereum from the LP pool which was locked for 265 years.
- We will be publishing a further medium once we know the full details of how 0xBlock were exploited, and once we reach out to the hacker to see if we can recover funds stolen. In the meantime you can be assured that $CULT as a protocol and DAO cannot ever be edited or changed.
- We will strive to keep you as updated as possible.


## ArbiSwap Rug Pull
- https://arbiscan.io/tx/0x54ca307057b38110f60fce515ba35321fde82b876b4a2abf77368924903216e1
- ArbiSwap deployers minted 1 trillion ARBI before Rug Pull, and then converted ARBI into USDC, which caused a sharp drop in ARBI in the USDC/ARBI transaction pair. In the next block, the robot passed USDC to ARBI then traded ETH for spatial arbitrage, making a profit of 68.47 ETH. 
- ArbiSwap has transferred 84 ETH to the Ethereum mainnet and sent it to TornadoCash.
- 0x8a60f91178da2F9de3D7a825380B7CE03933724F - "ARBI Token Rug Pull" on Etherscan
- 0x6cd36b9459dfef332479d50bec129932285a1656 - receives from [ARBI Token Rug Pull](0x8a60f91178da2F9de3D7a825380B7CE03933724F) and [Cult DAO Deployer](0x0d31a41c93e483a69e10d067e353a9c489962f67). Sends to [LunaFi Hacker](0x0a0ed79f9fbbcc6b44a054d2608031818e391b3b)
- 0x86d49a933d1f6aa1218dfa91250733d9818e36fa
- https://coindesk.com/tech/2023/03/02/arbitrum-dex-arbiswap-rug-pulls-users-for-over-100k/



## LunaFi
- May 22nd, 2023
- The root cause is pretty simple: there is no time lock for the user 'staking' amount(balance).  There are multiple other issues in the contract. Highly encourage the project owner to do an audit before put it Onchain.
- LunaFI, a Polygon-based project, was exploited resulting in the loss of 1,500,000 $LFI tokens worth around 36,362 $USD.
- LunaFi is a betting platform running on Polygon. LunaFI's vLFI contract rewarding system was exploited. The attacker found an issue with the Claim Rewards function that allowed them to repeatedly claim LFI tokens. As a result of this exploit, approximately 1,500,000 $LFI tokens were stolen which is equivalent to around 36,362 $USD at current market value. After stealing these tokens from multiple users' wallets on the Polygon network using this method they swapped them for around 20 $ETH and transferred it to their initial address.
- 0x11576cb3d8d6328cf319e85b10e09a228e84a8de - Attacker
- 0x43623b96936e854f8d85f893011f22ac91e58164 - Malicious Contract
- 0x9ada20b835aa178813a8c174f1f93b1dc1bfa775 - LunaFi Hacker on Arkham
- 0x232B1f770E7637f2656ce08Ed42eC6fB4c84590E - LunaFi Hacker on Arkham, sends to OKX Dex Hacker
- 0x0a0ed79f9FBbCc6b44A054d2608031818e391B3b
- Hacker address: 0x11576cB3D8d6328cf319E85B10e09A228e84A8De
- https://twitter.com/AnciliaInc/status/1660767088699666433





