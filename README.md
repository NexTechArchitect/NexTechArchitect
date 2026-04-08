<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a5f,100:0f172a&height=120&section=header&text=NexTechArchitect&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35" width="100%"/>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=3000&pause=1000&color=60a5fa&center=true&vCenter=true&width=600&lines=Smart+Contract+%26+Web3+Engineer;DeFi+%7C+Account+Abstraction+%7C+Cross-Chain;Every+concept+shipped+as+production+code." alt="Typing SVG" />
</div>

<br/>

---

## About

Smart Contract & Web3 Engineer based in India. Building since 2024 — focused on DeFi infrastructure, account abstraction, and cross-chain systems.

Every project starts from raw EIP specs, not tutorials. Every contract is invariant-tested before deployment. Every system ships with a production frontend.

**Stack:** Solidity · Foundry · ERC-4337 · Chainlink CCIP · Next.js 14 · Wagmi v2 
 
---

## Flagship Projects

### [Nexus Perpetuals DEX](https://nexus-protocol-os.vercel.app/)
Fully on-chain perpetuals exchange. No off-chain order book, no trusted operators.

- 50× leverage with isolated and cross-margin modes
- ERC-4337 `NexusPaymaster` — 100% gasless trading
- Chainlink CCIP cross-chain margin with per-trader nonce deduplication
- `PerpsVault.sol` solvency invariant held across 6,400 randomized state mutations

**v1** — Ethereum Sepolia · [Live](https://nexus-protocol-os.vercel.app/) · [Source](https://github.com/NexTechArchitect/Nexus-Protocol-OS)  
**v2** — Polkadot Hub Testnet · Polkadot Solidity Hackathon 2026 · [Live](https://nexus-protocol-v2.vercel.app/) · [Source](https://github.com/NexTechArchitect/nexus-protocol-v2)

--- 

### [Sentinel DAO](https://sentinel-dao-brown.vercel.app/)
Modular governance infrastructure built for adversarial conditions.

- 48H `DAOTimelock` — no instant execution, ever
- `VetoCouncil` + `RageQuit` — minority exit before hostile proposals execute
- `TreasuryYieldStrategy` — idle treasury auto-compounds into Aave V3
- ERC-4337 `SessionKeyModule` — gasless multi-action voting
- 256 tests, zero failures across unit, integration, and fuzz

[Live](https://sentinel-dao-brown.vercel.app/) · [Source](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

---

### [RST Protocol — ERC-5484 Soulbound Reputation](https://rst-reputation-protocol.vercel.app/)
On-chain identity layer using soulbound tokens.

- ERC-5484 SBT with dynamic on-chain SVG medals — zero IPFS dependency
- UUPS upgradeable `ReputationEngine` + intentionally immutable `ReputationToken`
- Score clamped to [0, 1000] via pure `ReputationMath` library — overflow impossible by design
- `ReputationVault` with cooldowns, strict CEI, `nonReentrant` throughout

[Live](https://rst-reputation-protocol.vercel.app/) · [Source](https://github.com/NexTechArchitect/ERC-5484)

---

## Protocol Implementations

| Project | What It Does | Source |
|:---|:---|:---|
| **Decentralized StableCoin** | 200% overcollateralized · Chainlink oracles · 10K+ fuzz sequences | [→](https://github.com/NexTechArchitect/Foundry-Defi-StableCoin) |
| **ERC-4337 Account Abstraction** | `validateUserOp` · custom Paymaster · session keys — from raw spec | [→](https://github.com/NexTechArchitect/ERC4337-Account-Abstraction-Foundry) |
| **UUPS Upgradeable Protocol** | EIP-1967 proxy · atomic V1→V2→V3 migration · `__gap` arrays | [→](https://github.com/NexTechArchitect/uups-protocol-config) |
| **Merkle-712 Airdrop** | O(1) claims · EIP-712 front-run protection · phased vesting | [→](https://github.com/NexTechArchitect/Siso-Merkle-Airdrop) |
| **Provably Fair Raffle** | Chainlink VRF + Automation · CEI · state machine | [→](https://github.com/NexTechArchitect/Raffle-Lottery-Foundry) |
| **SISO ERC-20** | RBAC · Pausable · deployed & verified on Sepolia | [→](https://github.com/NexTechArchitect/SISO-Token-ERC20) |
| **Oracle Crowdfunding** | USD-denominated · Chainlink price feeds · 1e18 precision | [→](https://github.com/NexTechArchitect/FundMe-Contract) |

---

## Open to Work

Looking for a **Smart Contract** or **Web3** role.  
DeFi protocols, infrastructure teams, or anywhere the engineering bar is high.

[![Portfolio](https://img.shields.io/badge/Portfolio-0f172a?style=for-the-badge&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![Resume](https://img.shields.io/badge/Resume-1e293b?style=for-the-badge&logo=googledocs&logoColor=white)](https://raw.githubusercontent.com/NexTechArchitect/web3-resume/main/resume.pdf)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amitthapa181133@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://in.linkedin.com/in/amit-kumar-811a11277)
[![Twitter](https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a5f,100:0f172a&height=80&section=footer" width="100%"/>
</div>
