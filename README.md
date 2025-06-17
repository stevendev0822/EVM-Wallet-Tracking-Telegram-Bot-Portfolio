# EVM-Wallet-Tracking-Telegram-Bot

A professional real-time Ethereum and EVM-compatible blockchain wallet monitoring system that tracks transactions, and delivers instant notifications via Telegram.

<p align="center">
  <img src="https://github.com/steven228312/EVM-Wallet-Tracking-Telegram-Bot-Portfolio/blob/main/EVM%20Wallet%20Tracking%20Bot.gif" alt="Main Menu">
</p>

## EVM Wallet Monitoring Overview

This application monitors Ethereum and other EVM-compatible blockchain wallet activities in real-time, analyzes transactions, and sends detailed notifications through Telegram. It's designed for traders, investors, and developers who need immediate insights into wallet transactions across multiple EVM blockchains.

## Key Blockchain Tracking Features

- **Real-time Transaction Monitoring:** Track wallet activities as they happen on Ethereum, Polygon, BSC, and other EVM chains
- **Multi-wallet Support:** Track multiple wallets simultaneously through an intuitive Telegram interface
- **Multi-chain Compatibility:** Monitor transactions across different EVM-compatible blockchains
- **Detailed Transaction Analysis:** Identify token swaps, transfers, liquidity provisions, and contract interactions
- **Instant Telegram Notifications:** Receive formatted alerts with comprehensive transaction details
- **Transaction History:** Store and query historical transaction data with a database backend
- **Token Information:** Get detailed token data including symbols, names, and amounts

## DeFi Monitoring Architecture

The system is built on three core components:
- **Moralis API Endpoints:** Provides reliable blockchain data access with WebSocket connections to Ethereum and other EVM chains
- **Web3 Providers:** Distinguishes Wallet address from token contract addresses and validates 
- **Database Storage:** Stores transaction history for analysis and reference
- **Telegram Bot API:** Delivers real-time notifications and interactive user interface

## Installation for EVM Wallet Tracking Telegram Bot

```bash
# Clone the repository
git clone https://github.com/steven228312/EVM-Wallet-Tracking-Telegram-Bot.git

# Navigate to the project directory
cd EVM-Wallet-Tracking-Telegram-Bot

# Install dependencies
pip install -r requirements.txt
```

## Environment Configuration

Create a `.env` file in the root directory with the following variables:

```bash
# API Keys
MORALIS_API_KEY=Your Moralis API Key
TELEGRAM_BOT_TOKEN=Your Telegram Bot Token

# Optional Configuration
POLL_INTERVAL=20

# DATABASE CONFIGURATION
MONGODB_URI = mongodb://localhost:27017/db_name

# BLOCKCHAIN CONFIGURATION
ETH_PROVIDER_URI=https://mainnet.infura.io/v3/your-api-key
BSC_PROVIDER_URI=https://bsc-dataseed.binance.org/
BASE_PROVIDER_URI=https://mainnet.base.org
POLYGON_PROVIDER_URI=https://polygon-rpc.com
ARBITRUM_PROVIDER_URI=https://arb1.arbitrum.io/rpc
OPTIMISM_PROVIDER_URI=https://mainnet.optimism.io
AVALANCHE_PROVIDER_URI=https://api.avax.network/ext/bc/C/rpc
FANTOM_PROVIDER_URI=https://rpc.ankr.com/fantom
CRONOS_PROVIDER_URI=https://evm.cronos.org
GNOSIS_PROVIDER_URI=https://rpc.gnosischain.com
CHILIZ_PROVIDER_URI=https://rpc.ankr.com/chiliz
MOONBEAM_PROVIDER_URI=https://rpc.api.moonbeam.network
RONIN_PROVIDER_URI=https://api.roninchain.com/rpc
LISK_PROVIDER_URI=https://rpc.mainnet.lisk.com
PULSECHAIN_PROVIDER_URI=https://rpc.pulsechain.com
LINEA_PROVIDER_URI=https://rpc.linea.build
PALM_PROVIDER_URI=https://rpc.palm.io
```

## Setting Up Your Telegram Bot

