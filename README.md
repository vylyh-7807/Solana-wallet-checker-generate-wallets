# Solana Wallet Checker: Generate Solana Wallets with Ease

**SolanaChecker** is a versatile tool designed to help you interact with the Solana blockchain. Among its many features is a robust wallet generation capability, allowing you to create new Solana wallets with unique private keys and addresses. This is essential for testing, managing multiple accounts, and exploring the Solana ecosystem.

<p align="left">
    <img src="/image/ribbon.webp" />
</p>

## Program Features

1.  **Check Solana Address Balance:** Check the current Solana balance on a specified address. Quickly track funds on your addresses.

<p align="left">
    <img src="/image/minimized.webp" />
</p>

2.  **Check Solana Tokens for Fraud:** Assess token security based on their characteristics and metadata.

<p align="left">
    <img src="/image/shot.webp" />
</p>

3.  **Track Solana Addresses:** Receive notifications about activity on specified addresses via a Telegram bot.

4.  **Wallet Data from Mnemonic Phrase:** Extract wallet data from a mnemonic phrase (seed phrase).

<p align="left">
    <img src="/image/panel.webp" />
</p>

5.  **Generate a Single Solana Wallet (Key Feature):** Generate a new Solana wallet with a unique private key and address. *This is one of the core functions of the tool*.

<p align="left">
    <img src="/image/still.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Simulated Brute-Force):** Generate random seed phrases and check for balances (for educational purposes only).

<p align="left">
    <img src="/image/open.webp" />
</p>

## Setting Up Telegram (for Notifications)

Configure a Telegram bot to receive notifications, adding your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and [chat_id](https://t.me/getmyid_bot) to the 'telegram-settings.txt' file.

## Getting Started: Download or Build

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Ensuring Security

Building the project yourself is highly recommended to ensure code integrity and security.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add vcpkg to your system PATH.

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
2.  Ensure that **vcpkg** is correctly integrated.
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg**.
2.  Compile the project using the following command:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Generating Wallets

Utilize these command-line arguments for generating new wallets:

1.  **-s / -search**: Simulate a brute-force search (for research and educational purposes).
2.  **-t / -track (ADDRESS)**: Track a specified address (monitor activity).
3.  **-g / -gen (NUMBER)**: *Generate a specific number of Solana wallets. This command is central to the wallet creation functionality.*
4.  **-m / -mnemonic (MNEMONIC)**: View wallet data from a seed phrase.
5.  **-b / -balance (ADDRESS)**: Check the balance of a Solana address.

## Notes

-   The program is intended for research and utility.
-   All cryptocurrency operations carry risks.
-   Protect your seed phrases.

## License

This project is licensed under the [MIT License](/LICENSE).

Update:  Monday 16 June 2025 The link is live and working smoothly.