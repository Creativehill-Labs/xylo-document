# Blockchain & Smart contract

## 1. Overview

Xylo adopts a hybrid blockchain architecture that combines a private blockchain for internal operations and a public blockchain for external trading. This model enables us to optimize for transparency, security, liquidity, and scalability.

* **Private Blockchain:** Handles asset tokenization, subscription management, and regulatory compliance.
* **Public Blockchain:** Supports global liquidity by allowing RWA tokens to be traded freely on CEXs, DEXs, and DeFi platforms.

Through this dual-layered system, Xylo aims to establish a new financial paradigm where real-world assets become globally accessible and tradeable.

***

## 2. Blockchain Structure

### 2-1. Private Blockchain

Used for RWA asset evaluation, subscription, token issuance, and investor data management.

Key Features:

* **Reliable Data Recording:** Tracks all subscription, asset valuation, and allocation details.
* **Speed & Security:** Operates on a permissioned network for fast and secure transactions.
* **Regulatory Compatibility:** Auditors and evaluators have controlled access for legal oversight.

### 2-2. Public Blockchain

Enhances liquidity by allowing tokenized assets to move freely in global markets.

Key Features:

* **Exchange Compatibility:** Supports trading on CEXs and DEXs.
* **DeFi Integration:** Enables staking, lending, and liquidity provisioning.
* **Transparency:** Global investors can verify token holdings and transaction history on-chain.

### 2-3. Bridge Between Blockchains

A bridge system facilitates secure transfer of tokens between private and public chains.

* Smart contracts validate token issuance before mirroring them 1:1 on external blockchains.
* Security is reinforced with MPC (Multi-Party Computation) and Multi-Sig signature requirements.

***

## 3. Smart Contract System

Core Modules

### 3-1. RWA Subscription & Allocation

* Executes when users convert XLT into XUSD to join Launchpad offerings.
* Automates investment allocation and records every step on-chain.

### 3-2. RWA Token Minting

* Triggered after asset evaluation and verification.
* Tokens are first created on the private blockchain and then bridged to public networks.

### 3-3. XLT-XUSD Conversion & Burn

* XLT is burned when converted to XUSD, while XUSD is minted at a 1:1 ratio.
* The entire process is managed by smart contracts for transparency and auditability.

### 3-4. Bridge Smart Contracts

* Ensures 1:1 token mapping between internal and external chains.
* Includes anti-double-spend mechanisms via multi-signature verification.

***

## 4. Security & Integrity Mechanisms

### 4-1. MPC & Multi-Sig

* **MPC:** Distributes key storage across multiple parties, preventing single-point failures.
* **Multi-Sig:** Requires multiple approvals before executing sensitive transactions.

<figure><img src="../.gitbook/assets/Frame 1000004594.png" alt=""><figcaption></figcaption></figure>

### 4-2. On-Chain Data Integrity (Private Chain)

* All key processes (valuation, subscription, allocation) are monitored by trusted institutions.
* Regulatory agencies can review the records if necessary.

### 4-3. Decentralized Data Storage

* Uses IPFS and distributed ledger technology for storing critical external blockchain data.
* Ensures long-term durability and audit readiness.

<table><thead><tr><th width="209.5999755859375">Pillar</th><th>Trad-Fi System</th><th>Our Hybrid Blockchain</th></tr></thead><tbody><tr><td><strong>Transparency</strong></td><td>Centralized control over records</td><td>All transactions recorded on the blockchain</td></tr><tr><td><strong>Liquidity</strong></td><td>Low liquidity of physical assets</td><td>Global tradability after RWA tokenization</td></tr><tr><td><strong>Security</strong></td><td>High risk due to reliance on single-server infrastructure</td><td>Enhanced security via MPC and Multi-Sig protocols</td></tr><tr><td><strong>Accessibility</strong></td><td>Limited to qualified or institutional investors</td><td>Open to global retail and institutional investors</td></tr><tr><td><strong>Cost Efficiency</strong></td><td>High intermediary and brokerage fees</td><td>Cost reduction via smart contract automation</td></tr></tbody></table>
