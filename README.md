<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E1A,50:00D4AA,100:0088CC&height=140&section=header&text=Amit%20Kumar&fontSize=38&fontColor=E8F0FF&fontAlignY=45&desc=Smart%20Contract%20Engineer%20%C2%B7%20DeFi%20Protocol%20Developer%20%C2%B7%20EVM%20Security&descAlignY=68&descSize=13&descColor=6A8AAA" width="100%" />

</div>

&nbsp;

Solidity engineer focused on protocol security and production deployments. I build end-to-end: architecture, contracts, Foundry invariant suites, Slither validation, and Next.js/Wagmi frontends. Zero high-severity findings across 60+ verified contracts on Base Mainnet and EVM testnets.

Core stack: Solidity 0.8 · ERC-4337 · ERC-4626 · Chainlink CCIP · UUPS Proxies · Foundry · Yul

&nbsp;

---

### Production Deployments

&nbsp;

**[On-Chain Automation Protocol (Keeper Network)](https://on-chain-automation-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/OnChain-Automation-Protocol)

`Base Mainnet` `ETH Bonding & Slashing` `Foundry`

Permissionless keeper network where ETH-bonded operators execute jobs and earn rewards. Three slashes trigger autonomous permanent jail. ExecutionEngine wraps every target call in `try/catch` so reverting jobs never block the batch queue. Gas griefing ceiling, O(1) swap-pop queue, pull-payment treasury. **3 contracts on Base Mainnet. Slither: 0 Critical, 0 High.**

&nbsp;

**[Sentinel Insurance Protocol](https://sentinel-insurance-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Sentinel-Insurance-Protocol)

`Base Mainnet` `ERC-4626` `Aave V3` `DAO Governance` `ERC-5484`

ERC-4626 vault routes idle USDC into Aave V3 yield. Flash-loan-resistant DAO enforces `block.number-1` snapshot voting. Soulbound PolicyNFTs with on-chain SVG. **8 contracts on Base Mainnet. Slither: 0 High, 2 medium validated as false positives.**

&nbsp;

**[Nexus Perpetuals DEX](https://nexus-protocol-os.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Nexus-Protocol-OS)

`Sepolia` `ERC-4337` `Chainlink CCIP & Oracles` `5 Isolated Layers`

50x gasless leverage — ERC-4337 paymaster sponsors 100% of gas. Chainlink oracles with per-asset staleness guards. CCIP cross-chain margin with per-trader nonce dedup. Minimum-liquidity burn guards LP inflation. **Zero solvency violations across 6,400 invariant state mutations.**

&nbsp;

**[Sentinel DAO](https://sentinel-dao-brown.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

`Sepolia` `TimelockController` `Aave V3 Treasury` `ERC-4337` `Rage-Quit`

48H TimelockController + VetoCouncil rage-quit blocks flash-governance attacks. Aave V3 treasury yield. ERC-4337 gasless voting. ProposalGuard prevents spam. **256 tests, zero failures. Treasury solvency fuzz-proved.**

&nbsp;

**[RST Protocol — On-Chain Reputation](https://rst-reputation-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/RST-Reputation-Protocol)

`Sepolia` `ERC-5484 Soulbound` `UUPS Upgradeable`

ERC-5484 soulbound tokens with 5-tier on-chain SVG medals that auto-upgrade on score change — no re-mint required. UUPS proxy keeps scoring logic upgradeable while SBT ownership records stay immutable. Score bounded 0–1000, overflow impossible by design.

&nbsp;

**[Nexus Polkadot DEX](https://nexus-protocol-v2.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/nexus-polka-perps)

`Polkadot Hub Testnet` `Chainlink CCIP` `Foundry` `Polkadot Hackathon 2026`

Non-custodial 50x leverage exchange on Polkadot Hub. CCIP cross-chain margin, live Binance WebSocket PnL, invariant-proven vault solvency.

&nbsp;

---

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-00D4FF?style=flat-square&labelColor=0D1220)](https://nex-tech-architect-portfolio.vercel.app/)&nbsp;&nbsp;
[![Resume](https://img.shields.io/badge/Resume-0088CC?style=flat-square&labelColor=0D1220)](https://raw.githubusercontent.com/NexTechArchitect/web3-resume/main/resume.pdf)&nbsp;&nbsp;
[![X](https://img.shields.io/badge/𝕏-@itZ__AmiT0-304860?style=flat-square&labelColor=0D1220)](https://x.com/itZ_AmiT0)&nbsp;&nbsp;
[![Email](https://img.shields.io/badge/Email-304860?style=flat-square&labelColor=0D1220)](mailto:nextech.amit@gmail.com)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0088CC,50:00D4AA,100:0A0E1A&height=80&section=footer" width="100%" />
