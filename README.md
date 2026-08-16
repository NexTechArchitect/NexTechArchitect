<div align="center">

# Amit Kumar

### Smart Contract Engineer · DeFi Protocol Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

Solidity engineer specializing in production-grade DeFi protocol architecture across Base Mainnet and EVM networks. Verified contracts deployed across RWA tokenization, perpetuals DEX, insurance vaults, DAO governance, and keeper automation, zero critical or high-severity Slither findings. Independently architects, builds, and audits complete protocol stacks with threat-modeled security, invariant-proven solvency, and Yul-optimized gas efficiency

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
- **RWA Tokenization:** ERC-3643 compliance engines, KYC/OFAC on-chain enforcement, NAV oracles, Merkle yield distributors
- **Perpetuals DEX:** On-chain position management, liquidation engines, cross-chain margin via CCIP, EIP-712 MEV-resistant order flow
- **DeFi Vaults:** ERC-4626 yield routing, Aave V3 integrations, flash-loan resistant snapshot governance
- **DAO Infrastructure:** TimelockController, rage-quit modules, anti-flash governance, gasless voting via ERC-4337
- **Keeper Networks:** Permissionless automation, ETH bonding, slashing registries, try/catch fault-isolated batch execution
- **Account Abstraction:** ERC-4337 smart accounts, custom paymasters, session keys, gasless UX flows
- **NFT Systems:** Soulbound tokens (ERC-5484), on-chain SVG art engines, dynamic metadata without IPFS
- **Upgradeability:** UUPS collision-safe proxy migrations, storage gap patterns, atomic V1 to V3 state migrations
- **Token Primitives:** MEV-resistant EIP-712 airdrops, Merkle claim systems, overcollateralized stablecoins, VRF lotteries
---

## Notable Engineering
- **O(1) Swap-Pop Queue:** Keeper Network uses swap-and-pop instead of array shift. Unbounded arrays never degrade performance regardless of queue size.
- **try/catch Gas Griefing Isolation:** ExecutionEngine wraps every external call in try/catch. A malicious job that intentionally reverts cannot block the entire batch or drain keeper gas.
- **Flash-Loan Resistant Governance:** Sentinel DAO enforces `block.number - 1` snapshot voting. Tokens borrowed in the same block carry zero voting weight, eliminating flash-governance attack vectors.
- **15% NAV Circuit Breaker:** RWA oracle automatically halts price reads if NAV drops more than 15% in 24 hours, protecting against flash crashes and oracle manipulation.
- **Vault Solvency Invariant:** `totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` is mathematically preserved across all randomized state mutations.
- **UUPS Collision-Safe Migrations:** Storage gap pattern with `__gap[50]` arrays ensures parent contract upgrades never corrupt child storage layout across V1 to V3 migrations.
- **EIP-712 MEV Protection:** Airdrop claim signatures bind to specific `msg.sender` and `chainId`. An intercepted proof cannot be replayed, the transaction reverts if caller is not the signed beneficiary.
- **Zero-ETH Execution Layer:** Keeper ExecutionEngine holds absolutely no ETH. Attack surface is eliminated by design, not by access control.
---

## Currently Open To

Remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure.

--- 

<div align="center">

**[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)**

</div>
