# NotArb

[![Join Discord](https://dcbadge.limes.pink/api/server/mYfAQnBfqy)](https://discord.notarb.org)

**NotArb** is a powerful trading platform for the Solana blockchain, featuring specialized arbitrage bots and utility tools.

---

### 🚀 Features
- **Self-Hosted Jupiter API**
- **Jupiter Arbitrage Bot** – Cross-DEX arbitrage utilizing Jupiter API
- **On-Chain Arbitrage Bot** – Direct on-chain analysis for profit-maximizing trades
- **Essential Tools** – Includes WSOL wrapping/unwrapping and other utilities

---

## ⚠ Security Warning

> ✅ **Only download NotArb from the official release page:**  
> [https://github.com/NotArb/Release/releases](https://github.com/NotArb/Release/releases)  
>
> 🚫 Never enter private keys on shared or untrusted machines.

---

## 🛠 Getting Started

### 1. Download & Extract

Download the latest release from:  
➡️ [https://github.com/NotArb/Release/releases](https://github.com/NotArb/Release/releases)

Extract the `.zip` and navigate to the folder.

---

### 2. Configure Your Bots

Depending on your strategy, modify the appropriate `.toml` configuration file. You can edit the example file or copy it:

#### 🔧 Jupiter Server
```bash
cd jupiter-server
cp example.toml myconfig.toml
```

#### 🔧 Jupiter Bot
```bash
cd jupiter-bot
cp example-jito.toml myjito.toml
# OR
cp example-spam.toml myspam.toml
```

#### 🔧 On-Chain Bot
```bash
cd onchain-bot
cp example.toml myonchain.toml
```

---

### 3. Running the Bots

> 🛠 On first run, NotArb will automatically install Java and other dependencies.  
> 🧑‍💻 **You may need to run with admin privileges (e.g., `sudo` on macOS/Linux).**

#### ▶️ Start Jupiter Server
```bash
bash notarb.sh jupiter-server/myconfig.toml
```
**Windows:**
```bat
notarb.bat jupiter-server\myconfig.toml
```

#### ▶️ Start Jupiter Bot
```bash
bash notarb.sh jupiter-bot/myjito.toml
```
**Windows:**
```bat
notarb.bat jupiter-bot\myjito.toml
```

#### ▶️ Start On-Chain Bot
```bash
bash notarb.sh onchain-bot/myonchain.toml
```
**Windows:**
```bat
notarb.bat onchain-bot\myonchain.toml
```

---

## 🧠 Notes

- Running `jupiter-server` will automatically download the Jupiter Self-Hosted API.
- The `notarb.sh` / `notarb.bat` script handles environment setup, dependencies, and execution.
- It’s recommended to use a dedicated wallet with minimal funds for safety.

---
## 🔗 Official Links

- 📦 [Download NotArb](https://download.notarb.org)  
- 📊 [Dune Dashboard](https://dune.notarb.org)
- 💬 [Discord Community](https://discord.notarb.org)  


