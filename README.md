<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0055FF,50:0d9488,100:059669&height=130&section=header&text=NexTechArchitect&fontSize=38&fontColor=ffffff&animation=twinkling&fontAlignY=30" width="100%"/>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=2800&pause=1000&color=0d9488&center=true&vCenter=true&width=700&lines=Smart+Contract+%26+Full-Stack+Web3+Engineer;ERC-4337+%7C+Chainlink+CCIP+%7C+DeFi+Protocols;Building+protocols+that+survive+the+dark+forest." alt="Typing SVG" />
</div>

<br/>

<p align="center">
  <a href="https://nex-tech-architect-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/🌐_Portfolio-Live_Site-0d9488?style=for-the-badge&labelColor=0d1117" />
  </a>
  &nbsp;
  <a href="mailto:amitthapa181133@gmail.com">
    <img src="https://img.shields.io/badge/📧_Email-Hire_Me-0055FF?style=for-the-badge&labelColor=0d1117" />
  </a>
  &nbsp;
  <a href="https://x.com/itZ_AmiT0">
    <img src="https://img.shields.io/badge/𝕏_Twitter-@itZ__AmiT0-181717?style=for-the-badge&labelColor=0d1117" />
  </a>
  &nbsp;
  <a href="https://t.me/NexTechDev">
    <img src="https://img.shields.io/badge/💬_Telegram-NexTechDev-26A5E4?style=for-the-badge&labelColor=0d1117" />
  </a>
</p>

---

## 👋 About Me

I'm a **Smart Contract & Full-Stack Web3 Engineer** based in India. Been in the Web3 space since **2019** as a user — started building in **2024** and haven't stopped since.

I focus on three things: **getting the logic right**, **keeping gas low**, and **not breaking in edge cases**. Security and clean architecture aren't optional — they're the baseline.

Currently building full-stack dApps that real users can open and use — not just contract repos on GitHub. Strong Solidity foundations on the backend, Next.js + Wagmi on the frontend.

**What I've shipped:**
- ⚡ **15+ projects** built across DeFi, NFTs, DAOs, and infrastructure
- 🔗 **60+ contracts** deployed on EVM testnets
- 🏗️ **2 production-grade full-stack dApps** live on Vercel
- 🛡️ **256 tests written** with zero failures on flagship DAO project

---

## 🛠️ Technical Stack

<div align="center">

