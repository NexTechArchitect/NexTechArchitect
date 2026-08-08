<div align="center"> 
 
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E1A,50:00D4AA,100:0088CC&height=140&section=header&text=Amit%20Kumar&fontSize=38&fontColor=E8F0FF&fontAlignY=45&desc=Smart%20Contract%20Engineer%20%C2%B7%20DeFi%20Protocol%20Developer%20%C2%B7%20EVM%20Security&descAlignY=68&descSize=13&descColor=6A8AAA" width="100%" />
 
</div>  
 
&nbsp;

Solidity engineer focused on protocol security and production deployments. I build end-to-end: architecture, contracts, Foundry invariant suites, Slither validation, and Next.js/Wagmi frontends. Zero high-severity findings across 70+ verified contracts on Mainnet and EVM testnets.

Specializing in DeFi protocol architecture across RWA tokenization, perpetuals infrastructure, decentralized insurance, DAO governance, and keeper automation networks.

&nbsp;

---

### Production Deployments

&nbsp;

**[Nexus RWA Protocol](https://basescan.org/address/0x88bb8025dc10Cc642d2F0D10F4335EcDBdC9A594)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Nexus-RWA-Protocol)

`Base Mainnet` `ERC-3643` `Chainlink Automation` `Merkle Yield`

On-chain compliance engine intercepts every ERC-20 transfer in real-time: KYC tier, OFAC sanctions, jurisdictional rules, zero off-chain dependency. Chainlink-automated Merkle yield drops at O(1) gas. NAV oracle with 15% circuit breaker. **6 contracts on Base Mainnet. 219+ tests, stateful invariant fuzzing. Slither: 0 Critical, 0 High.**

&nbsp;

**[On-Chain Automation Protocol (Keeper Network)](https://on-chain-automation-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/OnChain-Automation-Protocol)

`Base Mainnet` `ETH Bonding & Slashing` `Foundry`

Permissionless keeper network where ETH-bonded operators execute jobs and earn rewards. Three slashes trigger autonomous permanent jail. ExecutionEngine wraps every target call in try/catch so reverting jobs never block the batch queue. O(1) swap-pop queue, pull-payment treasury. **3 contracts on Base Mainnet. Slither: 0 Critical, 0 High.**

&nbsp;

**[Sentinel Insurance Protocol](https://sentinel-insurance-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Sentinel-Insurance-Protocol)

`Base Mainnet` `ERC-4626` `Aave V3` `DAO Governance` `ERC-5484`

ERC-4626 vault routes idle USDC into Aave V3 yield. Flash-loan-resistant DAO enforces block.number-1 snapshot voting. Soulbound PolicyNFTs with on-chain SVG. **8 contracts on Base Mainnet. Slither: 0 Critical, 0 High.**

&nbsp;

**[Nexus Perpetuals DEX](https://nexus-protocol-os.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Nexus-Protocol-OS)

`Sepolia` `ERC-4337` `Chainlink CCIP & Oracles`

50x gasless leverage with fully on-chain execution. Chainlink oracles with per-asset staleness guards. CCIP cross-chain margin with per-trader nonce deduplication. Minimum-liquidity burn guards LP inflation. **Zero solvency violations across 6,400 invariant state mutations.**

&nbsp;

**[Sentinel DAO](https://sentinel-dao-brown.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/Web3-FullStack-Sentinal-DAO)

`Sepolia` `TimelockController` `Aave V3 Treasury` `ERC-4337` `Rage-Quit` 

48H TimelockController with VetoCouncil blocks flash-governance attacks. Rage-quit module protects dissenting minorities before hostile execution. Aave V3 treasury yield, gasless voting, spam-resistant proposal guard. **256 tests, zero failures. Treasury solvency fuzz-proved.**

&nbsp;

**[RST Protocol — On-Chain Reputation](https://rst-reputation-protocol.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/RST-Reputation-Protocol)

`Sepolia` `ERC-5484 Soulbound` `UUPS Upgradeable`

ERC-5484 soulbound tokens with 5-tier on-chain SVG medals that auto-upgrade on score change, no re-mint required. UUPS proxy keeps scoring logic upgradeable while SBT ownership records stay immutable.

&nbsp;

**[Nexus Polkadot DEX](https://nexus-protocol-v2.vercel.app/)** &nbsp;·&nbsp; [source](https://github.com/NexTechArchitect/nexus-polka-perps)

`Polkadot Hub Testnet` `Chainlink CCIP` `Polkadot Hackathon 2026`

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
