# Process & Secondary Trading

## Token Movement Process Overview

1. Token Issuance and Logging on Internal Blockchain
2. Transfer Request and Validation
3. Bridge or Wrapping Mechanism Activation
4. External Token Minting & Secondary Market Trading
5. On-Chain Monitoring & Data Synchronization

### _Step-by-Step Breakdown_

#### <mark style="background-color:purple;">1. Token Issuance and Logging on Internal Blockchain</mark>

* RWA tokens are initially minted on the internal blockchain.
* All metadata (e.g. ownership, legal status, token supply) is securely stored and validated by internal nodes.
* Immutable by design, the internal ledger ensures full compliance and traceability.

***

#### <mark style="background-color:purple;">2. Transfer Request and Validation</mark>

* Users submit requests to transfer tokens from the internal chain to a public chain.
* Requests can involve single or multiple RWA assets, including cross-asset bundling.

**Validation Includes:**

* KYC/AML checks to ensure regulatory alignment.
* Asset ownership verification to confirm token balances.
* Double-spending prevention through record reconciliation.

***

#### <mark style="background-color:purple;">3. Bridge or Wrapping Mechanism Activation</mark>

**(1) Cross-Chain Bridge:**\
A smart contract-based infrastructure facilitating token migration between private and public chains.

**How it works**\
When a user initiates a transfer, the bridge protocol <mark style="color:purple;">locks the corresponding tokens on the internal blockchain</mark>, ensuring that they cannot be duplicated or reused. Simultaneously, <mark style="color:purple;">an equivalent amount of tokens is minted on the external blockchain</mark>, maintaining a strict 1:1 ratio. Once minted, the user <mark style="color:purple;">receives the new tokens on the external chain</mark>, which can then be freely traded across supported CEXs, DEXs, or DeFi platforms—enabling seamless cross-chain liquidity without compromising asset integrity.

**Tech Features**

* Lock & Mint: Token pairs are cryptographically bound between chains.
* Oracle Integration: Ensures reliable cross-chain data synchronization.

**\[Example]**  \
Ethereum ↔ BNB Chain (Custom-built RWA bridges in development)

**(2) Wrapping Mechanism:**\
A technique to represent internal tokens as wrapped assets on external blockchains.

**How it works**\
When tokens are <mark style="color:purple;">deposited into a smart contract on the internal blockchain</mark>, a <mark style="color:purple;">wrapped token of equal value is minted on the public chain</mark>, preserving the integrity of the underlying asset. These wrapped tokens can then be <mark style="color:purple;">freely traded across public networks</mark>, including CEXs, DEXs, and DeFi protocols. For reverse conversion, a <mark style="color:purple;">burn-and-release mechanism</mark> is applied—burning the wrapped token on the public chain and <mark style="color:purple;">releasing the original token</mark> from the internal chain—ensuring seamless interoperability and trust across both ecosystems.

**\[Example]**\
Wrapped RWA-WETH (Ethereum-compatible RWA token)

***

#### <mark style="background-color:purple;">4. External Token Minting & Secondary Market Trading</mark>

* RWA tokens are registered on CEXs, DEXs, and DeFi platforms.
* Investors can trade, stake, or use tokens as collateral.
* Smart contracts automate dividend payouts, profit sharing, and governance rights.

***

#### <mark style="background-color:purple;">5. On-Chain Monitoring & Data Synchronization</mark>

**Data Sync Mechanism**

* Bridges and oracles verify and synchronize transaction records across chains.
* Full traceability is maintained through smart contracts.

**Audit Capabilities**

* Real-time asset status available to investors and regulators.
* Supports third-party audits and compliance checks.

**Preventing Inconsistencies**

* Ensures no double spending across chains.
* Automated integrity checks between internal and external ledgers.