### ⛓️ Blockchain Core
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![Foundry](https://img.shields.io/badge/Foundry-BE5212?style=for-the-badge&logo=rust&logoColor=white)
![OpenZeppelin](https://img.shields.io/badge/OpenZeppelin-4E5EE4?style=for-the-badge&logo=openzeppelin&logoColor=white)
![Chainlink](https://img.shields.io/badge/Chainlink-375BD2?style=for-the-badge&logo=chainlink&logoColor=white)

### 🌐 Full-Stack Web3
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Wagmi](https://img.shields.io/badge/Wagmi_v2-1C1C1C?style=for-the-badge&logo=ethereum&logoColor=white)
![Viem](https://img.shields.io/badge/Viem-FFC517?style=for-the-badge&logo=ethereum&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

### 🛡️ Security & Testing
![Slither](https://img.shields.io/badge/Slither-181717?style=for-the-badge&logo=python&logoColor=white)
![Invariant Fuzzing](https://img.shields.io/badge/Invariant_Fuzzing-FF4500?style=for-the-badge&logo=target&logoColor=white)
![ERC-4337](https://img.shields.io/badge/ERC--4337-AA00FF?style=for-the-badge&logo=ethereum&logoColor=white)

</div>

---

## 🏆 Flagship Projects

<table width="100%">
<tr>
<td width="50%" valign="top">

### ⚡ Nexus Perpetuals DEX
**On-chain perp exchange — zero off-chain dependencies**

A fully on-chain perpetuals protocol with **50× leverage**, no centralized matching engine, and no custodial bridge. Every price fetch, liquidation, and settlement runs on-chain.

**Key Engineering:**
- `PerpsVault.sol` — 18-decimal precision, dual accounting (free vs locked collateral), LP inflation attack prevention
- `LiquidationEngine.sol` — Isolated and cross-margin modes, keeper-compatible batch liquidations
- **ERC-4337 SmartAccount** — Gasless trading via NexusPaymaster; `paymasterAndData` chain + contract bound to prevent replay
- **Chainlink CCIP** — Cross-chain margin relay with per-trader nonce deduplication
- **Invariant suite** — 6,400 state mutations, zero vault solvency violations

[![Launch App](https://img.shields.io/badge/🚀_Launch_App-nexus--protocol--os.vercel.app-F0B90B?style=for-the-badge)](https://nexus-protocol-os.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat-square&logo=github)](https://github.com/NexTechArchitect/Nexus-Protocol-OS)

</td>
<td width="50%" valign="top">

### 🏛️ Sentinel DAO
**Institutional-grade governance OS — 256 tests, zero failures**

A modular on-chain governance system built as an Operating System for sovereign capital. Strictly separates State (Kernel) from Logic (Plugins) so modules can be upgraded without migrating treasury assets.

**Key Engineering:**
- `DAOTimelock.sol` — 48H mandatory delay, prevents flash governance attacks
- `VetoCouncil.sol` + `RageQuit.sol` — Active minority protection before hostile proposals execute
- `TreasuryYieldStrategy.sol` — Idle assets auto-deposited into Aave V3
- **ERC-4337 AA layer** — `SessionKeyModule` eliminates repeated wallet popups; `DAOPaymaster` sponsors gas
- **Next.js 14 Dashboard** — Zero-backend, all reads direct from chain via Wagmi v2 + Viem

[![Launch DAO](https://img.shields.io/badge/🏛️_Launch_DAO-sentinel--dao.vercel.app-e0aaff?style=for-the-badge)](https://sentinel-dao-brown.vercel.app/)
[![Source Code](https://img.shields.io/badge/Source_Code-181717?style=flat-square&logo=github)](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

</td>
</tr>
</table>

---

## 🔬 Core Protocol Implementations

> Deep dives into Ethereum standards. Each built from the raw EIP spec — not from tutorials.

| Protocol | What It Demonstrates | Repo |
|:---|:---|:---:|
| **Merkle-712 Airdrop** | O(1) gas distribution for 1M+ users. Off-chain Merkle tree + EIP-712 typed signatures to block front-running claim theft | [↗](https://github.com/NexTechArchitect/Siso-Merkle-Airdrop) |
| **Decentralized StableCoin Engine** | Over-collateralized (200%) USD-pegged token. Chainlink oracle feeds, dynamic liquidation engine with 10% keeper incentive, stateful fuzz invariants over 10K+ tx sequences | [↗](https://github.com/NexTechArchitect/Foundry-Defi-StableCoin) |
| **ERC-4337 Account Abstraction** | EntryPoint validation flow, custom Paymaster gas sponsorship, Session Key delegation — built from spec, no SDK | [↗](https://github.com/NexTechArchitect/ERC4337-Account-Abstraction-Foundry) |
| **UUPS Upgradeable Protocol** | EIP-1822 proxy pattern, collision-proof ERC-1967 storage slots, atomic V1→V2→V3 state migrations, `__gap` arrays | [↗](https://github.com/NexTechArchitect/uups-protocol-config) |
| **Automated Provably Fair Raffle** | Chainlink VRF for tamper-proof randomness + Chainlink Automation for self-execution. State machine: `OPEN → CALCULATING → OPEN` with reentrancy prevention via CEI | [↗](https://github.com/NexTechArchitect/Raffle-Lottery-Foundry) |
| **SISO Token (ERC-20)** | RBAC, Pausable circuit breaker, deflationary burn mechanics, CI/CD-ready deployment scripts. Deployed & verified on Sepolia | [↗](https://github.com/NexTechArchitect/SISO-Token-ERC20) |
| **CuteCat NFT (ERC-721)** | IPFS split-stack architecture, decentralized asset provenance, admin governance controls, MetaMask & OpenSea-compatible URI formatting | [↗](https://github.com/NexTechArchitect/FOUNDRY-Basic-and-Mood-Nft) |
| **Oracle-Pegged Crowdfunding** | USD-denominated funding thresholds on ETH. 1e18 precision math via Chainlink aggregators, gas optimization: `constant`, `immutable`, custom errors, memory-cached loops | [↗](https://github.com/NexTechArchitect/FundMe-Contract) |

---

## 📊 Engineering Metrics

<div align="center">

<img src="https://github-readme-streak-stats-eight.vercel.app?user=NexTechArchitect&theme=tokyonight&hide_border=true&background=0D1117&ring=0d9488&fire=0055FF&currStreakNum=0d9488&sideNums=0d9488&currStreakLabel=0d9488&dates=FFFFFF" alt="GitHub Streak" />

<br/><br/>

<img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=NexTechArchitect&layout=compact&hide_border=true&bg_color=0D1117&title_color=0d9488&text_color=ffffff&langs_count=6&hide=html,css" alt="Top Languages" />

</div>

---

## 🤝 Open to Opportunities

I'm actively looking for my **first full-time Web3 role** — Smart Contract Engineer, Full-Stack Web3 Dev, or Protocol Engineer.

Happy to discuss protocol design, contribute to an existing codebase, or build something new from scratch.

<div align="center">

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-nex--tech--architect--portfolio.vercel.app-0d9488?style=for-the-badge)](https://nex-tech-architect-portfolio.vercel.app/)
[![Email](https://img.shields.io/badge/📧_Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amitthapa181133@gmail.com)
[![Twitter](https://img.shields.io/badge/𝕏_Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Telegram](https://img.shields.io/badge/💬_Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/NexTechDev)

</div>

---

<div align="center">

*"Building protocols that survive the dark forest."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:059669,50:0d9488,100:0055FF&height=100&section=footer" width="100%"/>

</div>
