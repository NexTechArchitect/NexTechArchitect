<div align="center">

# Amit Kumar

### Smart Contract Engineer · DeFi Protocol Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

Solidity engineer specializing in production-grade DeFi protocol architecture across Base Mainnet and EVM networks. Verified contracts live across RWA tokenization, perpetuals DEX, insurance vaults, DAO governance, and keeper automation, with zero critical or high-severity findings on any deployment.

I own the entire stack of a protocol alone: threat-modeling the architecture, writing the contracts, proving solvency with Foundry invariant fuzzing, optimizing gas down to Yul, then building the frontend so people can actually use it. Live protocols are pinned below.

---

## Core Stack

```text
Languages     Solidity 0.8, Yul, Inline Assembly, TypeScript
Security      Foundry Invariant Fuzzing, Slither, CEI, SafeERC20, Access Control
Standards     ERC-20/721, ERC-3643, ERC-4337, ERC-4626, ERC-5484, EIP-712, UUPS
Integrations  Chainlink Price Feeds, VRF, CCIP, Automation, Aave V3, OpenZeppelin
Frontend      Next.js 15, Wagmi v2, Viem, RainbowKit, TanStack Query, Tailwind
Tooling       Foundry, Anvil, Basescan, Tenderly, Vercel, CREATE2
```

---

## What I Can Build

- **RWA Tokenization** · ERC-3643 tokens that carry their own rulebook, so KYC and sanctions checks run inside the transfer itself
- **Perpetuals DEX** · Leveraged perps with liquidation engines, funding rates and oracle-driven mark pricing
- **Yield Vaults** · ERC-4626 vaults that put idle deposits to work in lending markets like Aave V3
- **DAO Infrastructure** · Voting, timelocks, treasury management and exit rights for outvoted minorities
- **Keeper Networks** · Operator networks that fire on-chain jobs on schedule, bonded with real money and slashed for failure
- **Account Abstraction** · ERC-4337 smart accounts and paymasters, so a user can trade without ever holding ETH
- **Upgradeable Systems** · UUPS proxies migrated across versions without corrupting stored balances

---

## Notable Engineering

- **Vault Solvency Invariant** · Liquidity plus locked plus free collateral always equals the vault's real balance, proved across 6,400 randomized state mutations with zero reverts
- **Flash-Loan Resistant Governance** · Snapshot voting at `block.number - 1`, so tokens borrowed inside the same block carry zero voting weight
- **Compliance At Transfer Level** · KYC, sanctions and jurisdiction checks live inside the transfer hook, making a non-compliant transfer impossible rather than discouraged
- **Gas Griefing Isolation** · Every keeper job runs in its own try/catch boundary, so one hostile revert cannot stall the batch or drain the operator
- **Zero-ETH Execution Layer** · The keeper execution engine holds no ETH, removing the attack surface instead of guarding it
- **15% NAV Circuit Breaker** · The RWA oracle halts price reads if net asset value drops more than 15% in 24 hours
- **O(1) Swap-Pop Registries** · Job and asset lists use swap-and-pop instead of array shifting, so gas stays flat however large the queue grows
- **Decimal Normalization** · 8-decimal feeds, 6-decimal USDC and 18-decimal accounting reconciled through one scalar, with a modulo guard against silent precision loss
- **EIP-712 MEV Protection** · Claim signatures bind to a specific sender and chain, so an intercepted proof reverts for anyone else
- **Collision-Safe Upgrades** · Reserved `__gap[50]` slots keep child storage intact across V1 to V3 UUPS migrations

---

## Currently Open To

Remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure.

<div align="center">

**[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)**

</div>
