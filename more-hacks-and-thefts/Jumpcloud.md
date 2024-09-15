# JumpCloud

Date:: July 20, 2023

Attribution:: [TraderTraitor / Jade Sleet](https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/)

---



## Details

In July 2023, Mandiant Consulting responded to a supply chain compromise affecting a US-based software solutions entity. We believe the compromise ultimately began as a result of a sophisticated spear phishing campaign aimed at JumpCloud, a zero-trust directory platform service used for identity and access management. 

JumpCloud reported this unauthorized access impacted fewer than five customers and less than 10 devices.The details in this blog post are based on Mandiant’s investigation into the attack against one of JumpCloud’s impacted customers.

Mandiant attributed these intrusions to UNC4899, a DPRK-nexus actor, with a history of targeting companies within the cryptocurrency vertical. 

Mandiant assesses with high confidence that UNC4899 is a cryptocurrency-focused element within the DPRK's Reconnaissance General Bureau (RGB). Based on reporting from trusted partners, UNC4899 likely corresponds to TraderTraitor, a financially motivated DPRK threat group that primarily targets blockchain-related companies.

On June 11, Phylum’s automated risk detection platform alerted us to a peculiar pattern of publications on NPM. The packages in question seem to be published in pairs

Two weeks after the IT management firm JumpCloud announced that it was the victim of a supply chain attack aimed at a small population of customers in the cryptocurrency industry, an investigation by ReversingLabs researchers has uncovered evidence of more malicious npm packages, with links to the same infrastructure that also appear to target cryptocurrency providers.

Specifically, ReversingLabs identified a number of additional npm packages with links to the same malicious campaign. One, named __btc-api-node__, was uploaded to npm on July 11th and has links to a supply chain attack first[ identified by the firm Phylum on June 23


## URLs

- https://jumpcloud.com/blog/security-update-incident-details

- https://jumpcloud.com/support/july-2023-iocs

- https://mandiant.com/resources/blog/north-korea-supply-chain

- https://techcrunch.com/2023/07/20/north-korea-backed-hackers-breached-jumpcloud-to-target-cryptocurrency-clients/?guccounter=1

- https://sentinelone.com/labs/jumpcloud-intrusion-attacker-infrastructure-links-compromise-to-north-korean-apt-activity/

- https://reuters.com/technology/n-korea-hackers-breached-us-it-company-bid-steal-crypto-sources-2023-07-20

- https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/

- https://blog.phylum.io/sophisticated-ongoing-attack-discovered-on-npm/

- https://blog.phylum.io/junes-sophisticated-npm-attack-attributed-to-north-korea/

- https://github.blog/2023-07-18-security-alert-social-engineering-campaign-targets-technology-industry-employees/

- https://cisa.gov/news-events/cybersecurity-advisories/aa22-108a



## IoCs

### Malicious Domains (Source: [Github](https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/))

- npmjscloud[.]com
- npmrepos[.]com
- cryptopriceoffer[.]com
- tradingprice[.]net
- npmjsregister[.]com
- bi2price[.]com
- npmaudit[.]com
- coingeckoprice[.]com


### Malicious npm Packages  (Source: [Github](https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/))

- `assets-graph` 
- `assets-table` 
- `audit-ejs` 
- `audit-vue` 
- `binance-prices` 
- `coingecko-prices` 
- `btc-web3` 
- `cache-react` 
- `cache-vue` 
- `chart-tablejs` 
- `chart-vxe` 
- `couchcache-audit` 
- `ejs-audit` 
- `elliptic-helper` 
- `elliptic-parser` 
- `eth-api-node` 
- `jpeg-metadata` 
- `other-web3` 
- `price-fetch` 
- `price-record` 
- `snykaudit-helper` 
- `sync-http-api` 
- `sync-https-api` 
- `tslib-react` 
- `tslib-util` 
- `ttf-metadata` 
- `vue-audit` 
- `vue-gws` 
- `vuewjs`


### Malicious GitHub Accounts (Source: [Github](https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/))

- GalaxyStarTeam 
- Cryptowares 
- Cryptoinnowise 
- netgolden


### Malicious npm Accounts (Source: [Github](https://github.blog/security/vulnerability-research/security-alert-social-engineering-campaign-targets-technology-industry-employees/))

- charlestom2023
- eflodzumibreathbn
- galaxystardev
- garik.khasmatulin.76
- hydsapprokoennl
- leimudkegoraie3
- leshakov-mikhail
- linglidekili9g
- mashulya.bakhromkina
- mayvilkushiot
- outmentsurehauw3
- paupadanberk
- pormokaiprevdz
- podomarev.goga
- teticseidiff51
- toimanswotsuphous
- ufbejishisol


### Malicious Domains (Source: [JumpCloud](https://jumpcloud.com/support/july-2023-iocs))

- `nomadpkgs[.]com` 
- `centos-repos[.]org` 
- `datadog-cloud[.]com` 
- `toyourownbeat[.]com` 
- `datadog-graph[.]com` 
- `centos-pkg[.]org` 
- `primerosauxiliosperu[.]com` 
- `zscaler-api[.]org` 
- `nomadpkg[.]com` 
- `launchruse[.]com` 
- `Reggedrobin[.]com` 
- `Canolagroove[.]com` 
- `alwaysckain[.]com`






