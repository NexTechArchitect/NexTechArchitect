<div align="center">

# Amit Kumar

### Smart Contract Engineer · DeFi Protocol Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---

Solidity engineer building production DeFi protocols on Base Mainnet and EVM networks. I own the full lifecycle on everything I ship: threat modeling the architecture, writing the contracts, proving solvency with Foundry stateful invariant fuzzing, then building the frontend that makes it usable.

Deployed work spans RWA tokenization, perpetuals, insurance vaults, DAO governance, and keeper automation. Core protocols carry 200+ passing tests each and invariant suites running thousands of randomized state mutations with zero reverts, alongside clean Slither runs (0 critical, 0 high).

**Currently open to** remote roles in DeFi protocol engineering, smart contract security, or Web3 infrastructure.

---

## Live Deployments

Verified contracts with working frontends. Source repos are pinned below.

| Protocol | Focus | Network | Live |
| :--- | :--- | :--- | :---: |
| **Nexus RWA Protocol** | ERC-3643 compliance engine, on-chain KYC/OFAC enforcement, Merkle yield at O(1) gas, NAV circuit breaker | Base Mainnet | [↗](https://nexus-rwa-protocol.vercel.app/) |
| **Sentinel Insurance** | ERC-4626 coverage pool routing idle USDC into Aave V3, flash-loan resistant claim adjudication | Base Mainnet | [↗](https://sentinel-insurance-protocol.vercel.app/) |
| **On-Chain Automation** | Permissionless keeper network, ETH bonding with automated slashing, fault-isolated batch execution | Base Mainnet | [↗](https://on-chain-automation-protocol.vercel.app/) |
| **Nexus Perpetuals DEX** | 50x perps, fully gasless via ERC-4337 paymaster, CCIP cross-chain margin, staleness-guarded feeds | Sepolia | [↗](https://nexus-protocol-os.vercel.app/) |
| **Sentinel DAO** | Modular governance kernel, 48h timelock, Aave V3 treasury yield, gasless voting, minority rage quit | Sepolia | [↗](https://sentinel-dao-brown.vercel.app/) |
| **On-Chain Reputation** | ERC-5484 soulbound scores with dynamic on-chain SVG medals that upgrade without re-minting | Sepolia | [↗](https://rst-reputation-protocol.vercel.app/) |
| **Nexus Perps (Polkadot)** | Non-custodial 50x perps exchange, built for the Polkadot Solidity Hackathon 2026 | Polkadot Hub | [↗](https://nexus-protocol-v2.vercel.app/) |

Also in the repos: an overcollateralized stablecoin engine proved across 10,000+ fuzz sequences, a Merkle + EIP-712 airdrop with MEV-resistant claims, a from-scratch ERC-4337 stack with session keys, and a UUPS V1 to V3 stateful migration study.

---

## Notable Engineering

Specific decisions from the protocols above, and why they were made.

**Vault solvency as a proven invariant.** `totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` holds across 6,400 randomized state mutations with zero reverts. Solvency is verified, not assumed.

**Flash-loan resistant governance.** Sentinel DAO enforces `block.number - 1` snapshot voting, so tokens borrowed inside the same block carry zero weight. Closes the flash-governance attack vector entirely.

**try/catch gas griefing isolation.** The keeper ExecutionEngine wraps every external call in a try/catch boundary. A malicious job that deliberately reverts to trap gas cannot block the batch or drain the keeper.

**Zero-ETH execution layer.** That same ExecutionEngine holds no ETH at all. The attack surface is removed by design rather than defended with access control.

**O(1) swap-pop queues.** Active job and asset lists use swap-and-pop instead of array shifting, so gas cost stays flat no matter how large the queue grows.

**15% NAV circuit breaker.** The RWA oracle halts price reads automatically if NAV falls more than 15% in 24 hours, protecting against flash crashes and oracle manipulation.

**EIP-712 MEV protection.** Airdrop claim signatures bind to a specific `msg.sender` and `chainId`. An intercepted proof reverts when replayed by anyone other than the signed beneficiary.

**Decimal normalization across three scales.** Chainlink feeds return 8 decimals, USDC uses 6, internal accounting runs at 18. `DECIMALS_SCALAR` normalizes everything to 1e18 and withdrawals enforce `scaledAmount % DECIMALS_SCALAR == 0`, eliminating silent precision drain.

**UUPS collision-safe migrations.** `__gap[50]` reserved slots ensure a parent contract upgrade never corrupts child storage layout across V1 to V3.

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

Depth areas: RWA compliance engines, perpetuals and liquidation math, ERC-4626 yield routing, DAO infrastructure, keeper networks, account abstraction and paymasters, and upgradeable proxy migrations. Gas reduced 20 to 35 percent through Yul inline assembly, packed storage layouts, and O(1) data structures.

---

<div align="center">

**[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)**

</div>
