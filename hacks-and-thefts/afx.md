# AFX

Date:: 2026-07-22

Amount Stolen:: $24,047,838

Tags:: 👛

G:: 561367

---

## Details

- https://medium.com/@AFXTrade/afx-bridge-incident-what-happened-what-we-learned-and-what-comes-next-d97387746012

- https://x.com/AFX_XYZ/status/2080126901205770734

- https://x.com/blockaid_/status/2080080240265621680

- The malicious withdrawal was authorized by a quorum of hot-validator signatures and then finalized after the dispute period.

- Likely compromise or abuse of the bridge's hot-validator signing path. Five hot-validator signatures authorized a withdrawal of 24,150,000 USDC to the loot wallet, reaching 7,142 / 10,000 validator power (>2/3 quorum). The bridge contract then treated the withdrawal as valid and released funds after the 200-second dispute period.

### AFX Bridge Incident: What Happened, What We Learned, and What Comes Next

https://medium.com/@AFXTrade/afx-bridge-incident-what-happened-what-we-learned-and-what-comes-next-d97387746012

On July 22, AFX experienced a targeted attack that ultimately resulted in the compromise of the AFX-operated custody bridge.

Our investigation has since established the primary attack path.

While this incident resulted in the theft of assets, we believe its broader significance extends beyond AFX itself. Rather than exploiting a smart contract vulnerability, the attacker leveraged a modern software supply chain attack that combined **social engineering, trusted development tools, infrastructure persistence, and lateral movement.**

As software supply chains become increasingly complex, we believe these attack patterns deserve to be shared openly with the broader crypto community.

**What Happened**

**Stage 1: Social Engineering — The Initial Entry Point**

The attack began not with code, but with people.

On July 9, one of our developers was contacted through Telegram. During that interaction, the developer was instructed to clone what appeared to be a normal development repository.

The following commands were executed on a development workstation:

git clone --recursive https://<DEVELOPER>:glpat-********@git.oddium.io/dex/dex-aggregator.git  

cd dex-aggregator  

git switch --recurse-submodules dev

_The embedded GitLab token has been redacted for security reasons._

At first glance, these commands looked entirely consistent with a normal software development workflow.

However, the cloned repository contained malicious components that established the attacker’s initial foothold inside the development environment.

This marked the beginning of a multi-stage compromise.

**Stage 2: A Trusted Development Tool Became the Next Attack Surface**

Following the compromise of the developer workstation, the attacker expanded access into our internal software delivery infrastructure.

The next target was **JFrog**, the artifact repository that forms part of our development and deployment pipeline.

Rather than exploiting blockchain infrastructure directly, the attacker abused trusted software tooling — an increasingly common characteristic of modern supply chain attacks.

This shift is significant.

Today’s attackers increasingly target the software supply chain because compromising developer infrastructure often provides a path into production systems without ever exploiting blockchain protocols themselves.

**Stage 3: Why the Compromise Was Difficult to Detect**

On July 16, the attacker uploaded a malicious Groovy plugin (ops_maintenance.groovy) into our JFrog environment using compromised administrative privileges.

Shortly afterward, the JFrog EC2 instance began experiencing severe out-of-memory (OOM) conditions, resulting in service degradation.

Because the symptoms appeared operational rather than security-related, our engineering team immediately engaged **JFrog’s official support team** to investigate.

Following their review at that time, the issue was believed to be consistent with backup-related disk utilization, and the system was considered safe to restore.

Acting on that assessment, the affected host was restarted.

Unfortunately, the restart also caused the malicious plugin to be automatically reloaded, allowing the attacker to re-establish persistence without raising additional alarms.

Only after the subsequent forensic investigation did we discover that the attacker had also modified core system components, including the gssproxy process, injected malicious shared libraries (libsn-proc.so), and deployed additional persistence mechanisms (jf.js).

This sequence illustrates one of the defining characteristics of modern supply chain attacks: Operational symptoms may closely resemble ordinary infrastructure failures, making early detection extraordinarily difficult — even when trusted vendors are involved in the investigation.

**Stage 4: Lateral Movement Across Internal Systems**

With persistent access established, the attacker began moving laterally through our internal infrastructure.

Instead of directly targeting blockchain assets, the attacker systematically expanded privileges across multiple internal systems until eventually reaching validator-related infrastructure.

This progression — from developer workstation to infrastructure services and ultimately validator systems — demonstrates a sophisticated attack chain rather than an isolated software exploit.

**Stage 5: Validator Compromise and Bridge Theft**

During the final stage of the attack, the attacker downloaded and executed a remote script from:

<https://23.27.48.177/claude-lastest>

Execution of this payload ultimately enabled unauthorized access that resulted in the theft of assets from the AFX-operated custody bridge.

