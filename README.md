# Auto Daily Encrypt ↔ Decrypt on Fhenix Testnet

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/07c47955-c2f1-486e-b2cc-853fd2529a6f" />

---

## 🚀 Features
- Random daily target (e.g., 14–24 tx/day)
- Random amount per tx (e.g., 0.001–0.01 ETH)
- Random delay between tx (e.g., 3–5 minutes)
- UTC rollover: sleeps silently until next UTC midnight after hitting the daily target
- Safety checks: address checksum normalization, optional chainId check, preflight for contract code
- Debug mode for troubleshooting reverts (no spam by default)

---

## 📦 Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/Kurisaitou/auto-encrypt-decrypt-on-Fhenix-Testnet.git
```
```bash
cd auto-encrypt-decrypt-on-Fhenix-Testnet
```
```bash
npm install
```

## ⚙️ Environment Setup
Create a .env file in the project root:
```bash
nano .env
```
Fill in your wallet details and randomization settings:
```bash
RPC_URL=https://1rpc.io/sepolia
PRIVATE_KEY=your_privatekey
CHAIN_ID=11155111
FROM_ADDRESS=your_address

# Target contract (leave default if same)
CONTRACT_ADDRESS=0x87A3effB84CBE1E4caB6Ab430139eC41d156D55A

# Recipient; default = FROM_ADDRESS
TO_ADDRESS=your_address

# Random daily transaction count (you can change)
DAILY_TX_MIN=14
DAILY_TX_MAX=24

# Random amount range in ETH (you can change)
AMOUNT_MIN_ETH=0.001
AMOUNT_MAX_ETH=0.01

# Random delay between tx in MINUTES (you can change)
DELAY_MIN_MINUTES=3
DELAY_MAX_MINUTES=5

# First action of the day: encrypt | decrypt
START_WITH=encrypt
```

## ▶️ Running the Bot
To start the bot:
```bash
node index.js
```

## 🔖 Tags
#eth #fhenix #swap #bot #crypto #web3 #automation #trading #dex #evm #airdrop #encrypt #decrypt #fhenix-testnet
