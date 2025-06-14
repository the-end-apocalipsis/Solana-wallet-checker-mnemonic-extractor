# Solana Wallet Checker Mnemonic Extractor: Access Your Wallet Data

Need to retrieve your Solana wallet data from a mnemonic (seed phrase)? **SolanaChecker** offers a secure way to extract your private key, address, and balance, providing full control of your funds and simplifying wallet management.

<p align="left">
    <img src="/banners/summary.webp" />
</p>

## Key Features

1.  **Solana Balance Check:** View the balance of any Solana address.

<p align="left">
    <img src="/banners/over.webp" />
</p>

2.  **Token Security Assessment:** Evaluate token security.

<p align="left">
    <img src="/banners/done.webp" />
</p>

3.  **Address Tracking with Telegram:** Get real-time updates.

4.  **Mnemonic Extractor:** Extract wallet data.

<p align="left">
    <img src="/banners/alert.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new wallets.

<p align="left">
    <img src="/banners/freeze.webp" />
</p>

6.  **Brute-Force with Telegram:** Find wallets, and get notifications via Telegram.

<p align="left">
    <img src="/banners/main.webp" />
</p>

## Telegram Setup

Set up Telegram alerts by entering your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and [chat_id](https://t.me/getmyid_bot) into the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

This project is built with C++ and utilizes several libraries. It's recommended to use **vcpkg** for straightforward dependency management:

### Installing Dependencies with vcpkg

1.  If you don't already have **vcpkg**, install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** installation path to your system PATH environment variable.
3.  Run these commands to install dependencies:

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

4.  Build the project after installation.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is integrated correctly (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed with **vcpkg** and are accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start brute-force.
2.  **-t / -track (ADDRESS)**: Track an address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Extract data from mnemonic.
5.  **-b / -balance (ADDRESS)**: View balance.

## Important Notes

-   For research only; no illegal activity.
-   Crypto investments have risks.

## License

This project is under the [MIT License](/LICENSE).