At this stage of the investigation, we have found no evidence that the Arbitrum network or the native Arbitrum bridge was compromised.

The incident was isolated to infrastructure operated by AFX.

**What This Incident Teaches**

This incident fundamentally changed how we think about blockchain security.

The attack did not begin on-chain.

It began with a developer.

It did not exploit a smart contract.

It exploited trust.

It did not target consensus.

It targeted the software supply chain.

As the crypto industry matures, protecting smart contracts alone is no longer sufficient.

Development environments, CI/CD pipelines, artifact repositories, build systems, and operational tooling have become part of the protocol’s security boundary.

Every trusted component in the software supply chain is now a potential attack surface.

**Security Advisory to the Industry**

Based on our investigation, we encourage development teams to review the following immediately if they have recently experienced unexplained operational issues involving JFrog:

* Unexpected out-of-memory (OOM) events;
* Unexplained service restarts;
* Unauthorized plugins (especially ops_maintenance.groovy);
* gssproxy modifications;
* Unknown shared libraries such as libsn-proc.so;
* Suspicious JavaScript files including jf.js.

Operational anomalies should never be dismissed as purely infrastructure issues until security compromise has been ruled out.

We will continue publishing additional indicators of compromise (IOCs), forensic evidence, and technical findings over the coming days.

**Looking Ahead**

The security investigation has now established the primary attack path.

Our attention is now turning toward recovery.

A comprehensive recovery plan for affected users is currently being finalized and will be shared with the community as soon as it is complete.

We hope that openly sharing this investigation can help strengthen the resilience of the broader crypto ecosystem.

**Transparency does not undo what happened. But we believe it is the first step toward rebuilding trust. We remain committed to learning from this incident, strengthening our infrastructure, and earning back the confidence of our community through actions — not words.**


## Onchain

- https://arkm.com/explorer/entity/f5e5fdea-d613-4163-9b71-5414b564199a

### Victim / Compromised 

- 0xCb3B9A3E5668AFE84DC7A864B36b845dCE062e67 - Bridge contract
- 0x5553EA7Bda594aDE7AFe91D279779a42b2B84208 - Finalizer
- 0x32E3200D6E944cd9bD1C8C9865293B07206e7A01 - Withdrawal creation sender
- 0x00BB84aF06daC03BFe744Da13dF9D2D6fd8e77E5 - Validator
- 0x27259f90D6ae500262AcE6E8428434e0c1f308F5 - Validator
- 0x2e26dE22a92e41704B3eA00cc65a6CDA47b12c9e - Validator
- 0x52D4D9AD78a53a69bD089eE8f282CE0Cd0506Da7 - Validator
- 0xBB472BC3962Ad02Ac660429FdBB319B5BC66DA7b - Validator

### Attacker

- bc1q3ff9au48n4jzusxvj73tnuapgt9e6lredqwhkn - Funding
- 3GM3UZt1mUh7LetQzPDZZX7o3Q7g3TCYfv - Funding
- 0x32e3200d6e944cd9bd1c8c9865293b07206e7a01 - Funding
- 0x2f2974fAbc54dbA33442261211c06BD20E0FEefc - Attacker
- 0x627654b2782bfc57580ecd11d40869b350b6ebac - Holder
- Exploit tx: https://arbiscan.io/tx/0x50d0b3ec6c3f5fce0f10abf81540bbb508f421494aa2b3480c4a264b0436547b
- Withdrawal creation tx: https://arbiscan.io/tx/0x217c45c1272550e0439e53243f2987b7fb3f58b1d33c222597bbb71851b93f74

### Laundering

#### Hop 1

