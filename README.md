# Amit Kumar

**Smart Contract Engineer · DeFi Protocol Architect**

I build DeFi protocols end to end — threat model, Solidity architecture, Foundry test suite, on-chain deployment, and the frontend users actually touch.

Most of what I ship is not a single contract. It is a system: identity registries, execution engines, NAV oracles, reward distributors — separate contracts that have to stay consistent with each other while someone is actively trying to break them.

Deployed and source-verified on Base Mainnet and EVM testnets. Zero critical or high severity findings across all deployments.

---

## Stack

```
Languages     Solidity 0.8.24, Yul, EVM Inline Assembly, TypeScript, JavaScript
Security      Foundry (Unit · Fuzz · Stateful Invariant), Slither, Echidna, CEI, SafeERC20
Standards     ERC-20/721/1155 · ERC-3643 · ERC-4337 · ERC-4626 · ERC-5484 · EIP-712 · UUPS
Integrations  Chainlink (Price Feeds · Automation · CCIP · VRF) · Aave V3 · OpenZeppelin
Frontend      Next.js 14/15 · Wagmi v2 · Viem · RainbowKit · TanStack Query v5 · Tailwind
Networks      Base Mainnet · Ethereum Sepolia · Polkadot Hub
```

---

## What I Build

**RWA Tokenization** — ERC-3643 compliance engines, KYC and OFAC enforcement inside the transfer hook, NAV oracles with autonomous circuit breakers, Merkle yield distribution at constant gas regardless of holder count.

**Perpetuals DEX** — On-chain position lifecycle, liquidation engines, cross-chain margin via Chainlink CCIP, ERC-4337 gasless trading, fuzz-proven vault solvency invariants.

**DeFi Vaults** — ERC-4626 yield routing into Aave V3, share-price accounting hardened against inflation attacks, decimal normalization across 6, 8, and 18 decimal assets.

**DAO Governance** — TimelockController, rage-quit minority protection, flash-loan resistant snapshot voting, ERC-4337 gasless participation.

**Keeper Networks** — Permissionless automation, ETH bonding and slashing registries, try/catch fault-isolated batch execution, O(1) job queues.

**Account Abstraction** — ERC-4337 smart accounts, custom paymasters bound to chain ID and contract address, session keys, gasless UX flows.

---

## Security Patterns I Enforce

**Vault solvency as an invariant**
`totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` — proved under 6,400 randomized state mutations. Zero reverts.

**Flash-loan resistant governance**
Sentinel DAO reads voting weight at `block.number - 1`. Tokens borrowed and returned in a single transaction carry zero votes. The attack is impossible by design, not by policy.

**Compliance at the transfer layer**
ERC-3643 identity, sanctions, and jurisdiction checks run inside `_update()`. A non-compliant transfer cannot exist. There is no off-chain gate to bypass or shut down.

**try/catch gas griefing isolation**
Every external job call in the Keeper Network is wrapped in try/catch. One malicious contract cannot revert the batch or drain keeper gas.

**15% NAV circuit breaker**
RWA oracle halts autonomously if price drops more than 15% in 24 hours. Automated systems do not silently resume after a crash — a human resets it.

**O(1) job queue**
Keeper Network uses swap-and-pop. No array shifting. Gas cost stays flat regardless of queue depth.

---

## Projects

| Protocol | What it does | Stack | Network |
|---|---|---|---|
| [Nexus RWA Protocol](https://nexus-rwa-protocol.vercel.app/) | Compliance-enforced RWA tokenization | ERC-3643 · Chainlink · Merkle | Base Mainnet |
| [On-Chain Automation](https://on-chain-automation-protocol.vercel.app/) | Permissionless keeper network with slashing | ETH Bonding · Fault-isolated router | Base Mainnet |
| [Sentinel Insurance](https://sentinel-insurance-protocol.vercel.app/) | DeFi-native coverage with DAO adjudication | ERC-4626 · Aave V3 · On-chain SVG | Base Mainnet |
| [Nexus Perpetuals](https://nexus-protocol-os.vercel.app/) | 50x leverage, gasless, cross-chain margin | ERC-4337 · Chainlink CCIP | Sepolia |
| [Sentinel DAO](https://sentinel-dao-brown.vercel.app/) | Attack-resistant treasury governance | Timelock · Rage-quit · Aave V3 | Sepolia |
| [Nexus Polkadot Perps](https://nexus-protocol-v2.vercel.app/) | Perpetuals engine on Polkadot Hub | Foundry · CCIP · MockAggregator | Polkadot Hub |

---

## Open To

Remote protocol engineering, smart contract security, or Web3 infrastructure roles.

[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)
