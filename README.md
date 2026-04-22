# CommitMint 🚀

**Stake. Commit. Mint Habits.**

CommitMint is a decentralized social accountability application built on the **Base** blockchain. It leverages financial incentives and social validation to help users achieve their goals. By combining the transparency of smart contracts with the social fabric of communities, CommitMint turns habit formation into a rewarding, collaborative game.

![CommitMint Hero](./public/hero.png)

## 🌟 Overview

The concept is simple: you create a challenge pool (e.g., "30 Days of Morning Runs") and stake USDC. To win, you must prove your progress daily.

At the core of the system lies a **"Proof and Voting"** mechanism:
1. **Create/Join**: Users stake USDC into a commitment pool.
2. **Submit Proof**: Participants upload video proofs (IPFS/Hash) of their daily activity.
3. **Social Validation**: Pool members watch and vote to verify each other's proofs.
4. **Win Rewards**: Participants who successfully complete the challenge and remain active in voting split the total pot.

## ✨ Key Features

- **Decentralized Staking**: Secure USDC commitment pools on Base Sepolia.
- **Social Accountability**: Peer-to-peer verification ensures authenticity.
- **Game Theory Incentives**: Earn rewards from the stakes of those who didn't follow through.
- **Farcaster Integration**: Built as a Farcaster Mini-App for seamless social distribution.
- **OnchainKit Powered**: Leverages Coinbase's OnchainKit for a premium web3 user experience.

## 🛠️ Technology Stack

- **Blockchain**: Base (Sepolia Testnet)
- **Framework**: Next.js 15+ (App Router)
- **Web3 Libraries**: OnchainKit, Wagmi, Viem
- **Social Integration**: Farcaster Mini-App SDK
- **Styling**: Tailwind CSS, Lucide React
- **Smart Contracts**: Solidity (OpenZeppelin)

## 📜 Smart Contract Logic (`HabitPoolV2`)

The platform is powered by the `HabitPoolV2` contract, which handles:
- **Pool Creation**: Define contribution amounts, duration, and quorum requirements.
- **Participation**: Securely manages USDC deposits using `SafeERC20`.
- **Proof Submission**: Tracks daily video hashes for every participant.
- **Validation Engine**: Implements a quorum-based majority voting system.
- **Automated Settlement**: Calculates winners based on both survival (completing habits) and activity (voting on others).
- **Pull-Pattern Withdrawals**: Securely distribute rewards to verified winners.

**Contract Address (Base Sepolia):** `0xfF4D2De0dE888875c6C1ee1fd7ec5155676bCDCC`

## 🚀 Getting Started

### Prerequisites

- Node.js 20+
- A Farcaster account (for Mini-App integration)
- Base Sepolia ETH and USDC for testing

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/justacoder120/CommitMint.git
   cd CommitMint
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env.local` file based on `.example.env`.

4. **Run the development server:**
   ```bash
   npm run dev
   ```

## 🏆 Hackathon Project

CommitMint was developed for the **Base 101: Build Apps Onchain - Işık Session**

---

Built with ❤️ on [Base](https://base.org) 🔵
