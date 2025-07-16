# House of Voi: Permissionless Gambling Protocol

> **Note**: This documentation is a work in progress. We're building House of Voi iteratively, and content will evolve based on community feedback, TestNet insights, and new learnings. Join us to shape the future!

## 1. Introduction

### 1.1 What is House of Voi?

House of Voi (HoV) is a revolutionary permissionless gambling protocol that empowers players and liquidity providers to truly "own the House." By leveraging immutable smart contracts and community-backed liquidity pools, HoV eliminates the opacity and centralization of traditional casinos. Players wager directly against provably fair, on-chain game logic, while liquidity providers (LPs) supply capital and earn sustainable yields from the house edge. This creates a transparent, permissionless ecosystem where fairness is coded in, not promised.

At its core, HoV combines the thrill of classic casino games—like slots, dice, roulette, and more—with crypto-native innovations. It's not just gambling; it's a composable infrastructure that anyone can build upon, integrate, or participate in as a player, LP, or developer.

### 1.2 Why Now?

The online gambling market is exploding, projected to reach approximately $88 billion in 2025, driven by smartphone proliferation, regional legalizations, and digital innovation. Simultaneously, global cryptocurrency adoption has surged to over 860 million users, fueled by clearer regulations and mainstream integration. These trends converge at a pivotal moment: Traditional platforms remain plagued by custodial risks, black-box algorithms, and exploitative loyalty systems, while crypto offers the tools for reinvention.

House of Voi bridges this gap, arriving as blockchain infrastructure matures to support seamless, scalable applications. Yet, we prioritize user experience above all—abstracting away complexities like wallets, gas fees, and chain interactions. The result? A sleek, intuitive interface that rivals top Web2 casinos, but with on-chain transparency and real ownership. HoV isn't limited to crypto enthusiasts; it's built for every gambler seeking provable fairness, instant payouts, and community-driven rewards. Plus, with built-in responsible gaming features—like self-exclusion tools and wager limits—we ensure a safe, enjoyable environment for all.

### 1.3 What Sets House of Voi Apart?

House of Voi stands out in a crowded landscape by addressing core pain points with innovative, permissionless solutions. Here's how we compare.

<Callout type="info">
#### Compared to Centralized Casinos
- **Non-custodial funds**: Users retain full control, eliminating platform risks and ensuring true ownership.
- **Transparent math**: Every outcome is verifiable on-chain, building trust through code, not claims.
- **Immutable contracts**: No hidden changes or manipulations. Rules are fixed and auditable forever.
- **Shared ownership**: Players and LPs earn directly from the ecosystem, democratizing the house edge.
</Callout>

<Callout type="info">
#### Compared to Other Crypto Casinos
- **Per-game liquidity vaults**: Yields flow to LPs, not opaque treasuries, fostering a community-driven economy.
- **Burn-to-status loyalty**: Sustainable incentives beyond volatile farming, rewarding commitment over speculation.
- **UX abstraction**: Web2 simplicity with on-chain power, plus responsible features like spending alerts.
- **Composability**: Open for integrations, such as DeFi yields, NFT cosmetics, or custom tournaments.
</Callout>

These advantages position HoV as the go-to protocol for fair, engaging, and extensible on-chain gaming.

## 2. System Architecture

### 2.1 Immutable Game Contracts

Each game in HoV is deployed as a standalone, non-upgradeable smart contract, ensuring eternal transparency and security. There are no admin keys or backdoors. Once live, the rules are set in stone. Key parameters like Return-to-Player (RTP) rates, volatility profiles, and core logic are fixed at deployment, verifiable by anyone on the blockchain.

### 2.2 Liquidity Pools

HoV's permissionless model relies on per-game liquidity vaults, where community LPs deposit capital to back wagers. LPs dynamically set max bet limits based on pool depth and earn a share of the house edge, creating a self-sustaining economy. Withdrawals are instant and permissionless, with no lockups, fostering trust and participation.

### 2.3 Frontend Interface

Our non-custodial frontend abstracts all blockchain intricacies, delivering a Web2-like experience: seamless onboarding, one-click betting, and real-time results without ever exposing users to gas or wallet prompts. Operated by a licensed entity, it handles KYC, compliance, and user support while earning a fixed portion of the house edge. All actions route directly to on-chain contracts, maintaining permissionless integrity.

### 2.4 Game Flow Summary

1. Players wager into a game contract using supported assets.
2. Outcomes and payouts are computed verifiably on-chain.
3. The house edge is split between LPs (e.g., 80%) and the frontend operator (e.g., 20%).
4. Active participants earn $HoV tokens proportional to wagering volume, fueling the loyalty ecosystem.

This flow ensures efficiency, fairness, and minimal friction, with optional integrations for advanced users like custom bots or DeFi composability.

## 3. Token Design: $HoV

### 3.1 Purpose

$HoV serves as the native utility token powering HoV's loyalty and incentive engine. It integrates seamlessly with gameplay, enabling:

- Loyalty tier progression through burns.
- Enhanced yields via RTP boosts.
- Eligibility for progressive jackpots.
- Meta-governance for protocol decisions, such as game additions or parameter tweaks.

As a utility asset, $HoV rewards engagement without interfering with core game math or LP yields.

### 3.2 How It Works

