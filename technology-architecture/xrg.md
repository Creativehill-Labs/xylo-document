---
description: 'XYLO Rights Graph (XRG): A Next-Generation RWA Tokenization Framework'
---

# XRG

## 1. **SRG (XRG) Design Verification and Enhancements**

The Smart Rights Graph (SRG), also known as XRG, is Xylo's proprietary technology designed to fully represent the rights structures of Real-World Assets (RWAs) as on-chain tokens. This framework is engineered to encompass a wide range of assets, from tangible ones like real estate to intangible business rights such as music IP, K-POP group revenues, and casino licenses. The core idea is to construct the asset's rights structure as a hierarchical NFT graph, integrating modules for Digital Identity (DID), real-time royalty streaming, and compliance.

An analysis of SRG's components is as follows:

### **1-1. IP Passport**

This component hashes legal documents, such as property deeds or copyright certificates, and anchors them with a DID signature. The original asset (the IP itself) is certified as a non-transferable entity, preventing forgery and double-spending. This creates a trust anchor connecting the off-chain physical asset or right to its on-chain token.\
&#xNAN;_(e.g., Linking the authentic digital version of a property deed or a music IP contract to a digital wallet.)_

### 1-2. Rights Graph (Hierarchical NFT)  `ERC-6150`

This is a hierarchical structure where a root NFT represents the total rights of an asset, and child NFTs represent subdivided, specific rights. This parent-child relationship enables the on-chain representation of complex rights configurations in a tree format. For example, a property's land (root NFT) can have buildings (child NFTs) under it, or a master IP business right (root NFT) can have regional or media-specific license rights (child NFTs) under it. The `ERC-6150` standard supports these hierarchical relationships, allowing for the on-chain management of tree-structured NFTs. Through this, SRG can build a complete rights map by representing all of an asset's primary and subsidiary rights as NFTs.

### 1-3. Token-Bound Account  `ERC-6551`&#x20;

This technology enables each NFT node to have its own wallet (Account). By implementing `ERC-6551`, a unique smart account is created for each NFT, allowing it to hold other tokens or assets and execute on-chain transactions directly. This effectively grants smart contract wallet functionality to the NFT, enabling each rights node in the SRG to hold and interact with independent modules and tokens. For instance, a rights NFT could hold related contracts or revenue tokens and automatically process settlements. This structure significantly enhances modularity and scalability for each right.

### 1-4. Rentable NFT  `ERC-4907`

For specific rights within the Rights Graph, a rental concept is introduced. The `ERC-4907` standard allows the usage rights of an NFT to be leased for a specific period, with the rights automatically reverting to the owner upon expiration. In SRG, this can be used to lease regional performance licenses for K-POP IP for a limited time or to grant property usage rights to a tenant during a lease period. The lease term and conditions are defined in a smart contract, automating expiration management and providing flexibility in rights utilization while preventing misuse.

### 1-5. Soulbound Asset-Passport  `ERC-5633`

A Soulbound Token is a non-transferable NFT that contains unique attribute information (metadata) about the asset. The SAP in SRG serves to record the proof and properties of the tokenized real-world asset. For a property, this could include the address, GPS coordinates, building registry information, insurance policies, and ESG scores in a JSON-LD format. As Soulbound Tokens cannot be transferred, they remain permanently attached to the asset, serving as a certificate. This allows investors to transparently verify the asset's actual properties through the token and ensures that this information follows the rights, enhancing trust between the physical asset and the token.

### 1-6. Modular Compliance Account  `ERC-7579`

This is a modular smart account, based on the `ERC-7579` standard, that manages transactions and governance for the SRG. It allows various compliance modules to be connected like plugins.

* **Transfer-Gate:** A module that checks for KYC/AML verification and country-specific limits during transactions. It utilizes regulated token standards like `ERC-3643` to automate restrictions, such as limiting transfers to whitelisted investors or enforcing transaction volume caps. `ERC-3643` embeds identity verification and transfer restriction logic into the token itself, making it ideal for tokenizing regulated assets like real estate and securities. This enables SRG-based RWA tokens to operate in a regulation-friendly manner by implementing measures against illicit fund flows at the smart contract level.
* **Governance Module:** Supports on-chain governance voting. For example, in a tokenized property, token holders can vote on important issues like rent increases or collateral changes. This module manages proposal creation, voting periods, and quorum requirements, enabling transparent and decentralized decision-making in asset management.
* **Forced-Transfer Hook:** A function to forcibly freeze or transfer tokens upon a court order or regulatory request. This serves as a hook to accommodate judicial rulings (e.g., seizure, forfeiture) or necessary regulatory actions within the smart contract. When a signature from an authorized entity is provided, this module can be executed to freeze tokens in a specified account or transfer them to another. This addresses legal risks and provides the control mechanisms required by institutional frameworks.

### 1-7. Revenue Oracle & Stream  `ERC-1620`

SRG brings cash flows from assets on-chain in real-time. For example, using Chainlink Functions, daily sales or royalty data can be fetched from external APIs and published on-chain. The Decentralized Oracle Network (DON) verifies and aggregates this data for the smart contract. This published real-time revenue data is then automatically distributed via a streaming protocol like Sablier, which is based on `ERC-1620`. This allows for per-second settlement of token payments. In practice, once daily revenue is reported, a stream is opened to flow the corresponding amount in stablecoins like USDC to investors on a per-second basis. This real-time royalty streaming allows investors to constantly monitor and withdraw their earnings, ensuring transparent and delay-free distribution of cash flows.

### 1-8. License Engine  `ERC-3525`

An engine that manages revenue distribution and transfer for license rights. `ERC-3525` is a Semi-Fungible Token (SFT) standard that allows a single token ID to hold divided values (slots), making it suitable for representing fractional shares of rights. In SRG, this could be used to represent K-POP group revenue rights as 30% and 70% slots, or to express real estate rental income rights in token values corresponding to investment ratios. The License Engine issues these `ERC-3525` tokens to automatically split revenue according to shares and allows for the transfer or trading of partial license rights. This implements the concept of traditional equity stakes as on-chain tokens, achieving both fractional ownership and liquidity.

### 1-9. Compliance / Parametric Cover  `ERC-3643`

Equity tokens issued to investors are created under the `ERC-3643` standard (the regulated token mentioned in the Transfer-Gate section), ensuring only whitelisted, verified investors can own them. If necessary, a forced freeze (e.g., in case of illicit possession) can be executed at the smart contract level to enhance security. Additionally, a Parametric Cover feature is considered, which is a smart contract-based concept that automatically triggers an insurance payout or protective measure under specific conditions. For example, if rental income is not paid for a certain period, the collateral asset could be automatically liquidated to compensate investors. These compliance and cover features ensure that SRG-based tokens come with built-in investor protection mechanisms.
