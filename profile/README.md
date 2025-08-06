
# 💎 Tstocks — Onchain RWA Stock Trading Protocol on TON
<img width="1024" height="418" alt="banner" src="https://github.com/user-attachments/assets/1129971c-fd4c-4f6e-964f-c09fbb9b782b" />

> Trade real-world stock assets on-chain with **zero KYC**, **full self-custody**, and **leveraged trading** powered by **TON** and cross-chain bridges.

---

## 🌐 Overview

**Tstocks** is a decentralized application (Dapp) built on **TON (The Open Network)** that allows users to trade tokenized real-world stocks (RWA) such as Tesla, NVIDIA, Apple, and more — all **without KYC**.

💡 Whether you're looking to trade spot, go long with leverage, or even short sell — Tstocks gives you all the tools in a fully onchain, transparent environment.

---

## 🪙 Supported Stock Assets

All assets are issued by [Backed.fi](https://backed.fi) and accessible via TON smart contracts:

| Name      | Contract Address                                 | Information URL                                                  |
|-----------|--------------------------------------------------|------------------------------------------------------------------|
| Tesla     | `XsDoVfqeBukxuZHWhdvWHBhgEHjGNst4MLodqsJHzoB`     | [Tesla xStock](https://assets.backed.fi/products/tesla-xstock)  |
| NVIDIA    | `Xsc9qvGR1efVDFGLrVsmkzv3qi45LTBjeUKSPmx9qEh`     | [NVIDIA xStock](https://assets.backed.fi/products/novo-nordisk-xstock) |
| Meta      | `Xsa62P5mvPszXL1krVUnU5ar38bBSVcWAB6fmPCo5Zu`     | [Meta xStock](https://assets.backed.fi/products/meta-xstock)    |
| Apple     | `XsbEhLAtcf6HdfpFZ5xEMdqW8nfAvcsP5bdudRLJzJp`     | [Apple xStock](https://assets.backed.fi/products/apple-xstock)  |
| Amazon    | `Xs3eBt7uRfJX8QUs4suhyU8p2M6DoUDrJyWBa8LLZsg`     | [Amazon xStock](https://assets.backed.fi/products/amazon-xstock) |
| Google    | `XsCPL9dNWBMvFtTmwcCA5v3xWPSMEBCszbQdiLLq6aN`     | [Google xStock](https://assets.backed.fi/products/alphabet-xstock) |

---

## 🔐 Wallet & Account System

Tstocks supports multiple wallet standards, with both **custodial** and **non-custodial** options:

### 🧩 MPC (Multi-Party Computation) Wallets

- **Web3Auth Integration**
  - Login with Google, Apple, or Email.
- **Security Options**
  - Local Storage (self-custody)
  - Telegram Cloud Encrypted Storage

### 🪪 External Wallets

- Connect via:
  - **TON Wallet** (TonConnect)
  - **EVM Wallet** (Metamask, WalletConnect)
  - **Phantom Wallet** (Solana)

### 🔑 Additional Features

- Private Key import/export
- Hierarchical Deterministic (HD) Wallet derivation

---

## 💱 Deposit System & Bridging

### 💸 Deposit

- Native Solana address QR code for seamless funding

### 🌉 Multi-chain Bridge Aggregator

- Integrated bridges:
  - [FF.IO](https://ff.io)
  - [Exolix](https://exolix.com)

---

## 📈 Spot Trading

Tstocks allows instant spot trading between **stablecoins (USDT/USDC)** and RWA tokens:

- ✅ **Gasless Transactions** for users
  - Gas fees sponsored by relayer (payer)
- 📊 **PNL Analysis** dashboard
- 🛒 Asset Controller Interface:
  - Buy / Sell stock tokens with stablecoins

---

## 📈📉 Leveraged Long Trading

Trade with leverage by staking stablecoins to gain increased exposure:

### 🚀 Long Workflow

1. **Stake**: User deposits `100 USDT` to the vault
2. **Trade**: System adds user’s `10 USDT`, leverages `90 USDT` from vault
3. **Hold**: Tstocks purchases and holds RWA token
4. **Close/Liquidation**:
   - Sell all stock tokens
   - Return funds to vault and user

---

## 📉📈 Leveraged Short Trading

Bet against stock price with borrowed tokens:

### 🔻 Short Workflow

1. **Stake**: User deposits `100 xStock` to vault
2. **Borrow**: Other user contributes `10 USDT`
3. **Trade**: Holder sells `90 xStock` for stablecoins
4. **Close/Liquidation**:
   - Buy back stock token
   - Return excess profit to user, vault earns fees

---

## 📊 Protocol Architecture

```mermaid
flowchart TD
    A[User Wallet] --> Z[Stake To Protocol]
    A[User Wallet] --> B[Self Generate Wallet]
    B --> C[Spot Stock Trading]
    C --> H[Buy]
    C --> I[Sell]
    B --> D[Leverage Trading ]
    D --> F[Make Long]
    D --> G[Make Short]
    F --> E[Close or Liquidtion]
    G --> E[Close or Liquidtion]
````

---

## 🌍 Why Tstocks?

* ✅ **No KYC Required** — total freedom for decentralized finance.
* 🔐 **Fully Self-Custodial** — own your wallet, own your trades.
* 🌉 **Multi-chain Access** — Solana, TON, EVM supported.
* 📈 **Real Stock Exposure** — trade tokenized TSLA, AAPL, NVDA, and more.
* ⚡ **Gasless Experience** — barrier-free trading, optimized for usability.

---

## 📌 Roadmap

* [x] Support RWA Stock trading
* [x] Cross-chain deposits (EVM, Solana)
* [x] Leverage long/short engine
* [ ] Governance DAO & tokenomics
* [ ] Mobile UI
* [ ] Integration with more RWA providers

---

## 🤝 Join Us

* 💬 Telegram: [@TstocksProtocol](https://t.me/+rt8g7-XJc_Y1YjU9)
* 🐦 Twitter: [@TstocksPro](https://twitter.com/TstocksPro)
* 🌐 Website: [https://tstocks.pro](https://tstocks.pro)

---

## 📄 License

MIT © Tstocks Contributors