1. Open Telegram and search for the @BotFather
2. Send `/newbot` command
3. Name your bot (e.g., "EVMWalletTracker")
4. Choose a username (e.g., "EVMWalletTrackerBot")
5. Save your bot token

## Crypto Tracking Usage

Once you clone the repository, install dependencies, and configure `.env`, you can simply start the application with the following command:

```bash
# Start the application
python src/main.py
```

## EVM Wallet Tracking Telegram Bot Commands

The bot supports the following commands:
- `/start` - Initialize the bot and see the welcome message
- `/track [chain] [address]` - Start tracking a new wallet
- `/list` - View all wallets you're currently tracking
- `/remove` - Remove wallets from tracking
- `/stop [chain] [address]` - Temporarily pause tracking for a specific wallet
- `/stopall` - Temporarily pause tracking for all wallets
- `/resume [chain] [address]` - Resume tracking for a paused wallet
- `/resumeall` - Resume tracking for all paused wallets 
- `/help` - Display available commands and usage instructions


## Sample Notification

```
🔔 New Wallet Activity

👛 Wallet: 0xfc9928f6590d853752824b0b403a6ae36785e535

🔗 Chain: Ethereum

🔍 Transaction Hash:
0x0561df1a3a5cc8ca68944cacf1d34a718ee7a7b2987a22869158cc33b1dc2eac

📊 Type: 🔴 SELL

🪙 Token: REALM (REALM)

📝 Token Address:
0x464fdb8affc9bac185a7393fd4298137866dcfb8

💲 Price: 0.00002340

📈 Amount: 146.16K

💰 Transaction Value: $3.42

🕒 Time: 2025-04-19 18:46:23 UTC

Stay sharp! Use /track to monitor more wallets.
```

## Technical Implementation

The system:
- Fetches transactions from EVM nodes using Moralis API
- Parses transaction data to extract relevant information
- Analyzes token transfers and ETH movements
- Formats and sends notifications via Telegram
- Stores transaction data in a database for historical reference

## Wallet Tracking Performance Considerations

- The bot fetches transactions from EVM chain periodically using Moralis API for efficient real-time monitoring
- Transaction data is cached to minimize RPC calls
- Database indexes optimize query performance
- Telegram message formatting is optimized for readability
- Multi-threading for handling multiple blockchain connections simultaneously

## Frequently Asked Questions

- **Does this bot require my private keys?**
  No, the bot only needs public wallet addresses to monitor transactions.

- **Can I track multiple wallets simultaneously?**
  Yes, you can track as many wallets as you need through the Telegram interface.

- **Which EVM chains are supported?**
  The bot supports Ethereum, Polygon, Binance Smart Chain, Arbitrum, Optimism, and other EVM-compatible networks.

- **Will I get notifications for all transaction types?**
  The bot focuses on token transfers, swaps, and ETH movements, filtering out less relevant transactions.

- **Is historical data available?**
  Yes, transaction data is stored in the database for historical analysis.

## License

This project is licensed under the [MIT License](./LICENSE).

## Contact Information

- Gmail: [steven0822.dev@gmail.com](mailto:steven0822.dev@gmail.com)
- GitHub: [Steven Leal(steven228312)](https://github.com/steven228312)
- Telegram: [@steven228312](https://t.me/steven228312)
- Twitter: [@steven228312](https://twitter.com/steven228312)
- Instagram: [@steven228312](https://www.instagram.com/steven228312/)

## Keywords

*Ethereum, EVM, Blockchain, Wallet Tracker, Telegram Bot, Real-time Monitoring, Transaction Analysis, Cryptocurrency, Trading Bot, DeFi Tools, Ethereum Transactions, Blockchain Monitoring, ERC-20 Tokens, Crypto Alerts, Token Tracking, Crypto PNL Monitoring, Ethereum Network, Blockchain Notifications, Cryptocurrency Trading, DeFi Monitoring, Ethereum DeFi, Wallet Notifications, Crypto Transaction Alerts, Blockchain Analytics, Whale Tracking, Token Transfer Monitoring, Crypto Portfolio Tracker, Polygon, BSC, Binance Smart Chain*
