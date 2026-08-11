```
 ________  ________  ________  _________  ________  ________  ___          
|\   __  \|\   __  \|\   __  \|\___   ___\\   __  \|\   ____\|\  \         
\ \  \|\  \ \  \|\  \ \  \|\  \|___ \  \_\ \  \|\  \ \  \___|\ \  \        
 \ \   ____\ \   _  _\ \  \\\  \   \ \  \ \ \  \\\  \ \  \    \ \  \       
  \ \  \___|\ \  \\  \\ \  \\\  \   \ \  \ \ \  \\\  \ \  \____\ \  \____  
   \ \__\    \ \__\\ _\\ \_______\   \ \__\ \ \_______\ \_______\ \_______\
    \|__|     \|__|\|__|\|_______|    \|__|  \|_______|\|_______|\|_______| 
```

<div align="center">

# Amit Kumar — Smart Contract Engineer

**Building production DeFi infrastructure. Not tutorials. Not forks.**

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/𝕏_@itZ__AmiT0-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

## What I Ship

70+ verified contracts across 6 production protocols. Every one cleared Slither with **0 Critical, 0 High**. Every one went through Foundry invariant fuzzing before touching mainnet.

I own the full stack — architecture, Solidity, security review, invariant suite, and Next.js/Wagmi frontend.

---

## Production Protocols

| Protocol | Network | Stack | Tests |
|---|---|---|---|
| [**Nexus RWA Protocol**](https://nexus-rwa-protocol.vercel.app/) | Base Mainnet | ERC-3643, Chainlink, Merkle Yield | 219+ · Invariant Fuzz |
| [**On-Chain Automation Protocol**](https://on-chain-automation-protocol.vercel.app/) | Base Mainnet | ETH Bonding, Slashing, O(1) Queue | Slither 0 Critical |
| [**Sentinel Insurance Protocol**](https://sentinel-insurance-protocol.vercel.app/) | Base Mainnet | ERC-4626, Aave V3, DAO, ERC-5484 | Slither 0 Critical |
| [**Nexus Perpetuals DEX**](https://nexus-protocol-os.vercel.app/) | Sepolia | ERC-4337, Chainlink CCIP, 50x | 6,400 invariant mutations · 0 reverts |
| [**Sentinel DAO**](https://sentinel-dao-brown.vercel.app/) | Sepolia | TimelockController, Rage-Quit, AA | 256 tests · 0 failures |
| [**RST Reputation Protocol**](https://rst-reputation-protocol.vercel.app/) | Sepolia | ERC-5484, UUPS, On-chain SVG | 4-layer Foundry suite |
| [**Nexus Polkadot DEX**](https://nexus-protocol-v2.vercel.app/) | Polkadot Hub | CCIP, 50x, Binance WebSocket PnL | Invariant proven vault |

---

## Security Track Record

```
Protocols audited internally    →   6
Contracts deployed              →   70+
Slither Critical findings       →   0
Slither High findings           →   0
Invariant violations            →   0
```

Every protocol threat-modeled from scratch. CEI enforced everywhere. ReentrancyGuard on all state-changing external calls. Flash-loan guards, staleness guards, circuit breakers where applicable.

---

## Core Stack

```solidity
Languages     →  Solidity 0.8, Yul, EVM Inline Assembly, TypeScript
Security      →  Foundry Invariant Fuzzing, Slither, Echidna, CEI, SafeERC20
Standards     →  ERC-20/721/1155, ERC-3643, ERC-4337, ERC-4626, ERC-5484, EIP-712, UUPS
Integrations  →  Chainlink VRF · CCIP · Price Feeds · Automation, Aave V3, OpenZeppelin
Frontend      →  Next.js 14/15, Wagmi v2, Viem, RainbowKit, TanStack Query, Tailwind
Tooling       →  Foundry, Anvil, Tenderly, Basescan, Etherscan, Vercel, CREATE2
```

---

## What I Can Build

- **RWA Tokenization** — ERC-3643 compliance engines, NAV oracles, yield distributors
- **Perpetuals DEX** — On-chain position management, liquidation engines, cross-chain margin via CCIP
- **DeFi Vaults** — ERC-4626 yield routing, Aave integrations, flash-loan resistant governance
- **DAO Infrastructure** — TimelockController, rage-quit modules, anti-flash governance, gasless voting
- **Keeper Networks** — Permissionless automation, ETH bonding, slashing registries
- **Account Abstraction** — ERC-4337 smart accounts, custom paymasters, session keys
- **NFT Systems** — Soulbound tokens (ERC-5484), on-chain SVG art engines, dynamic metadata

---

## Notable Engineering

**O(1) Swap-Pop Queue** — Keeper Network uses swap-and-pop instead of array shift. Unbounded arrays never degrade performance regardless of queue size.

**try/catch Gas Griefing Isolation** — ExecutionEngine wraps every external call in try/catch. A malicious job that intentionally reverts cannot block the entire batch or drain keeper gas.

**Flash-Loan Resistant Governance** — Sentinel DAO enforces block.number - 1 snapshot voting. Tokens borrowed in the same block carry zero voting weight, eliminating the flash-governance attack surface.

**15% NAV Circuit Breaker** — RWA oracle automatically halts price reads if NAV drops more than 15% in 24 hours, protecting against flash crashes and oracle manipulation.

**Vault Solvency Invariant** — 128 runs × 50 calls = 6,400 randomized state mutations. `totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` never violated once.

---

## Currently Open To

Remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure. Serious teams building serious things.

`Solidity` `Protocol Architecture` `DeFi` `RWA` `Security` `Remote`

---

<div align="center">

*Zero critical findings. Mainnet deployed. Open to work.*

**[View Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)**

</div>
