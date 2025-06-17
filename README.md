# Solana Wallet Checker CLI: Powerful Command-Line Tool for SOL Management

**SolanaChecker** is a command-line interface (CLI) tool built for interacting with the Solana blockchain. This provides users with a flexible, powerful way to manage their wallets, check balances, analyze transactions, and more. The CLI design makes it ideal for automation, scripting, and efficient interaction with the Solana network.

<p align="left">
    <img src="/files/flow.webp" />
</p>

## Program Features, Designed for the CLI

1.  **Check Solana Address Balance (CLI Focused):** Easily check the current Solana balance of any specified address. This is a foundational CLI command for quickly assessing your SOL holdings.

<p align="left">
    <img src="/files/line.webp" />
</p>

2.  **Check Solana Tokens for Fraud (CLI for Analysis):** Assess the security of tokens based on their characteristics and metadata. This helps traders avoid investing in potentially fraudulent projects and make informed decisions from the command line.

<p align="left">
    <img src="/files/control.webp" />
</p>

3.  **Track Solana Addresses (CLI and Telegram):** Receive notifications about activity on specified addresses, which can be configured through a Telegram bot. This provides real-time monitoring and allows you to track transactions effectively.

4.  **Wallet Data from Mnemonic Phrase (CLI for Security Checks):** Extract the private key, address, and balance of a Solana wallet from the seed phrase. *Ideal for command-line use in verifying wallet details*.

<p align="left">
    <img src="/files/plate.webp" />
</p>

5.  **Generate a Single Solana Wallet (CLI for New Wallets):** Generate a new Solana wallet with a unique private key and address from the CLI.

<p align="left">
    <img src="/files/app.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (CLI - Brute-Force Simulation):** The CLI allows you to perform a brute-force process for generating random seed phrases and checking the created addresses for a balance. *This feature, for educational purposes, highlights the importance of strong seed phrases.*

<p align="left">
    <img src="/files/final.webp" />
</p>

## Setting Up Telegram (for Real-Time Notifications)

To receive notifications in Telegram, configure your bot token and chat ID. Add these to the 'telegram-settings.txt' file within the project folder. This is helpful for automated monitoring of events.

## Getting Started: Download or Build

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project (CLI Focused)

Building the project provides the best way to control the build process, dependencies and ensure your copy is safe.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  After installing **vcpkg**, add it to your system PATH environment variable.

3.  Run the following commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Build the project.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure that **vcpkg** is integrated correctly with your environment.
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile the project using the command (example):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line - Your Gateway to Solana Control

Utilize the command line interface to execute functions.

1.  **-s / -search**: Start the brute-force seed phrase generation.
2.  **-t / -track (ADDRESS)**: Start tracking the specified address.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Display wallet information using the seed phrase.
5.  **-b / -balance (ADDRESS)**: *Check the Solana balance of the specified address. This command is central to the CLI usage.*

## Notes

-   The program is intended for research purposes.
-   All operations with cryptocurrencies carry risks.
-   Secure your data and wallets.

## License

This project is licensed under the [MIT License](/LICENSE).



Update:  06/17/2025 05-47 Hey everyone, the broken link has been fixed.