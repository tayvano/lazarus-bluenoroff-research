# Genius Ventures / GNUS Token

Toke Exploit Date:: May 5, 2024

Original Key Compromise Date:: January 25th, 2024

Tags: 🎙️ Contagious Interview

Amount Stolen:: $1,262,630

---


On January 25th, 2024, 0xcfa7db433f7af2fe5902d5f6246f6cb7b92d90e6 was compromised and funds were sent and co-mingled with stolen funds from various known incidents including OKX DEX, CloudAI, Murall, and Linkedin Job Dev Scams.

On May 5th, 2024, GNUS were minted via Axelar Bridge, bridged to ETH, and dumped for appoximately 407.3 ETH.

From a glance, it looks like if they have the deployer they can basically control token mappings, so they made their own fake token, and used the real deployers compromised key to map it to the "real" one on eth mainnet

- https://etherscan.io/token/0x614577036f0a024dbc1c88ba616b394dd65d105a?a=0x548c63a6a7299ab54762e1bfa6b56c1b94c2a820

- https://ftmscan.com/address/0x548c63a6a7299ab54762e1bfa6b56c1b94c2a820

- https://ftmscan.com/tx/0xf7d41afe531a52391672ef460e841082801dccfe73bfa87a5af3c5785b5da774


The Founder/CEO and project spoke about the exploit a bit on Twitter/X, though given the reality that we **know** the founder/CEO's ENS name was drained of funds back in January, best to put this shitshow in the pile with the rest of the shitshows and not trust anything he claims.

> 🚨 Important Announcement 🚨
> Due to a recent exploit, a hacker was able to mint fake $GNUS tokens on Fantom, transfer via Axelar Bridge to Ethereum and Polygon, and sell into existing liquidity pools. 
> We will be conducting a snapshot at the block preceding the exploit. 
> To ensure fairness, please refrain from purchasing $GNUS tokens post-exploit, as we'll be issuing a new token. 
> Stay tuned for further updates. 
> #GNUSes #CryptoSecurity 
> cc: @axelarnetwork

