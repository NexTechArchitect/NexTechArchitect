<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0055FF,50:0d9488,100:059669&height=130&section=header&text=NexTechArchitect&fontSize=38&fontColor=ffffff&animation=twinkling&fontAlignY=30" width="100%"/>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=21&duration=2800&pause=1000&color=0d9488&center=true&vCenter=true&width=750&lines=Smart+Contract+%26+Full-Stack+Web3+Engineer;ERC-4337+%7C+Chainlink+CCIP+%7C+DeFi+Protocols;Perpetuals+%7C+DAOs+%7C+Stablecoins+%7C+Proxies;Building+protocols+that+survive+the+dark+forest." alt="Typing SVG" />

  <br/><br/>

  <a href="https://nex-tech-architect-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-nex--tech--architect--portfolio.vercel.app-0d9488?style=for-the-badge&labelColor=0d1117" />
  </a>

</div>

---

## About Me

I'm **Amit** — a Smart Contract & Full-Stack Web3 Engineer from India.

I didn't start as a developer. I came into Web3 in **2019** the way most people do — as a user trying to understand what was actually happening on-chain. That curiosity turned into something deeper: reading whitepapers late at night, breaking down exploit post-mortems, trying to understand exactly why protocols fail the way they do. By **2024** I had enough foundation to start building, and I haven't stopped since.

Since then I've shipped across DeFi, DAOs, NFT infrastructure, stablecoins, account abstraction, and cross-chain systems — not as exercises, but as real deployed protocols with frontends people can actually open. Two of them are live on Vercel right now.

The way I think about engineering:

- **Security is not a feature.** CEI patterns, reentrancy guards, and access control go in on line one — not after someone finds a bug.
- **Gas is user experience.** Every `SLOAD`, every loop, every storage write is a conscious decision.
- **Tests are proof, not metrics.** Invariant fuzzing over 10,000+ randomized transactions tells me more than any coverage report ever could.

I care about building things that are correct — not just things that work most of the time.

<br/>

<p align="center">
  <img src="https://img.shields.io/badge/Web3_Since-2019-0d9488?style=flat-square&labelColor=0d1117" />
  &nbsp;
  <img src="https://img.shields.io/badge/Building_Since-2024-0055FF?style=flat-square&labelColor=0d1117" />
  &nbsp;
  <img src="https://img.shields.io/badge/Projects_Built-15+-059669?style=flat-square&labelColor=0d1117" />
  &nbsp;
  <img src="https://img.shields.io/badge/Contracts_Deployed-60+-F0B90B?style=flat-square&labelColor=0d1117" />
  &nbsp;
  <img src="https://img.shields.io/badge/Tests_Written-256,_Zero_Failures-e0aaff?style=flat-square&labelColor=0d1117" />
</p>

---

## Technical Stack

<div align="center">