- 0xd8a282d3cf54af666ae741a6cffc917c30fbcf95
- 0x7cbd780e482620102b09234b06303f9735855abd
- 0xc4039e44eea75a8a9d5f54bc0b38ce8450e0324e
- 0x7e1e71acfeb371228f46817d587e72cfa00e9d9b
- 0x8f9516fb99304e340bd8d9470aff6441fdba2a79
- 0x22222cd9f4f46a269311707f99f49ba6ed200553
- 0xe13d00f7f87548f47e3729af9ab150c9676e43da
- 0x27187cc6f852aba5d963551690674c0ae2745d41
- 0x4eedad8ce8c6a5b20d7acbb1bce92317311a9d39
- 0xcb17229dc772cfd8d36769709fd2ffa2f4dd7230
- 0xc934f593f1070d7ae0a7eba618504599fda1b1cd
- 0xbaeabebd0a9158edfb43dee63a5b9b16ed641354
- 0x53592308bbf60688929bfba814a47fe837eaaed2
- 0x1c80319d30431a497e2c52e50dfefec99d0d7d8e
- 0x678335b4d6a393c4891275d3d23aedd8ad596d14
- 0x7097957e5ee49cd6c204cb735bbb6dd23fe55bdc
- 0x1a587644c0fb5702a7f169692272f4844890f390
- 0xc997acaffb423e988eee328864c36072a644ced2
- 0xb52071b125ffbaf8ad545bd099b75b84efdd5430
- 0xfd3c8eea05d979a64053888de5eb4584a2754cb4
- 0x309c41ac45ee2bc9516320653d9d57fce2ddc9ce
- 0x0eede253f588b0c2beac64bc9cff4930b50c75d3
- 0x18ed71f6b5f02c44d5692d323bea030ac18acc40
- 0x4872b3842cbf3bdf490de8814f1f62d993206b9d
- 0x8cffde7919af9f9c4032e3a2d62d3a49de49cc64
- 0x79f73be17e620e8208ff653642ea10f7f854295d
- 0x8c22862d2a21f30402dd8b49872965bc9b746d8e
- 0x80119426cb6d9a1c700aa21e1604ef7bda657649
- 0xe2d93c01be1ae8e7eaf6c4723ad1ca8aada96539
- 0xd3f4d444518d0b0ec10fd67c4973a9643b7f426a
- 0xf02EEe51f78B49B7fC3575862E77FAeE95cd1b71
- 0x88A84742D73F81bf19EF3a49577446ef254fd8bb
- 0x2b300dc730b13b2870bf046E5cA6c9C45113F457
- 0xf5D7Ea8a70477C19DaE72E1471891d2a3E33A98a
- 0xc86Af3d2A14f9D5c6cB446E8C181A122C82961eF
- 0x5D99aad175eC826c8bFA182B426679A94FaEdd3b
- 0xf637339e7483f475fd65c57f61f85ee736a8ccb2 - Dust
- bc1qd6cpyslvahkg8dsxp4lgmku0gh996ftuql0d5d
- bc1q3xwmnjma5hcd74d93da2qn7240d4qfdpxemnfy
- bc1qhul96rjh39uuylumvd2rf6y6qsmru2twj8ex43
- bc1q3p5hkgqsnauudpy5hdff3hduusztx6dgudxngh
- bc1qncntje6me0rmlj4nh3raslhdjq9z0fs2qlrkt2
- bc1qpxp4lj738f2tglka5s00m5vshcfw60cd4fdx0g
- bc1qvydm9k9pkn5r9unh30xupzgypuh4ejaqajzcfy
- bc1qntq7wqfmmna79yh4djjahh563karjj3e3qunp9
- bc1q2rs7x4vhun80l2vt7zcg9lkce77az9s83pmm6a
- bc1qp9hterlkytzc99xhnxceh767nljn72ylpske7z
- bc1qt2tk2fcxz5uaa3r6pqswz03mhj4g08d9fkfmak
- bc1qpj6rt8ana5ukzg3e290rsquyx44yrvpvjgkntl
- bc1qvuu28us93xguz237ttvjva672dw3804xzhty9w
- bc1quaqkdkl0af2d0ycjm8klu809leslqykxfqtuxy
- bc1q8et5224kcmudc3svz45w8wzayqetn5n4k5zy60
- bc1q7kvp8gr483cdxgp56z9aje83rcmz6aytdtp3zd 
- bc1qg3p6kr7ytkrqjt97jqxs8dmeyyp2hawg5f95jl 
- bc1qmzyrrmxschreuehw5lyxwua9ysnl25zjn5mhy2 
- bc1qv6ugavgzw8h6s33v4putzmrpqnyrjrh0m0ga22 
- bc1qfdqc80ylpc4e80kcqrnr5vjhmp32qym98jr27n 
- bc1qgktzh7s8fds7drsp0dka8s7ylhmshye5qteyv5 
- bc1qlynw5qt0zckqa7ffwp25gv0n3tnzlujgkl7w6p
- bc1qxw55gvzs0g55f87r3f4rywrcpz6s88tlk2jh2c
- bc1qjtr6gjcwwysg3p5l9z4duykg95ytptdp8pamhp
- bc1qsux0y23tkjcespf4tqmkemf9ymzwps0mhxgfsk
- bc1qamr6qedjtqeskxwtnr79d8esyzdqpyn6m6p2ka
- bc1qhk84lt4qm3ldq9nw0l0prpglwhuj975ensu52w
- bc1qefq5hwnfwzy7kaup9aygdsvgth84xyrfd38wcl
- bc1qdeulx7y5thsgwx568syltu6ryy0l7kmtz889xn
- TY1XWgzEsBmCd5mog5yXnSbbNLPpynk94P
- TAPhwWRddFq14hLqFCSGvQ89MG9KJdPPBF