– [X:GnusAI - May 5, 2024 13:53 UTC](https://twitter.com/gnusai/status/1787118358862942361)


> We've figured out that the hackers got the devs 0x18 deployment wallet during a discord hack. Apparently the hackers can watch private messages on discord. 
> This 0x18 was not the owners of the smart contract, but enabled them to launch exact address on FTM of the Axelar Token  Minter Manager contract.
> I think we have a quick fix.
> I'll be putting up $500k Eth into liquidity for the new pool, once we are sure it can't be hacked again.
> There is also roughly another $500k in fees locked until February 2025. we can add back in.
> We will then focus on bridging in the future and just work on the AI processing

– [X:SuperGeniusEth (CEO/Founder) - May 5, 2024 17:07 UTC](https://twitter.com/SuperGeniusEth/status/1787167358706196758)


> It turns out that the https://GNUS.ai contract wasn't hacked/compromised.
> The Axelar Management contract was duplicated on the FTM network. The deployer wallet may have been compromised so that it could be deployed to the same contract address.  
> But I'm also analyzing everything to make sure there isn't a way to deploy on Fantom using an exploit similar to this:
> https://medium.com/@solidity101/100daysofsolidity-081-deploying-different-contracts-at-the-same-address-a-solidity-deep-dive-3a954d0c3709#:~:text=To%20deploy%20different%20contracts%20at,address%20for%20multiple%20contract%20deployments. 
> We've disabled the bridging on Polygon and Ethereum; the base, BSC liquidity, and contracts were not affected.

– [X:SuperGeniusEth (CEO/Founder) - May 5, 2024 19:09 UTC](https://twitter.com/SuperGeniusEth/status/1787197943524810994 )





## Onchain - Jan 25

- 0x9249e360dc6f4d2871187acde4fe38d4e13a7703 - Irrigation Protocol: Deployer
- 0x35ea7aa2b9706a05cc932a7350a5e5a7d80619bf - DiamondCutFacet Contract
- 0xcfa7db433f7af2fe5902d5f6246f6cb7b92d90e6 - Genius Ventures: Deployer supergnus.eth
- 0x033524b1ba83ceabd8452c08dcafe71966b9b3f6 - Genius Ventures: GNUS Token
- 0x55f36651b5b61b8286305740fa86ad996fc8bdc9 - Other compromised address of supergnus.eth
- 0xb570e2b13677fb94d13c0e85f2173fb416326c89 - Other compromised address of supergnus.eth
- 0xb540226173a30e290280facadd772425a418a5c7 - Other compromised address of supergnus.eth
- 0x2265e38c9b446f9d36d3643e7c89984aef56e5b0 - Other compromised address of supergnus.eth
- 0x2768186eae06c11fee52509fc03d526544b88276 - Other compromised address of supergnus.eth
- 0xe8dfa9c13cab87e38991961d51fa391aabb8ca9c - Safe address of supergnus.eth
- 0x1db4d664d818d4c710d0aeb2d7d6b3ad885a8f19 - Direct Theft from Genius Ventures - Receives from OKX Exploiter 0 & 3

## Onchain - May 5

- 0x1804deca63705e18edf04f242b325bcd54a8b463 - GNUS.ai: Deployer (Malicious)
- 0x8c10c2867384c87d5a555e4f96c7036336b575c6 - TokenManagerProxy Contract (Malicious)
- 0x548c63a6a7299ab54762e1bfa6b56c1b94c2a820 - FTM / ETH, primary theft
- 0x0da5ec61970226a09e1f0b5fb17ebe0d28f01b87 - ETH, direct from theft addr
- 0x6a713b1f2b06557c87bb4998adbd5991576fa319 - ETH, direct from theft addr
- 0x962d41268dee9bb2001bf53479c4f7c449a5d1ca - ETH, direct from theft addr
- 0xa861f88665ef9a18947dca7df2ae1f56af608c1b - ETH, direct from theft addr
- 0x1d931ee940e7cf18735d7918ac0bca7b9b20840a - ETH, direct from theft addr
- 0xd4c953a1bb641ed7db1b30959aa571a64550cfbe - ETH, direct from theft addr
- 0x6a9fce38201912c179f1468f214816c1661adafd - ETH, direct from theft addr
- 0xf7d3fd93e4531c62fd7d775cdf5ac9b56b1fda1e - ETH, from 0x6a9, to allbridge, lifi
- 0x7a9767641afe13183868226f0be17947e22c615b - ETH, from 0x6a9, to allbridge, lifi, 0x3cd2
- 0x036462b0f8ebb6b2801a03237b2f17a385d2304d - ETH, from 0x6a9, to okx, lifi
- 0xfafde5bff6283ec91e5b38fa17baf3c4ac8f47d8 - ETH, from 0x6a9, to okx
- 0x544ade4167b6c906d14764443359b225ffa1369b - ETH, from 0x6a9, to okx
- 0x423a32d5271f9db3900f844422da83bc17fc277d - ETH, from 0x6a9, to lifi
- 0xacfe89ad639616b50fe3387442163f03992a00c9 - ETH, from 0x6a9, to lifi
- 0x3cd2c5457fe68f45830c9d404be3d9f02663c3a0 - BSC, from 0x7a97
- 0x14d8563e4ab937dfae8ec62ab740563f2af1301f - ETH, ss
- 0x7add0d62495f67fddcb0b423d4b86555fedabe41 - ETH, ss
- 0x6bace0bb35600717aea338b7330f64dfcabf0bb2 - ETH, ss
- 0x5dea9150a6e357b7c340c4191f7327249edafb49 - ETH, ss
- 0x012f038780e2e5e175aed098b4250aeeee5f63d8 - ETH, ss
- 0x0209d2ef64178507e36f61976d50e00b874ac8e3 - ETH, ss
- 0x8f8835ea06f0e85df18b62de8a588d980b5b381c - ETH, ss
- 0x31ae347d0214881c219f4f5fc5bf233fdd821bf5 - ETH, ss
- 0xeb97d19a3faf2da3e157feda3921bb4c69c0b0c3 - ETH, ss
- 0x96dca30d8013e94f9d020493e2f19cc508add232 - ETH, ss
- 0x721D39c25Fc4b195c7Dc1D89aA51BC77c8005af4 - ETH, ss
- 0x23C8CBde11DB519Ff8B3168451e2c2560Ce74E58 - ETH, ss
- 0x12E83f56ab77B4B6A69c190607C471f292A0459d - ETH, ss
- 0x6d6EB9bB9F39FB1145969877FF37a6F0fE043Ac9 - ETH, okx
- 0xE7fD2dB63904baAebDb0dF75b972EA411E8e76C9 - ETH, okx
- 0x14e1f688ce6a5450a2449f327dc2389dbaef3b23 - ETH, lbank
- 0x1e4d7dbadf410b65ac72edc8bf45c67e135487b5 - BSC, li.fi
- 0x46cb66c295a0e0e0c6447bf0d72bf8fc268c4e9f - BSC, li.fi
- 0x5a931edb07c34204bd9a9f84bfb324c83844b4db - BSC, li.fi
- 0x7e16b61a5817b0b428cac3cf7d652da3521527a2 - BSC, li.fi
- 0xab15c02b81dddbdb317bc6afcc07223830eeb00b - BSC, li.fi
- 0xd28458f5b9f79d534b93265c5476fcabe4336bf8 - BSC, li.fi
- 0xd53936e1890e1efef9a8131f7383d25031927dc8 - BSC, li.fi
- 0xe2cf8b921c05fcd620fe08128e1a9bf11ef01ce0 - BSC, li.fi
- 0xed420fd9bf1939ec4c3a67c8e288fdbcfc202e7e - BSC, li.fi
- 4KF9eq6Wi4CYzRyE8HbpQ5m3xc4zj8XtP288dvP8BPZZ - SOL, allbridge
- 5dzSpR6YXKbEgiadJZdNgVydFUwni52yTjuhyPCXNTKr - SOL, allbridge
- 9bDbcpE6FFp49vuGeUpwzF6LY9E4ujnsbfmbwRWhbHHr - SOL, allbridge ss
- BnGo9dnMaDAhsocF7c6tAdDQBdB8TgXzLTeVNN3CHFRj - SOL, allbridge
- G284Q3AUCVVuauSo5nN47UjtaUhLsTfevi4FeeyGz189 - SOL, allbridge
- 2UbUrp3AyWc1USq2m6arETNZqKatwEcQTzzKGomwJmge - SOL, allbridge from BSC
- omumczRi3okXKpE19tnHf5z8N7BwNHnbMRNWm7d1Scs - SOL, allbridge from BSC
- ErwaGB5MpkWstxSLsF3A3TRSvLReLRUZT7G4q38fWcXh - SOL, from omum
- 8LUBPiyMCFKM83qb3vAHjrFxP4tYcjTCSuD82672cBuH - SOL, allbridge from BSC
- H3LzaZuxS9BfZ8JzLsqhc46aFtF5rNm2sr1Dxw1NekVz - SOL, Lbank Depo
- 4UiA16jTfsCQBrpfSwBdjqy5hDdiewourLqpYcruUMd4 - SOL, Lbank Depo
- 96XmfuerVssWLnspGaJj7ZaJNoRPtdwRRTyCqk1b9dks - SOL, from 2UbUrp
- Hp1Fxs9esqj98qVWBwbwj63xafEfcqA36q2Wd5h9obvX - SOL, from 8LUB, 
- 7aq2KJ4K3idSSvAFDvAoAfZhG5iUHASNFnXcGQRXGKa4 - SOL, from 5dzS, Unk Service Depo
- 8NX3rUKskuyNgiYWRsRHXmG9rCPSYrtPdguEMiBHcqtr - SOL, from G284, Bybit Depo
- TKFJS6HZE9cnXn5ShM7LW9AcaCUTywwVRq - Tron, ss


Indicators from laundering on May 5, 2024 = Astril VPN out of Stockholm, Sweden. Timezone = Shanghai, -8