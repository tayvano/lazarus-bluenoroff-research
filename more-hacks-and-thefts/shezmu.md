# Shezmu

Date:: September 20, 2024

Amount Stolen:: $4,900,000

Tags:: ITW?

---

## Details

Vault vulnerability that allowed unauthorized collateral minting. The hacker identified a critical flaw in Shezmu’s vault, allowing anyone to mint collateral freely.

The attacker returned the stolen funds to Shezmu after both parties agreed on a 20% bounty.




## Onchain

Shezmu’s recent contract upgrade on September 3 may have introduced or left the vulnerability unaddressed.

Attack Contract address: 0xEd4B3d468DEd53a322A8B8280B6f35aAE8bC499C

Shezmu Attacker address (created attack contract): 0xA3a64255484aD65158AF0F9d96B5577F79901a1D

Attack Contract Creation tx: 0x39328ea4377a8887d3f6ce91b2f4c6b19a851e2fc5163e2f83bbc2fc136d0c71


Just 17 days before the exploit, on September 3rd, Shezmu had deployed a contract upgrade: 

- 0xb18D3393786a3D95B22CDD6059Aa2abeB3907F0a

- 0x8db5356ec348a991adaadfd7f366d72eccafcb0113c7ac31f1dddde9c8c3f81e




## Technical Details

The attacker developed a custom smart contract designed to exploit this vulnerability.

Using the custom contract, the hacker minted a large amount of ShezUSD without the required collateral.


With the minted ShezUSD, the hacker borrowed a significant portion of the protocol’s resources, effectively draining $4.9 million.

The root cause of the Shezmu exploit was a critical vulnerability in their vault system that allowed unauthorized minting of collateral. This flaw enabled the attacker to mint ShezUSD freely, bypassing the necessary checks or collateral requirements.

The vulnerability likely stemmed from a contract upgrade implemented on September 3, which may have introduced the bug or failed to address an existing issue.



## Mildly Interesting:

This attacker also donated to REKT NEWS, a la Pancake Bunny

https://x.com/RektHQ/status/1397195892327858181