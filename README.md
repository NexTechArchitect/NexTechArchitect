<div align="center">
           
# Amit Kumar
### Smart Contract Engineer · DeFi Protocol Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=vercel&logoColor=white)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/nextech-amit)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nextech.amit@gmail.com)

</div>

---                                                      

I build DeFi protocols end to end: threat model, Solidity architecture, Foundry test suite, on-chain deployment, and the frontend users actually touch.

Most of what I ship is not a single contract. It is a system. Identity registries, execution engines, NAV oracles, reward distributors. Separate contracts that have to stay consistent with each other while someone is actively trying to break them.

Deployed and source-verified on Base Mainnet and EVM networks. Zero critical or high severity findings across all deployments.

---

## Core Stack

```text
Languages     Solidity 0.8, Yul, EVM Inline Assembly, TypeScript
Security      Foundry Invariant Fuzzing, Slither, Echidna, CEI, SafeERC20
Standards     ERC-20/721/1155, ERC-3643, ERC-4337, ERC-4626, ERC-5484, EIP-712, UUPS
Integrations  Chainlink VRF, CCIP, Price Feeds, Automation, Aave V3, OpenZeppelin
Frontend      Next.js 14/15, Wagmi v2, Viem, RainbowKit, TanStack Query, Tailwind
Networks      Base Mainnet, Ethereum Sepolia, Polkadot Hub
```

---

## What I Build

**RWA Tokenization:** ERC-3643 compliance engines, KYC and OFAC enforcement inside the transfer hook, NAV oracles with circuit breakers, Merkle yield distribution at O(1) gas regardless of holder count.

**Perpetuals DEX:** On-chain position lifecycle, liquidation engines, cross-chain margin via Chainlink CCIP, ERC-4337 gasless trading, staleness-guarded price feeds.

**DeFi Vaults:** ERC-4626 yield routing into Aave V3, share-price accounting hardened against inflation attacks, decimal normalization across 6, 8, and 18 decimal assets.

**DAO Governance:** TimelockController, rage-quit minority protection, flash-loan resistant snapshot voting, ERC-4337 gasless participation.

**Keeper Networks:** Permissionless automation, ETH bonding and slashing registries, try/catch fault-isolated batch execution, O(1) job queues.

**Account Abstraction:** ERC-4337 smart accounts, custom paymasters bound to chain ID and contract address, session keys, gasless UX flows.

**NFT Systems:** ERC-5484 soulbound tokens, fully on-chain SVG art engines, dynamic metadata with no IPFS dependency.

**Token Primitives:** EIP-712 MEV-resistant airdrops, Merkle claim systems, overcollateralized stablecoins, Chainlink VRF lotteries, UUPS proxy migrations with storage-collision safety.

---

## Engineering That Matters           

**Vault solvency as an invariant:** `totalLiquidity + totalLockedCollateral + totalTraderFreeCollateral == ASSET.balanceOf(vault)` holds under every sequence of deposits, trades, and liquidations. Proved under 6,400 randomized state mutations. Zero reverts.

**Flash-loan resistant governance:** Sentinel DAO checks `block.number - 1` for voting weight. Tokens borrowed and returned within one transaction carry zero votes. The attack is impossible by design, not by policy.

**Compliance at the transfer layer:** ERC-3643 identity, sanctions, and jurisdiction checks run inside `_update()`. A non-compliant transfer cannot exist. There is no off-chain gate to bypass or shut down.

**Zero-ETH execution engine:** Keeper ExecutionEngine holds no ETH. The attack surface is eliminated at the architecture level, not by access control.

**try/catch gas griefing isolation:** Every external job call is wrapped in try/catch. One malicious contract cannot revert the batch or drain keeper gas.

**15% NAV circuit breaker:** RWA oracle halts automatically if price drops more than 15% in 24 hours. Automated systems do not silently resume after a crash. A human resets it.

**Precision drain prevention:** 8-decimal Chainlink feeds, 6-decimal USDC, and 18-decimal internal accounting reconcile through a single scalar. A modulo guard on every withdrawal blocks silent rounding loss.

**EIP-712 replay protection:** Airdrop claim signatures bind to `msg.sender` and `chainId`. An intercepted proof is useless. The transaction reverts if the caller is not the signed beneficiary.

**O(1) job queue:** Keeper Network uses swap-and-pop. No array shifting. Gas cost stays flat regardless of queue depth.
               
---

## Open To

Remote protocol engineering, smart contract security, or Web3 infrastructure roles.

---

<div align="center">

**[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) · [LinkedIn](https://linkedin.com/in/nextech-amit) · [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)**

</div>
