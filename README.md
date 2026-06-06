# Amit Kumar — Smart Contract Engineer

Solidity engineer shipping production DeFi end to end —
fuzz-tested, Slither-audited, and verified on-chain.
Zero high-severity findings across 40+ contracts.

**Stack:** Solidity · Foundry · EVM · Chainlink · ERC-4337 · Next.js

---

## Featured Projects

### [Sentinel Insurance Protocol](https://sentinel-insurance-protocol.vercel.app/) · [Source](https://github.com/NexTechArchitect/Sentinel-Insurance-Protocol)
`Solidity 0.8.24` `ERC-4626` `Aave V3` `DAO Governance` `ERC-5484` `Base Mainnet`

ERC-4626 vault routes idle USDC into Aave V3 yield. Flash-loan-resistant DAO governance via `getPastVotes(block.number-1)`. Soulbound PolicyNFTs with on-chain SVG metadata.

**8 contracts live on Base Mainnet — Basescan verified — Slither: 0 high / 2 medium validated.**

---

### [Nexus Perpetuals DEX — Gasless 50× Leverage](https://nexus-protocol-os.vercel.app/) · [Source](https://github.com/NexTechArchitect/Nexus-Protocol-OS)
`Solidity` `ERC-4337` `Chainlink CCIP` `Cross-Chain` `Sepolia`

Fully on-chain perpetuals with ERC-4337 paymaster covering 100% of gas. Chainlink oracles with staleness guards, CCIP cross-chain margin with nonce deduplication. `MINIMUM_LIQUIDITY` burn prevents LP inflation attacks.

**Solvency invariant held across 6,400 randomized mutations — zero violations.**

> **v2 on Polkadot Hub** · [Live](https://nexus-protocol-v2.vercel.app/) · [Source](https://github.com/NexTechArchitect/nexus-protocol-v2)

---

### [Sentinel DAO — Anti-Flash Governance](https://sentinel-dao-brown.vercel.app/) · [Source](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)
`Solidity` `TimelockController` `Aave V3 Treasury` `ERC-4337` `Rage-Quit` `Sepolia`

48H `TimelockController` + VetoCouncil rage-quit mechanism blocks flash-loan governance attacks. Aave V3 auto-compounding treasury. ERC-4337 gasless voting removes gas as a participation barrier.

**256 tests — zero failures. Treasury solvency fuzz-proved.**

---

### [RST Protocol — On-Chain Reputation](https://rst-reputation-protocol.vercel.app/) · [Source](https://github.com/NexTechArchitect/ERC-5484)
`Solidity` `ERC-5484 Soulbound` `UUPS Upgradeable` `Sepolia`

ERC-5484 soulbound tokens with 5-tier dynamic SVG medals that auto-upgrade on score change. UUPS proxy pattern keeps scoring logic upgradeable while SBT records stay permanently immutable.

**Overflow and uniqueness fuzz-proved across 4-layer test suite.**

---

## Also on GitHub

| Project | What it does |
|---|---|
| DSC Stablecoin | Overcollateralised stablecoin — 10,000-run invariant fuzz suite |
| UUPS V1→V3 Migration | Live proxy upgrade path with storage-collision-safe layout |
| Merkle + EIP-712 Airdrop | O(1) gas, MEV-resistant claim verification |
| Chainlink VRF Lottery | Provably fair on-chain randomness |
| Dynamic SVG NFTs | Fully on-chain metadata, no IPFS dependency |
| ERC-20 Fundraise | RBAC + circuit breaker pattern |

---

Open to remote Solidity / Smart Contract roles — DeFi protocols, infra, audit-adjacent.
Anywhere the bar is high.

[Portfolio](https://nex-tech-architect-portfolio.vercel.app) · [Resume](https://raw.githubusercontent.com/NexTechArchitect/web3-resume/main/resume.pdf) · [Email](mailto:amitthapa181133@gmail.com) · [LinkedIn](https://in.linkedin.com/in/amit-kumar-811a11277)
