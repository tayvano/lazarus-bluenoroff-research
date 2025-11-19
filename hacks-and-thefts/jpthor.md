# JP Thor

Date:: September 9th, 2025

Time:: 

Amount Stolen:: $2,435,000

Tags:: 🔑

G:: 382609

---


## Details

Persona: Fake [Rena](./rena.md) (Stacks ecosystem)

> Got targeted AGAIN on my workstation. 
> Noticed a weird pop up which I dismissed. Immediately heard the Finder “download” sound (like you hear when copying files). 
> “That’s weird”
> Saw a pop-up - my entire documents folder being copied to a new folder /tmp
> “What?”
> Ran a quick script to see what was running  - someone had full remote access of my computer and had a copy script running. 
> Immediately disconnected from internet and did a full check. A osascript running from my terminal, copy files into Library/Caches then probably upload. 
> Insane. No idea how - could be anything from telegram/iMessage auto-download or worse. 
> My documents folder on desktop syncs to iCloud which has sensitive stuff. 
> Be super careful out there. At this point it’s not a matter of if - but when you will be targeted. 
> I did a full reset of my mac back to reset and will probably disable iCloud document syncing now. 
> Luckily I do not have private keys - only use  @vultisig so I’m safe even if I use iCloud to store one of 3 vault shares. 
> Be safe out there!

[Source](https://archive.ph/LEXFZ)



> After being targeted TWICE now
> I am absolutely convinced that you are insane if you are still using private keys. 
> Scammers will use AI agents at scale to target you and try and sniff those keys. 
> Vultisig is the correct solution (security through multi-factor) and I’m going to double down on it. 
> Been spiking the SDK to make it even easier to get Vultisig everywhere.

[Source](https://archive.ph/2WZZN)

> finally tracked down the source of the attack
> friend's hacked telegram account with a zoom link.
> Note: this is the OFFICIAL zoom link and I joined IN THE browser. I literally saw a deep fake of my friend, but couldn't hear anything so dropped off and tried on google meets. 
> INSANE - in 2 mins on being on the OFFICIAL zoom link - they had downloaded a malicious script to my computer and begun copying my entire iCloud documents folder to /tmp and probably to upload. 
> DO NOT USE ZOOM!!!!!!

[Source](https://archive.ph/KU1JE)


What I found on my computer running

[Source](https://archive.ph/msP8C)


> Ok so this attack finally manifested itself. 
> Had an old metamask cleaned out (which I forgot about, it was staking some assets which don’t appear on etherscan unless you use portfolio tracking sites)
> Summary 
> 1) friend’s hacked telegram account + deep-fake video on zoom
> 2) fake zoom link (likely) 
> 3) No pop-ups whilst I was on the link for 2 mins. 
> 4) Metamask was not being used in chrome for the active user - it was in another logged-out user profile (mac)
> 5) The metamask key was also stored in my iCloud Keychain 
> So I’m not sure if they were able to read across into the other user chrome profile (the active user had sudo priv) OR they fully swiped my (encrypted) iCloud Keychain. 
> There was no pop-ups asking for me to install anything or input my admin password. 
> It has to be an active or recently patched 0-day. 
> The only solution for this is threshold signature wallets - where key shares are split between multiple devices and you have to always co-sign. 
> Frustrating but I am deeply resolved to continue fixing and building @vultisig

