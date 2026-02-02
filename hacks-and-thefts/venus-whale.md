# Venus Whale

Date:: 2025-09-01

Time:: 9:05 UTC

Amount Stolen:: $27,000,000 (minus $3,000,000 used for the position)

Tags:: 🔑 POS

G:: 382712

---

## Details

Persona:: Someone from Stacks BD, male, not Rena


> Updating a few new pieces of information:
> 1. The Venus protocol should be fine, but we cannot rule out the possibility that the Venus frontend has been hijacked, and then phishing attacks were launched targeting large holders (the Venus team can investigate this part as well)
> 2. The large holder's computer may have been subjected to a targeted poisoning attack (currently under investigation)
> 3. The hacker was very premeditated, with somewhat complex funding sources, among which the gas came from XMR exchanges
> 4. The large holder and we are coordinating, many details will not be expanded for now, and the actual loss is not accurate either, it may not have exceeded 20 million USD. As for why, you can analyze the hacker's address yourself:
> https://bscscan.com/address/0x7fd8f825e905c771285f510d8e428a2b69a6202a#tokentxns
> These updates are issued to avoid unnecessary speculation and panic in the market. But we are also investigating many details, so the information is for reference only.

- [Source: Slowmist's evilcos](https://x.com/evilcos/status/1962823780298101111)



> Continuing updates: In this incident where the whale was hacked, the Venus protocol and frontend should both be fine. 
> Currently, our joint analysis with partners points to the whale being targeted in a specific attack. 
> Although the whale used a hardware wallet, the related wallet extension on the computer (used in combination with the hardware wallet) was replaced. 
> When the user issued a normal redeemUnderlying operation, it was replaced with an updateDelegate operation:
> https://bscscan.com/tx/0x75eee705a234bf047050140197aeb9616418435688cfed4d072be75fcb9be0e2
> This operation ultimately led to the theft of their assets in Venus:
> https://bscscan.com/tx/0x4216f924ceec9f45ff7ffdfdad0cea71239603ce3c22056a9f09054581836286
> The hacker's funds targeting this whale, with Gas coming from XMR exchanges, and other related fund tracing back to eXch—that sanctioned, taken-down dark web exchange, which North Korean hackers previously liked to use...:)

- [Source: Slowmist's evilcos](https://x.com/evilcos/status/1962834677871583256)



> UpDate: Venus Protocol has been fully restored (withdrawals and liquidations resumed) as of 9:58PM UTC. ✅
> The lost funds have been recovered under Venus' protection. ✅

- [Source: Venus Protocol](https://x.com/VenusProtocol/status/1963017766098907282)



> Kudos to @VenusProtocol! The lost funds have now been recovered by force-liquidating the exploiter's position.
> Here is the related tx: 
> https://bscscan.com/tx/0xee9928b8d1a212f4d7b7e9dca97598394005a7b8fef56856e52351bc7921be43

- [Source: Peckshield](https://x.com/peckshield/status/1963031758347370608)



> TL;DR: A user was the victim of a phishing attack. To protect them, the protocol was immediately paused. We now propose a partial resume so that users can manage their positions and avoid liquidations, while also force-liquidating the attacker’s wallet. Once a full security review is complete, the protocol will be fully resumed.
> What happened
> We have confirmed this was a phishing attack in which the victim unknowingly signed a transaction authorizing the attacker to borrow and withdraw from Venus Protocol on their behalf. As a result, funds were drained from the victim’s wallet into the attacker’s.
> Fortunately, the suspicious transaction was identified almost immediately, and Venus Protocol was paused. Because of this quick response, the stolen funds remain locked in the attacker’s wallet and this is why Venus is currently paused.
> Why this vote matters
> We are fully aware of the market risks of keeping Venus paused. But above all, we are committed to protecting our users and our community. In an industry plagued by bad actors, we believe protocols should stand by their users whenever possible.
> This is why we are calling for a fast-track Snapshot vote: time is critical not only for the affected user, but also for the broader Venus community.
> Proposed plan
> Within 5 hours — Partial restoration of Venus Protocol.
> Users will be able to adjust their positions (repay debt / supply funds) and avoid liquidations (which remain paused).
> This action will be performed through a Guardian transaction.
> Within 7 hours — Force-liquidate the attacker’s wallet.
> Stolen funds will be recovered in a single transaction.
> This will not affect any other user positions on Venus.
> Within 24 hours — We will continue to do a complete security review on Venus to prevent any replication of this attack on any other users.
> We will perform a full review of Venus contracts to ensure this attack cannot be replicated.
> Venus Protocol will be resumed fully
> Venus Protocol will be resumed fully, and we will continue to provide transparent updates to you via X throughout this process.
> Call to action
> As time is of the essence, please cast your vote on this Snapshot within 1 hour. If approved, we will immediately execute the plan outlined above.
> Hackers have no place on Venus. Thank you for your patience, understanding, and continued trust as we work tirelessly to protect our users, safeguard our community, and uphold the integrity of the Venus Protocol. The community is the foundation of Venus, and we will always act in your best interest.

- [Source: Venus Protocol Snapshot](https://snapshot.box/#/s:venus-xvs.eth/proposal/0x140da3dcb6dc711429700443d3b9f1def51eaae3b791f8b774664676f418a132)



## Recovery

Almost all of the stolen assets were recovered by the victim.

The math is approximately 

- $31,751,000 - Gained Initially

-  $2,930,000 - DPRK funded themselves to unwind the position

-    $250,000 - Amount that wasn't frozen



## Onchain

- 0x563617b87d8bb3f2f14bb5a581f2e19f80b52008 - Victim

- 0xc753fb97ed8e1c6081699570b57115d28f2232fa - Venus Recovery

- 0x42bD4DC1DF5e7eFa9bA299DE82C450fF7ACAFEe7 - DPRK Personal/Testing

- 0x149B8f32626B1Cf0023dF867620C9C2Fb0228c48 - DPRK Personal/Testing

- 0x7Bc9982123C3F49E16fc5bDD14D61B664E214B22 - Test of hack - https://bscscan.com/tx/0x2210188616d2a761cf2dae83889669e8439ab8c53c5b23f6c068b2184564ce02

- 0x5de3c5be52d7adbdc3aefe2ea061a2ece0c7d766 - SoF (likely from [NFPrompt](./nfprompt.md))

- 0x8492de414ca0e39f209e04099b34148f9103d8f6 - SoF (likely from [NFPrompt](./nfprompt.md))

- 0x7a35b01388a060b64cc8623086a30f8e3923889b - from 849, used to repay position

- 0x7fd8f825e905c771285f510d8e428a2b69a6202a - Theft

- 0x0455ed2a52b6118a804bb01cb8e144dda7f75cb5 - Theft

- 0x30aa3c5492370af9734694368b226347a5649be8 - from Tornado Cash (2025-08-21)
- 0xac1fc481591cad579589b9b06e670b702ee22370 - from Tornado Cash (2025-09-01)

- 0x208fe65b608c0303acd42a9d8de1451652ffee49 - Funds Holder (2025-09-08)

- 0xfa1f6ea06380ba940f94cc2c26f9ce05862084e4 - Dust 2025-12-03

- 0x0f0408a4b02b945e6be34c4851bbcafc5d2dae37 - Dust 2025-12-03