### Blockchain Core
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![Foundry](https://img.shields.io/badge/Foundry-BE5212?style=for-the-badge&logo=rust&logoColor=white)
![OpenZeppelin](https://img.shields.io/badge/OpenZeppelin-4E5EE4?style=for-the-badge&logo=openzeppelin&logoColor=white)
![Chainlink](https://img.shields.io/badge/Chainlink-375BD2?style=for-the-badge&logo=chainlink&logoColor=white)

### Full-Stack Web3
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_14-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Wagmi](https://img.shields.io/badge/Wagmi_v2-1C1C1C?style=for-the-badge&logo=ethereum&logoColor=white)
![Viem](https://img.shields.io/badge/Viem-FFC517?style=for-the-badge&logo=ethereum&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

### Security & Testing
![Invariant Fuzzing](https://img.shields.io/badge/Invariant_Fuzzing-FF4500?style=for-the-badge&logoColor=white)
![Slither](https://img.shields.io/badge/Slither-181717?style=for-the-badge&logo=python&logoColor=white)
![ERC-4337](https://img.shields.io/badge/ERC--4337_AA-AA00FF?style=for-the-badge&logo=ethereum&logoColor=white)
![Chainlink CCIP](https://img.shields.io/badge/Chainlink_CCIP-375BD2?style=for-the-badge&logo=chainlink&logoColor=white)

</div>

---

## Flagship Projects

<table width="100%">
<tr>
<td width="50%" valign="top">

### [Nexus Perpetuals DEX](https://nexus-protocol-os.vercel.app/)
**Fully on-chain perp exchange — zero off-chain dependencies**

50× leverage, ERC-4337 gasless trading via `NexusPaymaster`, Chainlink CCIP cross-chain margin with per-trader nonce deduplication, and an invariant-tested vault that held solvency across 6,400 randomized state mutations.

[![Launch App](https://img.shields.io/badge/Launch_App-F0B90B?style=for-the-badge)](https://nexus-protocol-os.vercel.app/)
[![Source](https://img.shields.io/badge/Source_Code-181717?style=flat-square&logo=github)](https://github.com/NexTechArchitect/Nexus-Protocol-OS)

</td>
<td width="50%" valign="top">

### [Sentinel DAO](https://sentinel-dao-brown.vercel.app/)
**Modular governance OS — 256 tests, zero failures**

48H timelock, `RageQuit` minority exit protection, Aave V3 idle treasury yield, and an ERC-4337 AA layer with session keys for gasless voting. Next.js 14 dashboard — zero backend, all state read directly from chain.

[![Launch DAO](https://img.shields.io/badge/Launch_DAO-e0aaff?style=for-the-badge)](https://sentinel-dao-brown.vercel.app/)
[![Source](https://img.shields.io/badge/Source_Code-181717?style=flat-square&logo=github)](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

</td>
</tr>
</table>

---

## Core Protocol Implementations

> Each built from raw EIP specs — not tutorials. Every repo is tested, documented, and deployable.

| Protocol | What It Is | Key Engineering |
|:---|:---|:---|
| [**Merkle-712 Airdrop**](https://github.com/NexTechArchitect/Siso-Merkle-Airdrop) | Gas-optimized token distribution | O(1) claim cost · EIP-712 typed sigs · front-run protection |
| [**Decentralized StableCoin**](https://github.com/NexTechArchitect/Foundry-Defi-StableCoin) | USD-pegged overcollateralized system | 200% collateral ratio · Chainlink oracles · 10K+ tx fuzz suite |
| [**ERC-4337 Account Abstraction**](https://github.com/NexTechArchitect/ERC4337-Account-Abstraction-Foundry) | Smart wallet infrastructure from spec | EntryPoint validation · Custom Paymaster · Session keys |
| [**UUPS Upgradeable Protocol**](https://github.com/NexTechArchitect/uups-protocol-config) | Storage-safe proxy system | EIP-1967 slots · Atomic V1→V2→V3 migration · `__gap` arrays |
| [**Provably Fair Raffle**](https://github.com/NexTechArchitect/Raffle-Lottery-Foundry) | Autonomous on-chain lottery | Chainlink VRF + Automation · CEI pattern · State machine |
| [**SISO Token**](https://github.com/NexTechArchitect/SISO-Token-ERC20) | Production ERC-20 primitive | RBAC · Pausable circuit breaker · Deployed & verified on Sepolia |
| [**CuteCat NFT**](https://github.com/NexTechArchitect/FOUNDRY-Basic-and-Mood-Nft) | ERC-721 with IPFS provenance | Split-stack architecture · Immutable metadata · Admin controls |
| [**Oracle Crowdfunding**](https://github.com/NexTechArchitect/FundMe-Contract) | USD-denominated funding dApp | Chainlink price feeds · 1e18 precision math · Gas optimized |

---

## Engineering Metrics

<div align="center">

<img src="https://github-readme-streak-stats-eight.vercel.app?user=NexTechArchitect&theme=tokyonight&hide_border=true&background=0D1117&ring=0d9488&fire=0055FF&currStreakNum=0d9488&sideNums=0d9488&currStreakLabel=0d9488&dates=FFFFFF" alt="GitHub Streak" />

<br/><br/>

<img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=NexTechArchitect&layout=compact&hide_border=true&bg_color=0D1117&title_color=0d9488&text_color=ffffff&langs_count=6&hide=html,css" alt="Top Languages" />

</div>

---

## Open to Opportunities

I'm looking for my first full-time Web3 role — ideally somewhere I can go deep on protocol design, contribute to a real codebase, and keep pushing on both the contract and frontend sides of the stack.

I'm not looking for a place to learn the basics. I'm looking for a team that builds seriously and cares about getting the details right. If that sounds like your team, I'd genuinely like to talk.

<div align="center">

[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amitthapa181133@gmail.com)
[![Twitter](https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/itZ_AmiT0)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/NexTechDev)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/NexTechArchitect)

</div>

---

<div align="center">

*"Building protocols that survive the dark forest."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:059669,50:0d9488,100:0055FF&height=100&section=footer" width="100%"/>

</div>
