<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a5f&height=120&section=header&text=&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=28&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=600&lines=Smart+Contract+Engineer;DeFi+Protocol+Architect;Security-First+Builder" alt="Typing SVG" />

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-0f172a?style=for-the-badge&logo=vercel&logoColor=38BDF8)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0f172a?style=for-the-badge&logo=linkedin&logoColor=38BDF8)](https://linkedin.com/in/nextech-amit)
[![Email](https://img.shields.io/badge/Email-0f172a?style=for-the-badge&logo=gmail&logoColor=38BDF8)](mailto:nextech.amit@gmail.com)
[![Base Mainnet](https://img.shields.io/badge/Base_Mainnet-0f172a?style=for-the-badge&logo=ethereum&logoColor=38BDF8)](https://basescan.org/)

<br/>

</div>

I build DeFi protocols end to end: threat model, Solidity architecture, Foundry test suite, on-chain deployment, and the frontend users actually touch.

Most of what I ship is not a single contract. It is a system of identity registries, execution engines, NAV oracles, and reward distributors that have to stay consistent with each other while someone is actively trying to break them.

Deployed and source-verified on Base Mainnet. Zero critical or high severity findings across all deployments.

<br/>

## Stack

```solidity
// Languages
Solidity 0.8.24  |  Yul  |  EVM Inline Assembly  |  TypeScript  |  JavaScript

// Security
Foundry (Unit, Fuzz, Stateful Invariant)  |  Slither  |  Echidna  |  CEI  |  SafeERC20

// Standards
ERC-20/721/1155  |  ERC-3643  |  ERC-4337  |  ERC-4626  |  ERC-5484  |  EIP-712  |  UUPS

// Integrations
Chainlink (Price Feeds, Automation, CCIP, VRF)  |  Aave V3  |  OpenZeppelin

// Frontend
Next.js 14/15  |  Wagmi v2  |  Viem  |  RainbowKit  |  TanStack Query v5  |  Tailwind

// Networks
Base Mainnet  |  Ethereum Sepolia  |  Polkadot Hub
```

<br/>

## What I Build

<table>
<tr>
<td width="50%" valign="top">

**🏦 RWA Tokenization**
ERC-3643 compliance engines, KYC and OFAC enforcement inside the transfer hook itself. NAV oracles with autonomous circuit breakers. Merkle yield distribution that costs the same gas for ten holders or a million.

**📈 Perpetuals DEX**
Fully on-chain position lifecycle: open, update, close, liquidate. Cross-chain margin via Chainlink CCIP. ERC-4337 gasless trading with a custom paymaster bound to chain ID and contract address.

**🏛️ DAO Governance**
48-hour timelock on every execution. Rage-quit lets outvoted members withdraw their proportional share before a hostile proposal executes. Flash-loan attacks closed via prior-block snapshot voting.

</td>
<td width="50%" valign="top">

**🔐 DeFi Vaults**
ERC-4626 yield routing into Aave V3. Share-price accounting hardened against inflation attacks. Decimal normalization across 6, 8, and 18 decimal assets.

**⚙️ Keeper Networks**
Permissionless ETH-bonded operators. Three slashes trigger autonomous permanent jailing. Every external call runs in its own try/catch so one bad job cannot block the batch.

**🪪 Account Abstraction**
ERC-4337 smart accounts with session keys. Custom paymasters that sponsor gas while staying replay-proof across chains and contracts.

</td>
</tr>
</table>

<br/>

## Security Patterns I Enforce

**Vault solvency as an invariant**
The perpetuals vault enforces one rule that cannot break: every unit of liquidity, locked collateral, and free trader collateral has to add up exactly to what the token contract reports. This is not an assertion checked at deployment. It is a stateful fuzz invariant that runs against hundreds of randomized deposit, trade, and liquidation sequences before anything ships.

**Flash-loan resistant governance**
Sentinel DAO reads voting weight at `block.number - 1`. Tokens borrowed and returned in a single transaction carry zero votes. The attack is impossible by design, not by policy.

**Compliance at the transfer layer**
ERC-3643 identity, sanctions, and jurisdiction checks run inside `_update()`. A non-compliant transfer cannot exist. There is no off-chain gate to bypass or shut down.

**Gas griefing isolation**
Every external job call in the Keeper Network is wrapped in try/catch. One malicious contract cannot revert the batch or drain keeper gas.

**15% NAV circuit breaker**
The RWA oracle halts autonomously if price drops more than 15% within any 24-hour window. Automated systems do not silently resume after a crash. A human has to reset it.

**O(1) job queue**
Keeper Network uses swap-and-pop removal. No array shifting. Gas cost stays flat regardless of queue depth.

<br/>

## Protocols

<table>
<tr>
<td align="center" width="33%">

**[Nexus RWA Protocol](https://nexus-rwa-protocol.vercel.app/)**
Compliance-enforced RWA tokenization
`ERC-3643` `Chainlink` `Merkle`
🟢 Base Mainnet

</td>
<td align="center" width="33%">

**[On-Chain Automation](https://on-chain-automation-protocol.vercel.app/)**
Permissionless keeper network with slashing
`ETH Bonding` `Fault-isolated`
🟢 Base Mainnet

</td>
<td align="center" width="33%">

**[Sentinel Insurance](https://sentinel-insurance-protocol.vercel.app/)**
DeFi-native coverage with DAO adjudication
`ERC-4626` `Aave V3` `On-chain SVG`
🟢 Base Mainnet

</td>
</tr>
<tr>
<td align="center" width="33%">

**[Nexus Perpetuals](https://nexus-protocol-os.vercel.app/)**
50x leverage, gasless, cross-chain margin
`ERC-4337` `Chainlink CCIP`
🔵 Sepolia

</td>
<td align="center" width="33%">

**[Sentinel DAO](https://sentinel-dao-brown.vercel.app/)**
Attack-resistant treasury governance
`Timelock` `Rage-quit` `Aave V3`
🔵 Sepolia

</td>
<td align="center" width="33%">

**[Nexus Polkadot Perps](https://nexus-protocol-v2.vercel.app/)**
Perpetuals engine, Polkadot Hackathon 2026
`Foundry` `CCIP`
🟣 Polkadot Hub

</td>
</tr>
</table>

<br/>

## Open To

Remote protocol engineering, smart contract security, or Web3 infrastructure roles.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a5f,100:0f172a&height=80&section=footer" width="100%"/>

</div>
