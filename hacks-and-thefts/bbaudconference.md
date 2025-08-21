# BbaudConferenceDV

Date:: April 29th, 2025

Amount Stolen: $7,919

Tags:: 🎙️ Contagious Interview

---



## Onchain

- 0x3FC1F081c9aaCF19C913552A96B5F336fDA52561 - Victim

- 0xf97dc3990a07aa72e44e6fc33d00eb2d37ebe531 - Theft (Also receives from Oxya Orgin Exploiter)

- 0x3a0f9A097962C36a072f841fF2C752b38A7656F0 - Theft (Also receives from Concentric Finance Exploiter 0xc62a25462a61f02ebab35cd39c5e9651426e760b on Arbitrum)




## Details

Hello,

I am reporting a wallet compromise that appears to be the result of a targeted phishing attack involving a malicious DApp.

The attacker, or someone working with them, first contacted me via Fiverr under the profile eduardo1124212, requesting assistance on a development project. As part of the project, I was invited to interact with a private GitHub repository and run the associated DApp locally. The repository is - https://github.com/BbaudConferenceDV/Monkey-M

During usage, I was prompted to connect my MetaMask wallet and sign a message under the pretense of "logging in." At no point was I informed that the signature would authorize any kind of token permission.

Hours later, I discovered an unauthorized permit() transaction from my wallet:

The signature I provided was likely crafted in such a way as to act as a valid ERC-2612 permit() call, allowing the attacker to transfer my tokens without further authorization.

I strongly believe this DApp is malicious and designed to trick users into unknowingly signing off-chain messages that grant on-chain permissions.

Please investigate this address, flag it as malicious, and take any actions necessary to prevent further victims.

Thank you for your time and support.

Private chats (Fiverr, telegram) - chats.zip

Dapp code - Monkey-M-main.tar.bz2

The interact.js file includes some MetaMask interactions that could be abused if paired with malicious logic:

It uses window.ethereum.request with the personal_sign method. This can be used to trick users into signing arbitrary messages — which can be used in phishing attacks to authorize malicious DApps or trigger gasless transactions with off-chain signatures.

It also connects to the wallet and fetches addresses.

This confirms that signed wallet messages are sent to a server via a GET request:

axios.get(`checkLoginMessage.php?publicKey=${walletAddress}&signedMessage=${signedMessage}&print=${fingerPrintStr}`);

https://github.com/BbaudConferenceDV/Monkey-M

https://www.chainabuse.com/report/771c7970-2788-4326-ac87-72546367fa40?context=search-address&a=0xf97dc3990a07aa72e44e6fc33d00eb2d37ebe531&chain=ETH