- **Earn**: Accumulate $HoV through wagering (e.g., 4 tokens per $1 bet, adjustable for game volatility).
- **Burn**: Commit $HoV to unlock and maintain loyalty tiers, creating deflationary pressure.
- **Status Perks**: Higher tiers grant RTP boosts and jackpot tickets, incentivizing long-term play.
- **Trade**: $HoV is fully transferable on mainnet; testnet version (tHoV) is non-transferable for fair testing.

### 3.3 Loyalty Tier System

| Tier     | Burn to Unlock | Quarterly Burn | RTP Boost | Jackpot Tickets/Month |
| -------- | -------------- | -------------- | --------- | --------------------- |
| Silver   | 10,000 $HoV    | 2,500 $HoV     | +0.25%    | 2                     |
| Gold     | 50,000 $HoV    | 10,000 $HoV    | +0.50%    | 15                    |
| Platinum | 200,000 $HoV   | 25,000 $HoV    | +1.00%    | 65                    |
| Diamond  | 1,000,000 $HoV | 100,000 $HoV   | +1.25%    | 300                   |

Tiers last up to 12 months but require quarterly burns to prevent decay, ensuring ongoing commitment.

### 3.4 Jackpot System

HoV features a monthly progressive jackpot with a 25% payout probability. It rolls over for bigger prizes if untouched. Funded by protocol revenue (e.g., house edge shares or token buybacks), it's accessible only to active status holders. Tickets are allocated based on burned $HoV plus tier bonuses, adding excitement without altering base RTP.

### 3.5 Tokenomics

- **Total Supply**: 1,000,000,000 $HoV (fixed, deflationary via burns).
- **Distribution**:

| Category                     | Percentage | Notes                                                                                   |
| ---------------------------- | ---------- | --------------------------------------------------------------------------------------- |
| Core Contributors & Advisors | 20%        | Vested over 4 years with 1-year cliff; includes pro-rata shares for pre-TGE supporters. |
| Community Incentives         | 10%        | For airdrops, TestNet participants, and early adopters.                                 |
| Protocol Incentives          | 50%        | Emitted via wagering; tapers over time to preserve value.                               |
| Liquidity Mining             | 10%        | For LP rewards and DEX seeding.                                                         |
| Ecosystem Development        | 10%        | DAO-governed for expansions, partnerships, and growth.                                  |

Emissions prioritize active users, with burns acting as long-term sinks to support scarcity.

## 4. Testnet & Launch Strategy

### 4.1 tHoV System

The Testnet uses non-transferable tHoV tokens, distributed via faucets and simulated gameplay. Participation qualifies users for mainnet airdrops, gated by KYC to ensure Sybil resistance and fair distribution.

### 4.2 Launch Objectives

- Drive engagement with gamified leaderboards and reward incentives.
- Stress-test contracts, validate math, and gather feedback.
- Build a vetted community of KYC-ready users for sustainable growth.
- Incorporate responsible gaming metrics during testing to refine features like spending alerts.

## 5. Compliance Strategy

HoV's core protocol remains fully permissionless and immutable, operating without central control. The frontend, managed by a licensed entity, oversees KYC, AML compliance, and user protections. We explore flexible jurisdictions like Curacao or Anjouan for launch, with geo-fencing and self-exclusion tools to promote responsible play. This hybrid model balances innovation with regulatory adherence, adapting as global standards evolve.

## 6. Team

House of Voi is led by Christopher Swenor, a seasoned entrepreneur and blockchain innovator with over 25 years of experience in software development, product acceleration, and launching funded ventures. Starting his career as a developer in 2000, Swenor has founded and scaled multiple companies, many of which have been successfully acquired, demonstrating his ability to build value in competitive tech landscapes.

Swenor's blockchain expertise includes founding Voi Network in 2023, a high-performance, community-owned Layer 1 blockchain built on Algorand Virtual Machine (AVM) technology. He co-founded Reach Platform in 2021, a tool that simplifies smart contract development for Web3 builders; Humble Decentralized Exchange (Humble DeFi) in 2022, which merged with Pact Finance in 2024 to become a leading DEX on Algorand and Voi; and playAlloy in 2024, a gaming-blockchain project acquired shortly before launch. Earlier, he founded East Coast Product in 2015, a product accelerator later acquired, and served as CTO at Vsnap from 2018 to 2021, overseeing its acquisition by Gainsight.

From 2018 to 2020, Swenor was a Technologist in Residence at Harvard Business School, advising on emerging technologies and mentoring in blockchain-business intersections. Known for his collaborative leadership and ability to bridge technical and non-technical worlds, Swenor is actively expanding the HoV team with specialists in smart contracts, regulatory compliance, and user experience to realize the protocol's full potential.

## 6. Vision & Mission

### Vision

Turn the tables. Own the House.

Envision a world where casinos are open protocols. Transparent, extensible, and collectively owned. Anyone can contribute liquidity, build games, or simply play with confidence.

### Mission

To pioneer the permissionless future of gambling: User-owned liquidity, immutable logic, and provably fair experiences that reward participation while prioritizing safety and innovation.

## 7. Conclusion

House of Voi redefines on-chain gaming as a collaborative stack: From immutable contracts and LP yields to $HoV-driven loyalty and progressive jackpots, every element empowers participants. With a focus on seamless UX, ethical design, and community governance, HoV isn't just a protocol. It's the foundation for a fairer, more exciting gambling era. Join us in flipping the House.

## Disclaimer

This document contains preliminary information about House of Voi and is subject to change. All details, including tokenomics, features, and timelines, are conceptual and may be modified as the project evolves.
