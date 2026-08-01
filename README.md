<div align="center">

# 🛡️ SENTINEL DAO
### Institutional Grade Governance Operating System

[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Stack](https://img.shields.io/badge/Full_Stack-Next.js_14_%7C_Foundry-blueviolet.svg)](https://nextjs.org)
[![Network](https://img.shields.io/badge/Network-Sepolia_Testnet-blue.svg)](https://sepolia.etherscan.io/)

<p align="center">
  <br>
  <b>A modular, protocol-level governance infrastructure designed for long-term institutional control.</b><br>
  <i>Engineered with Account Abstraction (ERC-4337), Real-time Treasury Telemetry, and Automated Yield Strategies.</i>
  <br>
</p>

<br>
<a href="https://sentinel-dao-brown.vercel.app/">
  <img src="https://img.shields.io/badge/🔴_LIVE_ACCESS-LAUNCH_SENTINEL_DASHBOARD-000000?style=for-the-badge&logo=vercel&logoColor=white&labelColor=232323&height=50" height="50" />
</a>
<br>
<br>

<p align="center">
  <a href="https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO">💻 View Source Code</a> • 
  <a href="https://github.com/NexTechArchitect/Sentinel-DAO/tree/main/docs">📜 System Documentation</a> • 
  <a href="https://sepolia.etherscan.io/address/0xf4ffd6558454c60E50ef97799C3D69758CB68cf6">🔗 View On-Chain Registry</a>
</p>

</div>

---

### 🦅 Executive Summary

**Sentinel DAO represents a paradigm shift in on-chain organization management.** It is not merely a voting tool; it is **critical infrastructure** designed to survive the adversarial nature of the dark forest. Engineered as a modular 'Operating System' for sovereign capital, Sentinel bridges the gap between rigorous, immutable smart contract security and frictionless user experience. By strictly separating state (Kernel) from logic (Plugins) and integrating a non-custodial **Account Abstraction layer**, it ensures that complex voting strategies never compromise the security of the treasury, while offering a gasless, "Web2-like" experience for stakeholders.

---

## 📑 Table of Contents

1. [🏛️ Architectural Philosophy](#-architectural-philosophy)
2. [✅ Verified Contract Addresses](#-verified-contract-addresses)
3. [🧩 Smart Contract Topology](#-smart-contract-topology)
4. [💻 Frontend Engineering](#-frontend-engineering)
5. [🧪 Testing & Security Vectors](#-testing--security-vectors)
6. [🛠️ Installation & Deployment](#-installation--deployment)

---

## 🏛️ Architectural Philosophy

Sentinel DAO addresses specific failure modes observed in earlier DAO generations (Governance Attacks, Treasury Draining, and Apathy) by enforcing a strict **"Code is Law"** hierarchy.

### Key Invariants:
1.  **Zero Implicit Trust:** The architecture follows a strict separation of concerns. No contract possesses implicit power over another. Even system administrators cannot bypass the **TimelockController**.
2.  **Deterministic Execution:** All state-changing proposals execute exclusively through a Timelock. This creates a transparent, immutable delay window, ensuring no governance decision is applied instantly.
3.  **Governance as an OS:** The system is designed as an Operating System. Modules (Voting Strategies, Yield Engines, Account Abstraction) are "Pluggable," allowing the DAO to upgrade logic without migrating the underlying asset-holding contracts.

---

## ✅ Smart Contract Deployment (Sepolia)

All contracts are deployed and verified on the **Sepolia Testnet**. Click the address to view the contract on Etherscan.

### 🔹 Core & Security Kernel
| Module | Contract Name | Contract Address |
| :--- | :--- | :--- |
| **Kernel** | **DAO Registry (Core)** | [**0xf4ffd...8cf6**](https://sepolia.etherscan.io/address/0xf4ffd6558454c60E50ef97799C3D69758CB68cf6) |
| **Security** | **Timelock Controller** | [**0xC4c57...6FCd**](https://sepolia.etherscan.io/address/0xC4c57946dE2b9b585d05D21423Eee82501466FCd) |
| **Security** | **Role Manager (RBAC)** | [**0xa5720...9d8F**](https://sepolia.etherscan.io/address/0xa5720e4434da10b6c47D8D84542d5a77861A9d8F) |
| **Config** | **DAO Configuration** | [**0x2DE65...6EC1**](https://sepolia.etherscan.io/address/0x2DE65ABEA5dC9C0f18a4975e07E281a2a25C6EC1) |
| **Security** | **Emergency Pause** | [**0x54078...Ba96**](https://sepolia.etherscan.io/address/0x5407869765C92dA9c3B039979170aaBFFaB3Ba96) |

### 🔹 Governance Engine
| Module | Contract Name | Contract Address |
| :--- | :--- | :--- |
| **Gov** | **Hybrid Governor** | [**0x24BC3...CAD3**](https://sepolia.etherscan.io/address/0x24BC3F0e1D0e8732Ce30fbf07EF36beCC9a9CAD3) |
| **Token** | **Governance Token** | [**0x7F787...c1DB**](https://sepolia.etherscan.io/address/0x7F78740d138edEBC17334217b927F5c4D50ec1DB) |
| **Guard** | **Proposal Guard** | [**0xC4015...C3bE**](https://sepolia.etherscan.io/address/0xC4015518192B3f86bF9F27DDeBEd253267D9C3bE) |
| **Veto** | **Veto Council** | [**0x4Abd1...5278**](https://sepolia.etherscan.io/address/0x4Abd12fAED0eabc8cC7825b503EB2B853C8a5278) |
| **Exit** | **Rage Quit Module** | [**0x2c26e...44a2**](https://sepolia.etherscan.io/address/0x2c26e0b0BdA62434aA4e694a767cF2643C7b44a2) |

### 🔹 Financial Treasury
| Module | Contract Name | Contract Address |
| :--- | :--- | :--- |
| **Vault** | **Main Treasury** | [**0xE1131...1A4E**](https://sepolia.etherscan.io/address/0xE113199AE42eF5E9df14a455a67ACC26C8901A4E) |
| **Yield** | **Aave V3 Strategy** | [**0x843ab...b524**](https://sepolia.etherscan.io/address/0x843abAd0B13436b93E7ab71e075bED679586b524) |
| **Grants** | **Quadratic Funding** | [**0xFb045...b198**](https://sepolia.etherscan.io/address/0xFb0455c92908b57c978Fe4B7BE9D1f870B58b198) |

### 🔹 Account Abstraction (ERC-4337)
| Module | Contract Name | Contract Address |
| :--- | :--- | :--- |
| **AA** | **Account Factory** | [**0x7B587...9E96e**](https://sepolia.etherscan.io/address/0x7B587a4A5F571486f4A8dc1bd6aDB745F71fE96e) |
| **AA** | **Gasless Paymaster** | [**0x6927f...E9cD**](https://sepolia.etherscan.io/address/0x6927fc2B44008b5D05611194d47fa3451f9fE9cD) |
| **AA** | **Session Key Module** | [**0xA8F12...95Fa**](https://sepolia.etherscan.io/address/0xA8F129d87Ba978aedFbd40D764445a706dAA95Fa) |
| **Core** | **Entry Point** | [**0x5FF13...2789**](https://sepolia.etherscan.io/address/0x5FF137D4b0FDCD49DcA30c7CF57E578a026d2789) |

---

## 🧩 Smart Contract Topology

The codebase is organized into logical domains, strictly separating **State (Kernel)** from **Logic (Plugins)**.

### 📂 Directory Structure

```bash
src/contracts/
├── core/           # THE KERNEL (Registry, Timelock, Treasury)
├── aa/             # USER ABSTRACTION (ERC-4337 Smart Wallets)
├── governance/     # CONSENSUS LAYER (Voting Logic, Tokens)
├── security/       # DEFENSE SYSTEMS (Pause, Analytics, RBAC)
└── treasury/       # ASSET MANAGEMENT (Yield Strategies)

```

### ⚙️ Module Breakdown

#### 1. The Kernel (Core Execution)

The immutable heart of the protocol. These contracts define the rules of power.

* **`DAOCore.sol`** – **The Registry:** Acts as the central source of truth. It maintains the allowlist of all active modules. If a contract is not registered here, it is not part of the DAO.
* **`DAOTimelock.sol`** – **Execution Gatekeeper:** Enforces a mandatory delay (e.g., 48 hours) on all passed proposals before execution. This strictly prevents "Flash Governance" attacks.
* **`HybridGovernorDynamic.sol`** – **Consensus Engine:** Manages the proposal lifecycle (`Proposed -> Active -> Queued -> Executed`). It supports modular voting strategies based on proposal type.

#### 2. Autonomous Treasury (Financial Engine)

Designed for active capital allocation, not just passive storage.

* **`DAOTreasury.sol`** – **The Vault:** Holds ETH, ERC-20, and NFT assets. Implements a **Pull-Payment Pattern** to prevent reentrancy attacks during fund transfers.
* **`TreasuryYieldStrategy.sol`** – **Yield Optimizer:** A pluggable module that automatically deposits idle treasury assets into **Aave V3** lending pools, generating passive APY for the DAO.

#### 3. Account Abstraction (ERC-4337 Layer)

Removes blockchain complexity to offer a "Web2-like" user experience.

* **`DAOAccountFactory.sol`** – **Smart Wallet Generator:** Deploys deterministic, counterfactual Smart Accounts for users, enabling features like social recovery.
* **`DAOPayMaster.sol`** – **Gas Sponsor:** A protocol-funded contract that subsidizes gas fees, allowing members to vote and propose without holding ETH.
* **`SessionKeyModule.sol`** – **UX Enhancer:** Allows users to sign a single "Session Permission" (valid for X hours). This enables distinct actions (like voting) without repeated wallet popups.

#### 4. Sentinel Security (Defense Mechanisms)

Active protection systems against governance capture and malicious actors.

* **`VetoCouncil.sol`** – **Optimistic Guard:** A multisig of trusted guardians who can cancel malicious proposals (e.g., a 51% attack to drain funds) before they execute.
* **`RageQuit.sol`** – **Minority Protection:** If a hostile proposal passes, dissenting members can burn their governance tokens to withdraw their proportional share of the treasury *before* the new law takes effect.
* **`ProposalGuard.sol`** – **Anti-Spam:** Enforces dynamic thresholds and reputation checks before a user can submit a proposal, preventing Governance Griefing.

---

## 💻 Frontend Engineering

The frontend is built on **Next.js 14 (App Router)**, utilizing a modular provider pattern to manage blockchain state without a centralized backend.

### Technical Stack

* **Framework:** Next.js 14 (TypeScript)
* **State Management:** Wagmi v2 + Viem + TanStack Query
* **Authentication:** RainbowKit (Wallet Connect & Metamask)
* **Styling:** Tailwind CSS + Framer Motion (8K Animations)
* **Infrastructure:** Public RPC Nodes (Zero API Key dependency for resilience)

### Client Architecture

| Directory | Role & Responsibility |
| --- | --- |
| **`app/`** | **Routing & Pages.** distinct modules (`/treasury`, `/proposals`, `/guardian`) using Server Components for performance. |
| **`components/`** | **UI Atoms.** Reusable 8K UI elements. Includes `SessionGuard.tsx` which protects routes based on AA session status. |
| **`hooks/`** | **Business Logic.** Custom React Hooks wrapping Wagmi/Viem: <br>

<br>• `useAASession.ts`: Manages Account Abstraction session keys.<br>

<br>• `useDAOData.ts`: Fetches real-time governance metrics.<br>

<br>• `useProposals.ts`: Handles proposal lifecycle (Submit -> Vote -> Queue). |

---

### Key Methodologies

1. **Unit Tests:** Isolated testing of individual functions (e.g., `test_DepositERC20`) to ensure atomic logic correctness.
2. **Integration Tests:** Validating the complex interaction between modules, ensuring `Timelock` correctly respects `Governor` delays.
3. **Fuzz Testing:**
* `testFuzz_EndToEndChaos`: Simulates random user actions to find edge cases in state transitions.
* `testFuzz_RageQuitMath`: Verified the mathematical solvency of the exit mechanism under various economic conditions.



---

## 🛠️ Installation & Deployment

To run the full stack environment locally:

### 1. Smart Contracts (Foundry)

```bash
# Clone Repo
git clone [https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO.git](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO.git)
cd Web3-FullStack-Sentinal-DAO

# Install Dependencies
forge install

# Run Tests
forge test

```

### 2. Client Application (Next.js)

```bash
cd web3-app

# Install Node Modules
npm install

# Run Development Server
npm run dev

```

Open `http://localhost:3000` to view the Dashboard.

---

<div align="center">
<b>Engineered with ❤️ by <a href="https://github.com/NexTechArchitect">NexTech Architect</a></b>



<a href="https://x.com/itZ_AmiT0">Connect on 𝕏 (Twitter)</a>



<i>Smart Contract Developer · Solidity · Foundry · Full Stack Web3</i>
</div>

```

```
