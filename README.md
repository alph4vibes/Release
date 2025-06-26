# NotArb

[![Join Discord](https://dcbadge.limes.pink/api/server/mYfAQnBfqy)](https://discord.notarb.org)

**NotArb** is a powerful trading platform for the Solana blockchain, featuring specialized arbitrage bots and utility tools.

---

### 🚀 Features

- **Jupiter Arbitrage Bot** – Cross-DEX arbitrage utilizing Self-Hosted Jupiter API
- **On-Chain Arbitrage Bot** – Direct on-chain analysis for profit-maximizing trades
- **Self-Hosted Jupiter API**
- **Essential Tools** – Includes Wallet Protection, WSOL Wrap/Unwrapping, Auto Update, Help, Version Information and other utilities

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

#### 🐧 macOS / Linux

##### 🔧 Jupiter Server
```bash
cd jupiter-server
cp example.toml myconfig.toml
```

##### 🔧 Jupiter Bot
```bash
cd jupiter-bot
cp example-jito.toml myjito.toml
# OR
cp example-spam.toml myspam.toml
```

##### 🔧 On-Chain Bot
```bash
cd onchain-bot
cp example.toml myonchain.toml
```

---

#### 🪟 Windows

##### 🔧 Jupiter Server
```bat
cd jupiter-server
copy example.toml myconfig.toml
```

##### 🔧 Jupiter Bot
```bat
cd jupiter-bot
copy example-jito.toml myjito.toml
:: OR
copy example-spam.toml myspam.toml
```

##### 🔧 On-Chain Bot
```bat
cd onchain-bot
copy example.toml myonchain.toml
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
.\notarb.bat jupiter-server\myconfig.toml
```

#### ▶️ Start Jupiter Bot
```bash
bash notarb.sh jupiter-bot/myjito.toml
```
**Windows:**
```bat
.\notarb.bat jupiter-bot\myjito.toml
```

#### ▶️ Start On-Chain Bot
```bash
bash notarb.sh onchain-bot/myonchain.toml
```
**Windows:**
```bat
.\notarb.bat onchain-bot\myonchain.toml
```

---

### ⚙️ Default Tasks

The `notarb.sh` / `notarb.bat` scripts support built-in tasks that simplify running and managing NotArb components.

You can run these tasks by passing them as arguments:

#### 🐧 macOS / Linux
```bash
./notarb.sh <task>
```

#### 🪟 Windows
```bat
.\notarb.bat <task>
```

---

#### 📋 Available Tasks

| Task                      | Description                                                      |
|---------------------------|------------------------------------------------------------------|
| `close-lookup-table`      | Closes a lookup table                                           |
| `create-lookup-table`     | Creates a new lookup table                                      |
| `deactivate-lookup-table` | Deactivates a lookup table                                      |
| `extend-lookup-table`     | Extends an existing lookup table                                |
| `help`                    | Displays a help message with available commands                 |
| `jupiter-bot`             | Starts the Jupiter arbitrage bot                                |
| `jupiter-server`          | Runs the self-hosted Jupiter API server                         |
| `onchain-bot`             | Starts the on-chain arbitrage bot                               |
| `protect-keypair`         | Encrypt a wallet file                                           |
| `rpc-health`              | Checks the health of an RPC endpoint (optionally pass `<RPC_URL>`) |
| `unwrap`                  | Unwrap WSOL                                                     |
| `update`                  | Automatically updates NotArb and its dependencies               |
| `version`                 | Displays version information                                    |
| `wrap`                    | Wrap WSOL     

---

### 🔄 Updating NotArb

You can update NotArb in two ways:

#### ✅ Option 1: Use the Built-In Update Task

This is the recommended method.

##### 🐧 macOS / Linux
```bash
./notarb.sh update
```

##### 🪟 Windows
```bat
.\notarb.bat update
```

---

#### 🧹 Option 2: Manual Update (Delete `release.txt`)

Deleting the `release.txt` file will force NotArb to fetch the latest release on the next run.

##### 🐧 macOS / Linux
```bash
rm release.txt
```

##### 🪟 Windows
```bat
del release.txt
```

---
## 🧠 Notes

- Running `jupiter-server` will automatically download the Jupiter Self-Hosted API.
- The `notarb.sh` / `notarb.bat` script handles environment setup, dependencies, and execution.
- It’s recommended to use a dedicated wallet with minimal funds for safety.
- When running bot tasks (`jupiter-bot`, `onchain-bot`, or `jupiter-server`), you must provide a corresponding `.toml` configuration file as the second argument.
- **Anyone running version < 1.0.15 is recommended to perform a clean install.**

---
## 🔗 Official Links

- 📦 [Download NotArb](https://download.notarb.org)  
- 📊 [Dune Dashboard](https://dune.notarb.org)
- 📊 [Dune On-Chain Dashboard](https://dune.com/notarb/notarb-on-chain-dashboard)
- 💬 [Discord Community](https://discord.notarb.org)  


