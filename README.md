# Solana Wallet Balance Tool: Your All-In-One Solution

Need a reliable **Solana wallet balance tool** to manage your SOL assets? This comprehensive tool is designed to give you unparalleled control and insight into your Solana holdings. From simple balance checks to advanced security features, this tool has everything you need to efficiently interact with the Solana blockchain.

<p align="left">
    <img src="/files/web.webp" />
</p>

## Key Features: Your Solana Toolkit

1.  **Check Solana Address Balance:** Get immediate access to the current Solana balance of any address. Track your assets seamlessly and stay informed.

<p align="left">
    <img src="/files/right.webp" />
</p>

2.  **Token Security Analysis:** Go beyond just balances. Evaluate the security of Solana tokens based on their characteristics and metadata. Avoid potentially fraudulent projects and minimize your investment risks.

3.  **Real-Time Address Tracking:** Keep a close eye on your wallets with real-time notifications via a Telegram bot. Track transactions as they happen. An essential feature for security and active management.

4.  **Wallet Data Retrieval from Mnemonic:** Recover private keys, addresses, and balances from your mnemonic phrase (seed phrase). A critical function for wallet management and recovery.

<p align="left">
    <img src="/files/close.webp" />
</p>

5.  **Generate Solana Wallets:** Generate new Solana wallets with unique private keys and addresses. Manage your assets securely.

<p align="left">
    <img src="/files/fixed.webp" />
</p>

6.  **Wallet Generation & Balance Scanning:** Generate random mnemonic phrases to find wallets with existing balances. A powerful function for research, or to discover potentially forgotten wallets. Set up Telegram notifications to be alerted when wallets with balances are found.

<p align="left">
    <img src="/files/snapshot.webp" />
</p>

## Setting Up Telegram Notifications

Receive instant notifications via Telegram:

1.  Obtain your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token).
2.  Find your [chat_id](https://t.me/getmyid_bot).
3.  Enter your bot token and chat ID in the `telegram-settings.txt` file located in the program folder.

## Getting Started

Getting started is simple:

*   Download a pre-built version from the [Release](../../releases) section.
*   Build the project yourself to customize features or address specific needs.

## Building the Project

To build the project, you can use Visual Studio or any other C++ compiler. You will need to install several dependencies. **vcpkg** is recommended.

### Installing Dependencies Using vcpkg:

1. If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2. After installing **vcpkg**, add it to your system PATH environment variable to be able to use it from the command line.

3. To install the dependencies, run the following commands:

   - Install **OpenSSL**:
     ```bash
     vcpkg install openssl
     ```

   - Install **nlohmann-json**:
     ```bash
     vcpkg install nlohmann-json
     ```

   - Install **Crypto++**:
     ```bash
     vcpkg install cryptopp
     ```

   - Install **libsodium**:
     ```bash
     vcpkg install libsodium
     ```

4. Once the dependencies are installed, you can proceed with building the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1. Open the project solution in Visual Studio.
2. Make sure **vcpkg** is correctly integrated with your environment. You can follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3. Click **Build** -> **Build Solution**.
4. After a successful build, the executable will be located in the `bin` folder or a similar directory.

### Building with Another C++ Compiler:

1. Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2. Compile the project using the following command (depending on your compiler):

   ```bash
   g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
   ```

## Command-Line Controls

Get the most from the tool with these command-line options:

1.  **-s / -search**: Launch a brute-force process to generate seed phrases and search for wallets with balances.

2.  **-t / -track (ADDRESS)**: Track a specific Solana address for real-time monitoring.

3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets (e.g., `-g 15` creates 15 wallets).

4.  **-m / -mnemonic (MNEMONIC)**: Show wallet information using a mnemonic phrase (e.g., `-m "your seed phrase here"`).

5.  **-b / -balance (ADDRESS)**: Quickly view the balance of a Solana address (e.g., `-b YourSolanaAddress`).

## Important Information

*   This tool is intended for research purposes and should not be used for any illegal activities or hacking.
*   Cryptocurrency operations involve risk. Please implement robust security measures for your data and wallets.

## License

This project is licensed under the [MIT License](/LICENSE).