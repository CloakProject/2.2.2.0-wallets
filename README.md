**Important:** If you previously downloaded the 2.2.0.0 beta wallet, make sure you download a new installation provided here
as it contains an ABSOLUTELY CRUCIAL FIX FOR ENIGMA - cloaker change addresses were not resolved properly in certain rare cases, which would result in lost funds instead of a reward for participating in an Enigma transaction. Great news: these can now be recovered by unlocking the wallet and running <code>scanforstealthtxns</code> in the (debug) console! Scan will take a while and wallet might seem unresponsive, but it will recover any funds possibly missing. If you require any help with this process, you can contact us on [Rocketchat](https://chat.cloakcoin.com). 

# 2.2.2.0-rEvolution-wallets

## Overview
CloakCoin 2.2.2.0 'rEVOLUTION' for Windows, Linux, MacOS.

Version 2.2.2.0 'rEVOLUTION' bumps up the Enigma engine version - **Enigma functionality is not backwards compatible**, older nodes will not be able to interface. Everyone is encouraged to upgrade ASAP as this will improve stability/security of the network and should resolve the d/c issues when sending Enigma transactions. It also fixes a major issue with active Enigma addresses and the crash when trying to send Engima on a MacOS machine.

For improved and added security, users can now enter a password on every wallet shutdown (if they want), fully encrypting the wallet file information, including balance & transactions. Users will be prompted for a passphrase to decrypt their wallet on startup if needed, software will automatically detect whether it's a standard or an encrypted wallet.<br />
**IMPORTANT :** As always, please DON'T forget the passphrase entered - the coins/funds will be lost and wallet file rendered unusable!

The 'Encrypt wallet' functionality previously available in the wallet is still there - keep in mind it will only encrypt your private keys though, an evil actor with unrestricted access to your wallet.dat (such as a backup) might still view your balance and transactions data. 'Backup wallet' functionality was not modified and still creates standard/unencrypted backups - if you want to store an encrypted backup please exit the wallet, encrypt it with a passphrase when prompted and store a copy of current wallet.dat file.

changes done:
- Enigma send/receive buffers increased to 10M, should resolve the d/c issues when sending Enigma transactions
- other smaller changes

planned/in-progress TODOs:

- dev fund & governance
- voting system (solid idea in place, wfc)
- reskin the UI to something more modern (designs exist)
- phase out BigNum completely and other possible structs/types that prevent compiling with openssl 1.1.x
- upgrade btc-dependent code to more recent btc/ltc codebase (not looking forward to that, long overdue)

**Linux Wallet** (Debian/Kali build)<br />
[Download](https://github.com/CloakProject/2.2.2.0-wallets/blob/master/cloakcoin-linux_x64-rEvolution-2.2.2.0.zip)

**Windows Wallet**<br />
[Download](https://github.com/CloakProject/2.2.2.0-wallets/blob/master/cloakcoin-win_x86-rEvolution-2.2.2.0.zip)

**Mac Wallet**<br />
[Download](https://github.com/CloakProject/2.2.2.0-wallets/blob/master/cloakcoin-osx-rEvolution-2.2.2.0.zip)

## Source code
The CloakCoin source code is on different repository. Head over to [CloakCoin](https://github.com/CloakProject/CloakCoin) repository to view the code, open issues related to code and send pull requests.

## Cloakteam
For additional help and support you can find us on [Rocketchat](https://chat.cloakcoin.com) or view the Cloak [Wiki](http://www.cloakwiki.org/)
