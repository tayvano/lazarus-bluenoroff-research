# WOO X

Date:: July 24th, 2025 

Time:: 11:55–14:29 UTC (Thursday)

Time:: 20:55–23:29 KST (Thursday)

Time:: 13:50–15:40 UTC+8 (According to Woo X. The timezone on this is clearly wrong lol)

Amount Stolen:: $14,038,066

Tags:: 👛 UNC4899 or UNC5565 (per Woo X Post Mortem)




---


## Details

According to the official disclosure, the incident stemmed from a targeted phishing attack that compromised a team member’s device, allowing the attacker to gain access to the development environment.


## Original WOO X Statement


We're currently investigating a contained incident that occurred on WOO X earlier today

While user funds and trading are unaffected, withdrawals have been temporarily paused while we complete the investigation.

1. To provide further details, the incident has affected 9 user account who had unauthorized withdrawals placed.

The incident was quickly detected and as a precaution, withdrawals were paused and many of the withdrawals were blocked. We've already contacted the affected users, and all unauthorized withdrawals will be covered.

2. As we continue with the investigation, we can confirm losses of $14m from the affected accounts. These users will have all funds covered.

We are working with external security teams and other exchanges to halt the flow of funds. Appreciate your patience on this matter.

Update 3: The exploit stemmed from a team member device being compromised in a targeted phishing attack, allowing the exploiter to gain access to the development environment. Many security measures limited the access, but gave the exploiter time to coordinate a series of withdrawals from the user accounts mentioned in the previous message.

The exploiter requested the first withdrawal at 13:50 UTC+8

Subsequent withdrawal requests came in gradually and the exploit was discovered and halted at 15:40 UTC+8

The team is in the process of a complete forensic review and is prioritizing the re-opening of withdrawals for all users

We will update here as soon as that's completed

Update 4: Nearly all pending withdrawals have been processed, and all systems are now operating normally. For the 9 affected accounts, we’re working to fully restore balances within the next 24–48 hours.

We continue to work with leading security firms to further strengthen our cloud and database infrastructure. A full transparency report on the incident will be shared in the coming days.

We’re also cooperating with law enforcement in an effort to recover the stolen funds. Additionally, we are offering a 10% bounty to the attacker—should the remaining funds be returned, we will drop all further actions.

We know this has been a difficult time for our users and community. Thank you for your patience and continued support.

Update 5: Balances for the 9 affected accounts have been credited from our company treasury.

Reminder: No WOO tokens were stolen, and none were sold or distributed in order to compensate affected users.

Update 6: We’ve been working with Mandiant to perform a comprehensive investigation of the incident. Their deep expertise in cybersecurity and Google Cloud infrastructure makes them the ideal partner as we work to protect performance and security for our traders.

Update 7: We are continuing to talk to law enforcement and tracing firms to monitor the stolen funds, which haven't moved since the original exploit. On the tech side, we are in the remediation phase of our investigation. The next steps are:

- complete the security review

- app hardening

- re-automate withdrawals

- full incident post-mortem

If remediation goes smooth, we hope to complete these steps by next week. In the meantime, all trading operations are still normal.

Withdrawals are still being manually verified, if you have a pending withdrawal, reach out to http://support.woox.io to help verify.

Source: https://x.com/_woo_x/status/1948400223761342920
)







## Woo X Post Mortem

On July 24, 2025, WOO X experienced a sophisticated security incident that resulted in $14 million in unauthorized withdrawals from 9 user accounts. There is evidence that this attack was perpetrated by UNC4899, a North Korean state-sponsored cyber espionage group aligned with the Reconnaissance General Bureau and known publicly as Lazarus Group, TraderTraitor, and Jade Sleet.

The attack began with social engineering targeting our development team through what appeared to be a legitimate open-source collaboration request. A team member was approached on an open-source software forum to help debug a development tool. After a brief discussion, the developer downloaded the file on mobile, then used their company-issued MacBook to open the file. Prior to opening, the file was assessed for malware, but the scan was negative. After running, the program downloaded a hidden backdoor that resembled a common backend process. This allowed the exploiter to maintain access to the development environment, and after a period of time, find an opportunity to make changes in the database, gaining access to 9 accounts from which withdrawals were initiated. 

The unauthorized withdrawals were detected 2 hours later, immediately halted, and all affected users were fully compensated from WOO's treasury. Over the following three weeks, an investigation and remediation process ensued. This led to a number of new security and risk measures being implemented, along with a full migration of the development environment.

### Incident recap

The incident originated from a targeted social engineering attack against our development team. The threat actor:

- Researched WOO's development practices and identified team members active in open-source communities

