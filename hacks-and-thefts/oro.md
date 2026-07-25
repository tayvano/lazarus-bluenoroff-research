# Oro

Date:: 2026-07-13

Amount Stolen:: $3,100,000

Tags:: 🔑


---

## Onchain

- `https://termslivz.com/meet/219695644440?p=TFRzzVe2RnKlL0d3jQ`

- 5FxFqEZFQcKj67JkAYXv4ZzRNWNyPQCm4sy11aejPb73Gqpv


## Details

https://x.com/oroagents/status/2079371018880041257 

Last week, after our ORO owner wallet was hacked, we made a promise to do a full post-mortem and share with the community what happened and how we’ve made improvements. This report is a result of our investigation. We want this report to serve 2 purposes:

To make sure that no wallet owner in Bittensor falls victim to the hack that we suffered.

Make it clear to the community what we’re doing going forward.

First, the most important things, unchanged from our initial update:

The subnet is fully operational.

The breach was contained to the SN15 owner wallet: 147K Alpha Tokens transferred and sold by the attacker. No other wallets, and no user or subnet data, were affected.

Validator signing keys were on hardware wallets and were never exposed.

What's new is that we now know how the attacker got in, who they are, and precisely what we're changing so this doesn't happen to us or anyone else in Bittensor again.

### 1. What happened

On June 18, our team member got on what he thought was a catch-up call with a founder he’d met at a conference. He’d talked to this founder before, and now, the founder was claiming to be someone building in our exact space.

Before the meeting, they sent a link that mimicked a Microsoft Teams meeting. The audio wouldn't connect, we were having issues and he said it might make sense to reschedule instead. The link then prompted the team member to update MS Teams. At the time they thought nothing of this.

We now know the "update" was an Apple script that 5 days later, would install itself as a malicious extension in all their browser profiles. It did the following:

It keylogged + captured clipboard history

It took screenshots, full-page capture, browser history, local/session storage every 30 seconds and sent it to a remote server.

Injected JS in-page (can swap crypto addresses live)

Then, from June 22nd, after the attacker had all this information, they were patient. They had root access on our team member’s machine. Then, there were weeks of quietly pulling cookies, keys, and eventually a wallet seed before draining the SN15 owner wallet on July 13.

### 3. Who was behind it
We attribute this attack with high confidence to Sapphire Sleet. They’re a North Korean state actor group that specifically targets cryptocurrency, blockchain, and AI teams.

https://x.com/MsftSecIntel/status/2066900551854330340

Our attribution is based on direct overlap between the indicators we recovered and public research from Microsoft Threat Intelligence on Sapphire Sleet's macOS campaigns. The IP address that our compromised machine was beaconing to, the matching payload and some overlapping infrastructure outlined in the above post from Microsoft makes us confident that the attack came from this group.


### 4. Timeline

Feb 2025: A team member meets a contact at an industry conference, a legitimate relationship. We exchanged messages on Telegram.

May 28th, 2026 (19:05 PT): Sapphire Sleet hacker, using this legitimate Telegram contact, reaches out asking the team member if they would like to schedule a meeting asking to catch-up. They flag that they’re building synton.ai, AI for e-commerce, the exact industry that ORO AI is building in.

Jun 18, 2026 (06:28 PT): The contact's compromised Telegram account is used to get the team member to run a malicious "software update" (an AppleScript) for a deceitful Microsoft teams meeting. Run manually, it bypasses macOS Gatekeeper, notarization, quarantine, and privacy (TCC) protections. A fake system password prompt captures the login password. Using this, the attacker establishes a foothold with elevated privileges. The original message that sends the malicious link is edited and corrected the “https://teams.live.com” meeting link.

Jun 22, 2026 (17:52 PT): . A malicious browser extension was installed by the initial updater, across the team member's browsers, enabling theft of cookies, credentials, and keystrokes, plus remote command execution.

~Jun 25, 2026: A second-stage implant is deployed to the laptop, maintaining a persistent, self-cleaning presence.

Jul 13, 2026 (10:27 AM PT): The ORO SN15 owner wallet is drained, selling 147K Alpha Tokens into the liquidity pool over the course of the next 10 hours.

Jul 13, 2026:  Within minutes of the drain, we detect and contain the intrusion. Over the next 24 hours, we kill the remote shell, quarantine the extension, and block the attacker infrastructure. Re-imaging and credential/key rotation begin.

### 5. The mistake we own

When we acquired the subnet slot, we decided that both the validator and the owner wallet would sit on hardware wallets. However, without widespread support of hardware wallets in Bittensor, we decided that temporarily, the owner key would be set up as a software wallet instead. This is what allowed it to be exfiltrated from a compromised machine. That was inexcusable, and it was our mistake. We are sorry for the impact this has had on our community and our supporters.

### 6. What we've done and what we're doing

We took immediate action to contain the incident and have been hardening every layer of our operations since. Some of this we shared last week, but this is the full list:

Wallets and keys

Completed a coldkey swap of SN15 ownership

Moving the subnet owner keys to multi-signature hardware protection. Thank you @const for making this significantly easier in the latest SDK update.

Adding a Conviction lock on owner emissions.

Endpoints and detection

Deploying per-host outbound firewalls on every machine — the control most likely to catch this class of attack in minutes/hours rather than weeks.

We have been working closely with @opentensor, @CrucibleLabs, @ConnitoAI, cryptocurrency exchanges, law enforcement, and members of the community, and have filed reports with the relevant authorities to pursue recovery of the stolen funds and raise awareness.

### 7. Looking forward

We promised to share this so it doesn't happen to anyone else. If you work on a subnet or hold keys, watch specifically for:

Unsolicited "install this SDK / update this meeting tool" requests. This applies even to people you know. A trusted account being compromised was the reason alarm bells did not go off. Especially taking advantage of the "I'm late for this meeting and need to join" effect.

Verify any downloads out-of-band before running anything.

Files ending in .scpt, or instructions to paste curl … | osascript / terminal commands.

Keep signing keys on a hardware wallet.

Multi-signature wallets mean that more than 1 person must be compromised for an attacker to gain access to your funds, greatly increasing security. This has recently been made a lot easier with changes in the Bittensor SDK.

Closing

This incident reinforced a hard lesson: building great products also requires continuously evolving our operational security. Our priority now is rebuilding the community's trust and continuing to ship improvements to the subnet.

To everyone who has stood by us, thank you. The best is yet to come.

Yours,

ORO