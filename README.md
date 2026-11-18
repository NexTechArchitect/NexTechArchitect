<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a5f&height=120&section=header&text=&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=600&lines=Smart+Contract+Engineer;DeFi+Protocol+Architect;Security-First+Builder" alt="Typing SVG" />

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-0f172a?style=for-the-badge&logo=vercel&logoColor=38BDF8)](https://nex-tech-architect-portfolio.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0f172a?style=for-the-badge&logo=linkedin&logoColor=38BDF8)](https://linkedin.com/in/nextech-amit)
[![Email](https://img.shields.io/badge/Email-0f172a?style=for-the-badge&logo=gmail&logoColor=38BDF8)](mailto:nextech.amit@gmail.com)

<br/>

</div>

---

Smart contract engineer based in India, open to remote work.

I build the whole thing: security design, Solidity contracts, tests, mainnet deployment, and the frontend on top. Six protocols live on Base Mainnet right now. Zero critical or high severity findings across all of them.

The work I find most interesting is the security layer. Not bolt-on guards, not patching after an incident. Designing the system so certain attacks are structurally impossible. If someone can drain the vault by borrowing tokens for one block, that is a governance design problem, not a missing require statement.

---

## What I work with

```solidity
// Writing contracts in
Solidity 0.8.24, Yul, EVM Assembly, TypeScript, JavaScript

// Testing and auditing with
Foundry (unit, fuzz, stateful invariant tests), Slither, Echidna

// Token standards I have shipped
ERC-20, ERC-721, ERC-1155, ERC-4626 (vaults), ERC-3643 (compliance tokens),
ERC-4337 (account abstraction), ERC-5484 (soulbound), EIP-712, UUPS proxies

// Protocols and infrastructure
Chainlink price feeds, automation, CCIP, VRF — Aave V3 — OpenZeppelin

// Frontend stack
Next.js 14/15, Wagmi v2, Viem, RainbowKit, TanStack Query v5, Tailwind CSS
```

Deployed on Base Mainnet, Ethereum Sepolia, and Polkadot Hub.

---

## What I have built

**Compliance token system for real-world assets**
Institutions need to issue regulated assets like treasury bills or bonds as tokens, but those tokens cannot legally land in the wrong wallet. KYC checks, sanction lists, investor accreditation tiers, and country restrictions all run inside the token transfer itself. There is no approval server to bypass or shut down. The rule is the contract. [[Live](https://nexus-rwa-protocol.vercel.app/)] [[Code](https://github.com/NexTechArchitect/Nexus-RWA-Protocol)]

**Decentralized keeper network**
Any smart contract that needs time-sensitive work done (liquidations, yield compounding, reward epochs) can register as a job. A network of operators bonds ETH to participate and earns fees for executing jobs correctly. Bad execution gets slashed automatically. Three slashes and the operator is permanently banned, no admin required. [[Live](https://on-chain-automation-protocol.vercel.app/)] [[Code](https://github.com/NexTechArchitect/OnChain-Automation-Protocol)]

**DeFi insurance protocol**
Users deposit USDC to underwrite coverage. While that capital sits idle waiting for claims, it earns yield through Aave V3. Claims go through a 7-day voting window where token holders decide the outcome. The voting system cannot be gamed by borrowing tokens for a single block because votes are counted from the previous block. Each policy is an NFT with artwork generated entirely on-chain, no external servers. [[Live](https://sentinel-insurance-protocol.vercel.app/)] [[Code](https://github.com/NexTechArchitect/Sentinel-Insurance-Protocol)]

**Perpetuals exchange with 50x leverage**
Fully on-chain: pricing, execution, liquidations, settlement. Traders pay zero gas because a custom paymaster sponsors all transactions. Cross-chain margin works through Chainlink CCIP with per-trader nonce tracking to prevent replay attacks. Vault solvency is enforced as a mathematical invariant, not a runtime check. [[Live](https://nexus-protocol-os.vercel.app/)] [[Code](https://github.com/NexTechArchitect/Nexus-Protocol)]

**Attack-resistant DAO**
Every proposal sits in a 48-hour timelock before execution. If a hostile proposal passes, minority members can exit and withdraw their proportional share of the treasury before the new rule takes effect. Flash-loan governance attacks are closed by design: borrowed tokens carry zero voting weight. Idle treasury routes into Aave V3 automatically. [[Live](https://sentinel-dao-brown.vercel.app/)] [[Code](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)]

**Perpetuals engine on Polkadot**
Same architecture as the Ethereum version, ported and deployed on Polkadot Hub for the Polkadot Solidity Hackathon 2026. [[Live](https://nexus-protocol-v2.vercel.app/)] [[Code](https://github.com/NexTechArchitect/nexus-protocol-v2)]

---

## A few things I think about when designing systems

**Attacks should be structurally impossible, not just guarded against.**
Sentinel DAO reads voting weight from the previous block. A flash loan that borrows and returns tokens in one transaction contributes zero votes. The attack vector does not exist, not because there is a check, but because the timing makes it meaningless.

**The compliance layer belongs inside the token, not outside it.**
An off-chain approval gate can be bypassed, shut down, or replaced. KYC, sanctions, and jurisdiction rules running inside `_update()` cannot. A non-compliant transfer simply cannot happen.

**Vault accounting should be an invariant, not an assumption.**
The perpetuals vault runs a Foundry stateful fuzz suite that throws hundreds of randomized deposit, trade, and liquidation sequences at the accounting logic before anything ships. If the numbers ever stop adding up, the test fails and the code does not go out.

**Automation that fails silently is worse than no automation.**
The RWA oracle trips a circuit breaker if NAV drops more than 15% in 24 hours and requires a human to reset it. Automated systems should not quietly resume after a crash.

---

## Open to

Remote protocol engineering, smart contract security review, or Web3 infrastructure roles.

<div align="center">

<br/>

[Portfolio](https://nex-tech-architect-portfolio.vercel.app/) &nbsp;&nbsp; [LinkedIn](https://linkedin.com/in/nextech-amit) &nbsp;&nbsp; [nextech.amit@gmail.com](mailto:nextech.amit@gmail.com)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a5f,100:0f172a&height=80&section=footer" width="100%"/>

</div>
