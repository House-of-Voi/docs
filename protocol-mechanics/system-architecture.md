# System Architecture

> **Note**: This documentation is a work in progress. We're building House of Voi iteratively, and content will evolve based on community feedback, TestNet insights, and new learnings. Join us to shape the future!

House of Voi’s architecture is designed for transparency, security, and scalability, leveraging immutable smart contracts and decentralized liquidity.

## Components

- **Immutable Game Contracts**: Each game (e.g., dice, slots) is a standalone contract with fixed RTP and logic, no admin keys.
- **Liquidity Pools**: Per-game vaults where LPs provide capital, set bet limits, and earn from the house edge.
- **Frontend Interface**: Non-custodial, licensed for compliance, abstracts blockchain complexity for Web2-level UX.
- **Game Flow**: Wagers go to contracts, outcomes are computed on-chain, edge splits to LPs/frontend, players earn $HoV.

_Content under development—technical specs and diagrams to be added._