- Crafted a legitimate-seeming collaboration request for debugging assistance on a development tool

- Delivered malware disguised as open-source code 


### Timeline of Events

June 28, 2025
- External party approaches WOO developer on open-source forum requesting collaboration on development tool debugging

July 8, 2025
- Developer downloads project file on mobile device
- File AirDropped to company MacBook to access using development tools (Cursor)
- Backdoor deploys undetected, establishing persistent access

July 9, 2025
- First evidence of threat actor accessing Google Cloud (GCP) environment via compromised developer's VPN session
- Actor leverages existing 2FA-protected VPN connection from infected MacBook

July 10, 2025
- Threat actor accesses Google Kubernetes Engine (GKE) resources
- Begins reconnaissance of Argo CD and Apollo deployment infrastructure

July 11, 2025 - July 24, 2025
- Privilege escalation achieved: Actor deploys malicious POD revealing Kubernetes management service account token
- Deploys backdoor in microservice POD for persistent access to production environment
- For the two weeks after deploying the backdoor, no threat active behavior was observed
- Persistent access validated but unused during this period

July 24, 2025
- 13:50 UTC+8: Threat actor returns via backdoor in node server
- Uses previously extracted database credentials to access backend systems
- Replaces user emails, passwords, and 2FA seeds for 9 high-value accounts
- First unauthorized withdrawal initiated
- 15:40 UTC+8: Suspicious activity detected and contained
- Immediate response: Withdrawals suspended platform-wide, affected user account details restored

### Financial Impact
- $14 million in unauthorized withdrawals from 9 user accounts
- Funds stolen across multiple chains: Bitcoin, Ethereum, BNB, Arbitrum
- 100% user compensation provided from WOO treasury
- Operational Impact
- Withdrawal services suspended for security review
- Enhanced monitoring and incident response procedures activated
- Development environment isolation and forensic analysis
- No impact to trading services


### User Impact
- 9 users experienced account compromise
- All affected users contacted directly and compensated fully
- Platform trading remained operational throughout incident
- The treasury loss does not impact WOO's operational runway or business continuity - WOO maintains substantial reserves and a diversified treasury structure. 



Source: https://woox.io/blog/july-24th-security-incident-post-mortem









## Amount Stolen


- Time (BTC Theft):: 11:55–14:11 UTC

- Time (ETH Theft):: 12:16–14:29 UTC

- $5,579,872 - 1504.82 ETH

- $3,645,734 - 30.8 BTC

- $2,167,257 - 7,000,000 TRX

- $2,043,031 - 547.99 ETH on Arbitrum

-   $602,172 - 773.41 BSC



## Onchain

- 0x14896e88e0f7dce1fb88a979439c2f87b416c024 - Direct Theft

- 0x87aab7bac1308faf2a0d59da26b8379e18b26355 - Direct Theft (ETH + ARB + BSC)

- 0x1891438f4cfdff9e145285a3f15c8b2c52b571cc - Direct Theft (BSC)

- bc1qxvft9ytzjx50ylqnglc0fsd5ck0v6hayl2xsyh - Direct Theft (BTC)

- 0x04a94f134a808140cc3e6ffac064f8a9fecb465a - Initial Theft / Funds Holder (773.41 BSC)

- 0x77167f0bc412eb39d004f354869938e7c5acd518 - Initial Theft / Funds Holder (99.99 ETH)

- 0x889b49ef0bf787c3ddc2950bfc7d1d439320004b - Initial Theft / Funds Holder (1,404.82 ETH + 547.99 ETH on ARB)

- bc1q4xm6y972qa82f4cudr4d28xdhxa4e68v5atrej - Initial Theft / Funds Holder (4 BTC)

- bc1qvd58w5kperw3hzu7j5gkca8rxkzwd7vjxtu2gh - Initial Theft / Funds Holder (4.9 BTC)

- bc1qtzlpu326jcqnx8tnhrkqcfxjhn9e02zfutzsch - Initial Theft / Funds Holder (10 BTC)

- bc1qut0g2uflywfcycuftuek7944p6hhxgm2p92fzm - Initial Theft / Funds Holder (11.9 BTC)

- TUchNtdDgLXzhSSC32QaNnzKVPj2rNg8dX         - Initial Theft / Funds Holder? (7,000,000 TRX)


## Further Reading

- https://x.com/PeckShieldAlert/status/1948559304707244117

- https://x.com/_WOO_X/status/1948400223761342920

- https://x.com/_WOO_X/status/1948573397178339577

- https://support.woox.io/hc/en-us/articles/49178783818777-Temporary-withdrawal-suspension-July-24-2025




## IoCs

- Nord VPN