<div align="center">

# Amit Kumar

### Smart Contract Engineer · DeFi Protocol Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/@itZ__AmiT0-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

Solidity engineer specializing in production-grade DeFi protocol architecture across Base Mainnet and EVM networks. 70+ verified contracts deployed across RWA tokenization, perpetuals DEX, insurance vaults, DAO governance, and keeper automation, zero critical or high-severity Slither findings. Independently architects, builds, and audits complete protocol stacks with threat-modeled security, invariant-proven solvency, and Yul-optimized gas efficiency.

---

## Core Stack

```text
Languages     Solidity 0.8, Yul, EVM Inline Assembly, TypeScript
Security      Foundry Invariant Fuzzing, Slither, Echidna, CEI, SafeERC20
Standards     ERC-20/721/1155, ERC-3643, ERC-4337, ERC-4626, ERC-5484, EIP-712, UUPS
Integrations  Chainlink VRF, CCIP, Price Feeds, Automation, Aave V3, OpenZeppelin
Frontend      Next.js 14/15, Wagmi v2, Viem, RainbowKit, TanStack Query, Tailwind
Tooling       Foundry, Anvil, Tenderly, Basescan, Etherscan, Vercel, CREATE2

```

---

## What I Can Build

* **RWA Tokenization:** ERC-3643 compliance engines, NAV oracles, yield distributors
* **Perpetuals DEX:** On-chain position management, liquidation engines, cross-chain margin via CCIP
* **DeFi Vaults:** ERC-4626 yield routing, Aave integrations, flash-loan resistant governance
* **DAO Infrastructure:** TimelockController, rage-quit modules, anti-flash governance, gasless voting
* **Keeper Networks:** Permissionless automation, ETH bonding, slashing registries
* **Account Abstraction:** ERC-4337 smart accounts, custom paymasters, session keys
* **NFT Systems:** Soulbound tokens (ERC-5484), on-chain SVG art engines, dynamic metadata

---

## Notable Engineering

* **O(1) Swap-Pop Queue:** Keeper Network uses swap-and-pop instead of array shift. Unbounded arrays never degrade performance regardless of queue size.
* **try/catch Gas Griefing Isolation:** ExecutionEngine wraps every external call in try/catch. A malicious job that intentionally reverts cannot block the entire batch or drain keeper gas.
* **Flash-Loan Resistant Governance:** Sentinel DAO enforces `block.number - 1` snapshot voting. Tokens borrowed in the same block carry zero voting weight, eliminating flash-governance attack vectors.
* **15% NAV Circuit Breaker:** RWA oracle automatically halts price reads if NAV drops more than 15% in 24 hours, protecting against flash crashes and oracle manipulation.
* **Vault Solvency Invariant:** `totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` is mathematically preserved across all randomized state mutations.

---

## Currently Open To

Remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure.

---

**[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [Email**](https://www.google.com/search?q=mailto%3Anextech.amit%40gmail.com)
