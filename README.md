<div align="center">

# Amit Kumar

**Smart Contract Engineer · DeFi Protocol Architect**

[![Portfolio](https://img.shields.io/badge/Portfolio-000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/@itZ__AmiT0-000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/nextech.amit@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

I build DeFi protocols end-to-end — architecture, Solidity, security review, Foundry test suites, and Next.js/Wagmi frontends. Everything I ship goes through invariant fuzzing and Slither before mainnet. Zero critical or high findings across all deployments.

Currently focused on: RWA tokenization, perpetuals infrastructure, and keeper automation.

---

## Production Protocols

**[Nexus RWA Protocol](https://nexus-rwa-protocol.vercel.app/)** — Base Mainnet  
Institutional-grade RWA tokenization. Every ERC-20 transfer intercepted in real-time against an on-chain compliance engine — KYC tiers, OFAC sanctions, jurisdictional rules, zero off-chain dependency. Chainlink-automated Merkle yield distribution at O(1) gas. NAV oracle with autonomous 15% circuit breaker. Stateful invariant fuzzing across 5,000+ randomized sequences.

**[On-Chain Automation Protocol](https://on-chain-automation-protocol.vercel.app/)** — Base Mainnet  
Permissionless keeper network. ETH-bonded operators execute registered jobs and earn rewards. Three slashes trigger permanent autonomous jail. ExecutionEngine wraps every external call in try/catch — a reverting job never blocks the batch queue. O(1) swap-pop active job list, pull-payment treasury.

**[Sentinel Insurance Protocol](https://sentinel-insurance-protocol.vercel.app/)** — Base Mainnet  
ERC-4626 vault routing idle USDC into Aave V3 for continuous LP yield. Flash-loan-resistant DAO enforces block.number-1 snapshot voting — tokens borrowed in the same block carry zero voting weight. Soulbound PolicyNFTs with fully on-chain SVG art, no IPFS dependency.

**[Nexus Perpetuals DEX](https://nexus-protocol-os.vercel.app/)** — Sepolia  
On-chain perps with 50x leverage and zero off-chain dependencies. ERC-4337 smart accounts with custom Paymaster sponsoring 100% of gas. Chainlink oracles with per-asset staleness guards. CCIP cross-chain margin with per-trader nonce deduplication. Vault solvency proven as a mathematical invariant — zero violations across thousands of randomized state mutations.

**[Sentinel DAO](https://sentinel-dao-brown.vercel.app/)** — Sepolia  
Flash-governance resistant DAO infrastructure. 48-hour TimelockController blocks instant execution of hostile proposals. VetoCouncil can cancel malicious votes before they execute. Rage-quit module lets dissenting minorities exit with proportional treasury share before new law takes effect. Aave V3 treasury yield, gasless ERC-4337 voting, spam-resistant proposal guard.

---

## Stack

```
Solidity 0.8   Yul   EVM Inline Assembly   TypeScript

Foundry · Slither · Echidna · Anvil · Tenderly

ERC-20/721/1155 · ERC-3643 · ERC-4337 · ERC-4626 · ERC-5484 · EIP-712 · UUPS

Chainlink VRF · CCIP · Price Feeds · Automation
Aave V3 · OpenZeppelin · IPFS

Next.js 14/15 · Wagmi v2 · Viem · RainbowKit · TanStack Query · Tailwind
```

---

## How I Work

Every protocol starts with threat modeling — I identify attack surfaces before writing a single line. Security patterns are non-negotiable: CEI everywhere, ReentrancyGuard on all external calls, flash-loan guards, staleness checks on every oracle read.

Testing is layered: unit tests for every function path, integration tests for cross-contract flows, fuzz tests for edge cases, and stateful invariant suites that mathematically prove protocol-level properties hold under adversarial conditions.

Gas optimization happens after correctness is proven — Yul inline assembly, packed storage layouts, O(1) data structures replacing unbounded loops.

---

## Open To

Remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure.  
Serious teams building serious things.

---

<div align="center">

[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)

</div>