[Source](https://archive.ph/x7Wda)


> It was a 8-year old metamask that has lived on there since the start. I don't use metamask any more, completely forgot I even had it, but got a notification there was still funds on it. 
> If you can't trust your iCloud Keychain - what can you trust? Do you use 1Password or something else?
> I only use @vultisig now for key shares tho

[Source](https://archive.ph/Wlmrm)

https://archive.ph/dfHRg




## Further Reading

- https://x.com/lookonchain/status/1966426219639144474
- https://archive.ph/LEXFZ
- https://archive.ph/2WZZN
- https://archive.ph/KU1JE
- https://archive.ph/msP8C
- https://archive.ph/x7Wda
- https://archive.ph/Wlmrm
- https://archive.ph/dfHRg

Another person targetted by fake Rena:

- https://x.com/sat_eth/status/1960290703826706563



## Onchain

- 0xb00e81207bcda63c9e290e0b748252418818c869 - Victim
- 0x04c5998ded94f89263370444ce64a99b7dbc9f46 - Victim

- 0x37cdb6b40861f350e23aa5733e75755fcbed739f - Direct Theft

- 0x53ecac52d80a04f9b7a06ce7a408ccc6e6daa27c - Theft

- 0xac0eb0be4c5db74ad946cda1043e4b9ccc9728bb - Theft / Tornado Ins

- 0x5f4d314f507ec70f11461b52afc01ecde7377005 - Theft / ChangeNOW Outs

- 0xc233aa1831251a6223cb35e9eb624bce8c3ea85a - Theft / FixedFloat Outs

- 0x26ab8d50d8b629501a25ceab6cb7f336cf9111e5 - Thorchain 2025-09-15
- 0x2837bd30577d1374a5418b4c1c2b6b9749284bc6 - Thorchain 2025-09-15
- 0x614e58853e5fffac9f49b36de524ddff3da1a179 - Thorchain 2025-09-15

- 0x7abc09ab94d6015053f8f41b01614bb6d1cc7647 - Theft Tornado Outs 2025-09-12

- 0x7973d39be58c61e9b9257cc660aee5f565e973da - Near Intents Depo
- 0x374ceee19d49589c307207d80eba1698c25c4dca - Near Intents Depo
- 0x2837bD30577D1374a5418B4c1c2b6b9749284Bc6 - Near Intents Depo
- 0x6b6b99fe0e07faf85175588b63fc72b6d460bcb2 - HitBTC Depo
- 0x19f9e44e113bea269330ece219cc3a5f2d4127d6 - HTX
- 0x1ab2e36f6a0e8e180d836199958eb76a4dc885b5 - Gate
- 0x0f7616c3f074673f9eba719071bf4a1c087476bb - Bitget
- 0x455440deb8a6a91eed8270f593e4cefed4dcc64b - FixedFloat
- 0x99315508c2ced01df873b81b9c1a4d5bcf9de3d4 - FixedFloat
- 0x6544ac2b5203ab4aaea2d68bc5e979520e87b0d1 - FixedFloat
- 0x83f385c1afaa82d6267d7ced849dcb85d0f96608 - FixedFloat
- 0xa0a418ee351ac2604fe76db6b3971fb4e31de296 - ChangeNOW
- 0xb36af3883956af663a745e293b4a71d545eece15 - ChangeNOW
- 0x023250cfd7fde41c0c36bd1cac6366888fa91388 - ChangeNOW
- 0x28e3a9f4bcb79fb803e88cff3530e3b38b815709 - Unknown Service
- 0x957d8ec8ea1e8dbf9aa4c75cbe6681ba2101ef88 - Unknown Service

- 0x9cc9a8fe6ee45e890e5168622bd6e9fed9d951f7 - Theft (2025-09-15)
- 0xff2cd87a7a9cad5621dafa18d692a2eba795d828 - Theft
- 0xa4491e8b313b1f6ae7457b3ccb221df27a8b2b26 - Theft

- bnb1z8pdtduepmhnnag672g3y8zxwk6kx9hyap3gyu - Victim
- bnb15umuwjaxymmhdyjujpnxwakywh2ra25knsszsh - Victim
- 0x83f385c1afaa82d6267d7ced849dcb85d0f96608 - FF Deposit
- 0x1e2afd94cec831a456b75b0198b544017e09f9c5 - Theft
- 0xbb3a46dd04e1ca0e59d73e55a4184b80e920858a - Theft
- 0x73f452858c88bda6e87a657d7ed2ed0e0cdbc7f7 - Theft / Holding $1.135 from BNB
- 0xb70f8680977000B492c68ace6c5097a6B7fB504F - Theft 2025-11-18
- 0x0bb6885d6992258256A517860C3484808Ee1d8Ad - Theft 2025-11-18


- 0x66844e1651e9aee73fdf8633902702682b8cdf9e - Gas Funder?
- 0xcbcd040651e80bb4fcfe685d54852181c9819d7f - From Gate
- 0xce747f7efdb82d3e3a1d3a9d02f8dbc17a199b9e - Testing?
- 0xb3e00e57935590c77ac7e0630c934b697b96caea - Testing?
- 0xaad0b7ea163314821cf850b50aaf3ab67b5ce7ee - Testing?
- 0x13288dad6f86c99ab652905458cc91a506e41f5b - Testing?
- 0xb35e98fc16b1c517dd758a6c6a565139b99259ed - Testing?
- 0x4d05600d1cad7d668dec2c5ccc8da7ed244225a8 - Testing? Dormant.
- 0xacdf9f722a0ee9d584da3790714c625659fa5b3a - OKX Depo



## Timeline

2025-09-04 12:45 - Call

2025-09-09 2:54 - Theft

2025-09-09 3:28 - Attempts to Dump

2025-09-09 23:45 - Starts Dumping

2025-09-10 03:30 - Done Dumping

2025-09-10 09:15 - Done for the day

2025-09-10 12:54 - loljk withdraw BNB (0x1e2afd94cec831a456b75b0198b544017e09f9c5)

2025-09-12 12:38 - More Cleanup

2025-09-17 13:08 - BNB Moves



### Tornado Cash

- 2025-09-10 13:14 - 0.1 ETH (Withdrawal via 0xac0)
- 2025-09-12 01:34 - 0.1 ETH (Deposit via 0xac0)
- 2025-09-12 08:44 - 0.1 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:45 - 0.1 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:46 - 0.1 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:47 - 0.1 ETH (Withdrawal via 0x7abc)

- 2025-09-12 01:34 - 1 ETH (Deposit via 0xac0)
- 2025-09-12 01:35 - 1 ETH (Deposit via 0xac0)
- 2025-09-12 08:51 - 1 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:52 - 1 ETH (Withdrawal via 0x7abc)

- 2025-09-10 13:01 - 10 ETH (Deposit via 0xac0)
- 2025-09-11 15:06 - 10 ETH (Withdrawal via 0x7abc)
- 2025-09-12 00:38 - 10 ETH (Deposit via 0xac0)
- 2025-09-12 01:19 - 10 ETH (Deposit via 0xac0)
- 2025-09-12 01:20 - 10 ETH (Deposit via 0xac0)
- 2025-09-12 01:33 - 10 ETH (Deposit via 0xac0)
- 2025-09-12 01:38 - 10 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:34 - 10 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:38 - 10 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:39 - 10 ETH (Withdrawal via 0x7abc)
- 2025-09-12 08:41 - 10 ETH (Withdrawal via 0x7abc)











