# Amit Kumar

Solidity engineer. Self-taught. Two years of building DeFi protocols from scratch and shipping them to mainnet.

Not tutorials. Not forks. Original architecture — insurance vaults, perpetuals exchanges, DAO governance systems, on-chain reputation protocols — each one designed for production security from the first line of code.

Zero high-severity findings across 40+ verified contracts.

---

## What I build

**Sentinel Insurance Protocol** — ERC-4626 vault routing idle USDC into Aave V3 yield. Flash-loan-resistant DAO governance using snapshot voting. Soulbound PolicyNFTs with on-chain SVG metadata. Eight contracts live on Base Mainnet, Basescan verified, Slither clean.

[Live](https://sentinel-insurance-protocol.vercel.app) · [Source](https://github.com/NexTechArchitect/Sentinel-Insurance-Protocol)

---

**Nexus Perpetuals DEX** — Fully on-chain 50x leverage perpetuals. ERC-4337 paymaster sponsors 100% of gas, so users never touch ETH. Chainlink oracles with staleness guards. CCIP cross-chain margin with nonce deduplication to prevent replay attacks. Solvency invariant held across 6,400 randomised mutations with zero violations.

[Live](https://nexus-protocol-os.vercel.app) · [Source](https://github.com/NexTechArchitect/Nexus-Protocol-OS) · [v2 on Polkadot Hub](https://nexus-protocol-v2.vercel.app)

---

**Sentinel DAO** — Anti-flash-loan governance. 48H TimelockController plus a VetoCouncil rage-quit mechanism that lets minority holders exit before a hostile proposal executes. Aave V3 auto-compounding treasury. ERC-4337 gasless voting. 256 tests, zero failures.

[Live](https://sentinel-dao-brown.vercel.app) · [Source](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

---

**RST Protocol** — On-chain reputation with ERC-5484 soulbound tokens. Five-tier dynamic SVG medals that auto-upgrade when a user's score crosses a threshold. UUPS proxy keeps scoring logic upgradeable while the SBT records stay permanently immutable. Fuzz-proved against overflow and uniqueness violations.

[Live](https://rst-reputation-protocol.vercel.app) · [Source](https://github.com/NexTechArchitect/ERC-5484)

---

## Also on GitHub

**DSC Stablecoin** — Overcollateralised stablecoin with a 10,000-run invariant fuzz suite proving solvency under adversarial conditions.

**UUPS V1 to V3 Migration** — Live proxy upgrade path with storage-collision-safe layout across three contract versions.

**Merkle + EIP-712 Airdrop** — O(1) gas claim verification with MEV-resistant proof structure.

**Chainlink VRF Lottery** — Provably fair on-chain randomness with no trusted operator.

**Dynamic SVG NFTs** — Fully on-chain metadata. No IPFS dependency, no external rendering.

**ERC-20 Fundraise** — Role-based access control with a circuit breaker pattern for emergency pause.

---

## How I build

Security is not a review step at the end. Threat modeling happens before the first function signature. CEI patterns, reentrancy guards, oracle staleness checks, and flash-loan resistance are architectural decisions, not patches.

Testing means unit tests for correctness and fork tests for reality. A bug I missed on Nexus cross-chain margin only appeared in a fork test — not in 95 passing unit tests. That is the difference between testing your assumptions and testing the actual system.

Storage layout gets designed before implementation on anything upgradeable. Retrofitting UUPS onto an existing contract once cost me more time than writing the contract itself. It never happened again.

---

## Stack

Solidity 0.8 · Foundry · EVM · Yul · Chainlink CCIP, VRF, Price Feeds · Aave V3 · ERC-4337 · UUPS · OpenZeppelin · Slither · Echidna · Next.js 15 · Wagmi · Viem · TypeScript · IPFS

---

Open to remote Solidity and smart contract roles. DeFi protocols, infrastructure, audit-adjacent work. Anywhere the bar is high.

[Portfolio](https://nex-tech-architect-portfolio.vercel.app) · [Resume](https://raw.githubusercontent.com/NexTechArchitect/web3-resume/main/resume.pdf) · [Email](mailto:nextech.amit@gmail.com) · [LinkedIn](https://in.linkedin.com/in/amit-kumar-811a11277)
