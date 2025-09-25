# Seedify / SFUND

Date:: September 23rd, 2025

Amount Stolen:: $1,700,000

Tags:: 🎙️

---

## Details

Today at approximately 12:05 UTC, a DPRK state-affiliated group known for many hacks in Web3 gained access to one of our developer’s private keys. Using these, they were able to mint a large amount of SFUND tokens through a bridge contract that had previously passed audit.

The OFT contract was compromised as a result, allowing the attacker to modify the contract settings and mint unauthorized tokens on Avalanche. 

This contract should not have been able to mint these tokens without any token being bridged. We used one of the most trusted and experienced auditors in the world to review these contracts and were assured that they were secure contracts that passed audits. We will be in touch with our auditors and security experts to review the security of all of our other infrastructure. 

These tokens were bridged to Ethereum, Arbitrum, and Base, where the attacker drained available liquidity pools, and subsequently bridged the maximum possible amount to BNB, where they were sold before we contained the breach.

There is no ongoing risk to liquidity on BNBChain anymore, and we have paused all bridges. However, we advise against purchasing tokens on other chains until further notice.

Once the issue was detected, we immediately coordinated with centralized exchanges to halt trading, blacklisted the attacker’s addresses across multiple chains, and revoked the compromised permissions. Once again, in addition to these: cross-chain bridges have been temporarily disabled.

Importantly, this incident was limited to a compromised wallet’s minting privileges. Core contracts, user wallets, our website, and the underlying protocol remain unaffected.

We deeply regret the impact of this incident and are committed to handling it with transparency. Further updates will be provided through our official channels.

We want to extend our deepest gratitude to our community and partners, your incredible support means the world to us during this time.

Since 2021, Seedify has been a home for builders and everyone dedicated to creating value in the Web3 ecosystem, through both bull and bear.

This unfortunate event won’t stop us, it only ignited our team to build better and bigger from here.

We also want to thank @zachxbt for connecting us with @zeroshadow_io to help us understand how the hack exactly happened and by whom.

On-chain evidence:

Ownership transfer from OFT contract owner to malicious entity:

https://basescan.org/tx/0x1dd7c101c18cd1adc80c4c68ce480862245a7223f8e5182136aed316eae54ac9

ETH hacked funds:

https://etherscan.io/address/0x14181636dd5bc8c6b8b47f8d0fd1b1e351b84be4#tokentxns

BSC hacked funds:

https://bscscan.com/address/0x14181636dd5bc8c6b8b47f8d0fd1b1e351b84be4#tokentxns

Attribution reference (DPRK Hacker):

https://x.com/zachxbt/status/1970488338529558795


## Onchain

- 0x9ccAdC790EDAbF89664f6F509a81D827C116D80b - Theft
- 0xda1d99d3b891678c9d5D16Efc0fdb6A098d21698 - Theft
- 0x14181636dd5BC8C6b8b47F8D0fd1b1e351B84bE4 - Theft
- 0x28c71c57f806fb674d9fa9d1fd47056b8d3da8bb - Theft
- 0xba5126f3f5dedd02cac8a16fb5c79d94526f719e - Theft
- 0x747afb5c7a7fc34b547cd0fdebf9b91759c5a52b - Theft
- 0x0693181206e7d8832e6086ecb61191b663525925 - Theft
- 0x29315c178765495d5035ef4f5b363b48f32874e1 - Theft
- 0x2b9fb5571bf1082f5db5b16cb136fd138414a1c6 - Theft
- 0x7b550bf2b89a0a4b81b16deceea9ae4395f49d16 - Theft
- TAuwk3N5mZWAwnbrgK67znj8BLv23RZevY - Theft


## Further Reading

- https://x.com/zachxbt/status/1970488338529558795

- https://www.web3isgoinggreat.com/?id=seedify-bridge-exploit

- https://x.com/SpecterAnalyst/status/1970505411397886046

- https://x.com/meta_alchemist/status/1970470733017968841

- https://x.com/SeedifyFund/status/1970537553515417918


## Connections

On Ethereum:

- 0x93a8b27C8DC2089BB071c22491a715DcB381F554 (Serenity Shield hacker) -> 0x6e1C7652C3fD9c19E9026DbB9a4D8895134432FF

On Arbitrum:

- 0x6e1C7652C3fD9c19E9026DbB9a4D8895134432FF -> 0x28c71c57F806Fb674d9FA9D1fd47056b8D3Da8bB (SFUND hacker)