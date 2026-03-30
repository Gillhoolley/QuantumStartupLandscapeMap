# Multimodal Risk & Utility Audit

Generated: 3/30/2026 America/New_York

Source base: `globe.html` startup dataset plus `analysis/reports/partnership_network_web/report.md`

Dataset reviewed: **100** startup records

## Scope
This audit applies the user's screening lens to the repo's current dataset:
- Maturity Signal: hardware modality plus inferred development stage
- Technical Moat: explicit repo mentions of QEC, noise mitigation, control stack, compiler, or AI-native software
- Commercial Readiness: explicit repo mentions of cloud distribution, enterprise pilots, and end-user signals in materials or pharma
- Supply Chain Risk: HQ jurisdiction plus any repo mention of sovereign cloud or partner platform integration

## Important Limits
- The repo contains **short profiles**, not full diligence memos. Many startups have no disclosed foundry partner, sovereign cloud, or benchmark data in the source set.
- Development stage is **inferred** from the repo's own heuristic patterns and startup profiles, not from company roadmaps or audited revenue disclosures.
- Geopolitical supply risk is a **relative inference for a US-centric VC/commercial buyer**, using HQ jurisdiction and disclosed platform integration only.
- The repo includes a few duplicate or near-duplicate entities, such as `IQM` / `IQM Quantum Computers`, `QuEra` / `QuEra Computing`, and `PhaseCraft` / `Phasecraft`. They are retained because they exist as separate records in the dataset.

## Summary Signals
### Modality mix
| Modality | Count |
|---|---:|
| Software / hardware-agnostic | 39 |
| Unspecified hardware | 12 |
| Photonic | 11 |
| Superconducting | 10 |
| Quantum communications | 5 |
| Trapped ion | 4 |
| Quantum sensing | 4 |
| Neutral atom | 4 |
| Silicon spin | 2 |
| Diamond / NV | 2 |
| Silicon | 2 |
| Electrons on helium | 1 |
| Carbon nanotube | 1 |
| Quantum annealing | 1 |
| Quantum networking | 1 |
| Cat-qubit | 1 |

### Stage mix
| Development stage | Count |
|---|---:|
| NISQ / hybrid utility | 42 |
| Research / pilot hardware | 41 |
| Commercial security utility | 7 |
| Fault-tolerant roadmap | 5 |
| Adjacent utility | 5 |

### Moat and commercial-readiness sparsity
| Signal | Count |
|---|---:|
| No moat signal disclosed in repo | 84 |
| AI layer signal | 9 |
| Control-stack signal | 3 |
| Compiler / architecture signal | 3 |
| Noise-mitigation signal | 1 |
| QEC signal | 1 |
| No benchmark / partner signal in repo | 82 |
| Cloud / platform distribution signal | 12 |
| Enterprise pilots | 3 |
| Materials workflow signal | 3 |
| Enterprise software positioning | 3 |
| Pharma / bio workflow signal | 2 |
| Pharma partner signal | 1 |

## VC Heatmap
Scoring logic:
- `Path to utility` favors full-stack utility posture, platform distribution, enterprise-pilot evidence, and domain workflow fit
- `Supply risk` is reduced by low-risk HQ jurisdictions and disclosed platform or sovereign-cloud integration
- Heat score is a heuristic ratio, not a valuation model

| Rank | Startup | HQ | Utility score | Supply risk | Heat score | Why it screened highest |
|---|---|---|---:|---|---:|---|
| 1 | Quantinuum | United Kingdom | 6.5 | Low | 8.12 | Full-stack trapped-ion posture plus Azure Quantum and enterprise-pilot signals make it the strongest blend of technical depth and commercial path |
| 2 | QunaSys | Japan | 6.0 | Low | 7.50 | Direct materials and pharma utility story with cloud-distribution signal gives it one of the clearest near-term value paths |
| 3 | Pasqal | France | 5.5 | Low | 6.88 | Neutral-atom platform with enterprise-pilot and IBM Quantum Network signals lowers commercialization uncertainty |
| 4 | Q-CTRL | Australia | 4.5 | Low | 5.62 | Control-stack software is one of the strongest moat signals in the repo and it already shows platform distribution through AWS Braket and IBM |
| 5 | Xanadu | Canada | 4.5 | Low | 5.62 | Photonic full-stack positioning plus cloud-provider and ecosystem signals indicate a credible utility path with low jurisdictional friction |

### Near misses
- `D-Wave Quantum`: very strong utility path through annealing and cloud distribution, but the repo shows less differentiated moat detail than Q-CTRL or Xanadu
- `Quandela`: strong cloud-access signal and low-risk French base, with an added OVHcloud sovereignty signal, but end-user evidence is thinner than Pasqal or QunaSys
- `ORCA Computing`: enterprise-pilot signal is positive, but the repo still reads as earlier-stage than the top five
- `SandboxAQ`: screens well on AI-native utility, but it is less directly tied to quantum-compute hardware utility than the top five compute/platform names

## Notable Moat Signals
| Startup | Signal in repo | Audit interpretation |
|---|---|---|
| Riverlane | `Quantum error correction stack` | Strongest explicit QEC signal in the dataset; high strategic value as a fault-tolerance enabler |
| Qedma | `Quantum error mitigation software` | Strongest explicit near-term noise-mitigation signal |
| Q-CTRL | `Quantum control infrastructure software` | Clear control-stack moat below the algorithm layer |
| Quantum Machines | `Hybrid quantum-classical control systems` | Strong control and orchestration signal, but medium jurisdiction risk in this audit |
| ParityQC | `Quantum architecture and compiler co-design` | Strong compiler and hardware-software co-design signal |
| Classiq | `Enterprise quantum software design platform` | Strong compiler/design-layer signal and strong value translation, but medium jurisdiction risk in this audit |

## Commercial Readiness Leaders
| Startup | Commercial signal in repo | Comment |
|---|---|---|
| Quantinuum | `Enterprise Pilots`, `Azure Quantum`, `NVIDIA` | Best combination of enterprise signal and ecosystem reach |
| Pasqal | `Enterprise Pilots`, `IBM Quantum Network` | Strong pilot and channel evidence |
| QunaSys | `Pharma Partners`, `Cloud Providers`, materials workflow | Most explicit vertical-fit signal in the full dataset |
| Q-CTRL | `AWS Braket`, `IBM Quantum` | Strong platform distribution for infrastructure software |
| D-Wave Quantum | `AWS Braket`, `Google Cloud`, `Government Labs` | Broad distribution and public-sector signal support near-term utility |
| Quandela | `OVHcloud`, `European Research Labs` | Best sovereign-cloud signal in the current repo |

## Supply Chain Risk Readout
Low-risk jurisdictions in this audit:
- United States
- Canada
- United Kingdom
- EU states in the dataset
- Australia
- Japan
- Singapore

Medium-risk jurisdictions in this audit:
- Israel
- India
- Brazil
- Saudi Arabia

High-risk jurisdictions in this audit:
- China

Repo-disclosed sovereignty / platform signals:
- `Quandela`: OVHcloud signal
- `Quantinuum`: Azure Quantum
- `Pasqal`: IBM Quantum Network
- `Q-CTRL`: AWS Braket and IBM Quantum
- `QunaSys`: cloud-provider signal
- `Xanadu`: cloud-provider signal
- `D-Wave Quantum`: AWS Braket and Google Cloud

## Appendix: Full 100-Startup Audit
Legend:
- `Stage`: `FT` = fault-tolerant roadmap, `NISQ/Hybrid` = near-term utility / hybrid stack, `Research/Pilot` = earlier hardware track, `Security` = communications or post-quantum utility, `Adjacent` = sensing / non-compute utility
- `Moat`: `QEC`, `Mitigation`, `Control`, `Compiler`, `AI`
- `Commercial`: `Cloud`, `Pilots`, `Pharma`, `Materials`, `Bio`, `EnterpriseSW`

| Startup | HQ | Modality | Stage | Moat | Commercial | Supply risk |
|---|---|---|---|---|---|---|
| 1QBit | Canada | Software | NISQ/Hybrid | - | - | Low |
| Alice & Bob | France | Cat-Qubit | FT | - | - | Low |
| Aliro Quantum | United States | Software | NISQ/Hybrid | - | - | Low |
| Alpine Quantum Technologies | Austria | Trapped Ion | Research/Pilot | - | - | Low |
| Anyon Systems | Canada | Superconducting | Research/Pilot | - | - | Low |
| Atom Computing | United States | Neutral Atom | Research/Pilot | - | - | Low |
| BosonQ PSI | India | Software | NISQ/Hybrid | - | - | Medium |
| Brilliant | United States | Software | Research/Pilot | - | - | Low |
| C12 Quantum Electronics | France | CNT | Research/Pilot | - | - | Low |
| Cambridge Quantum Computing | United Kingdom | Software | NISQ/Hybrid | - | - | Low |
| Classiq | Israel | Software | NISQ/Hybrid | Compiler | Cloud,EnterpriseSW | Medium |
| ColdQuanta Inc | United States | Hardware-Unspec | Research/Pilot | - | - | Low |
| Crypta Labs | United Kingdom | Software | NISQ/Hybrid | - | - | Low |
| Crypto Quantique | United Kingdom | Software | Research/Pilot | - | - | Low |
| Diraq | Australia | Silicon Spin | Research/Pilot | - | - | Low |
| D-Wave Quantum | Canada | Annealing | NISQ/Hybrid | - | Cloud | Low |
| D-Wave Systems | Canada | Superconducting | NISQ/Hybrid | AI | - | Low |
| EeroQ | United States | E-on-He | Research/Pilot | - | - | Low |
| Equal1 | Ireland | Hardware-Unspec | Research/Pilot | - | - | Low |
| EvolutionQ | Canada | Software | NISQ/Hybrid | - | - | Low |
| Guardtime | United States | Software | Research/Pilot | - | - | Low |
| Horizon Quantum | Singapore | Software | NISQ/Hybrid | Compiler,AI | - | Low |
| Horizon Quantum Computing | Singapore | Software | NISQ/Hybrid | - | - | Low |
| HQS Quantum Simulations | Germany | Software | NISQ/Hybrid | - | Materials | Low |
| ID Quantique (company) | Switzerland | Software | Research/Pilot | - | - | Low |
| InfiniQuant | Germany | Software | Research/Pilot | - | - | Low |
| Infleqtion | United States | Quantum Sensing | Adjacent | - | - | Low |
| IonQ | United States | Trapped Ion | NISQ/Hybrid | - | Cloud | Low |
| IQM | Finland | Superconducting | NISQ/Hybrid | AI | - | Low |
| IQM Quantum Computers | Finland | Superconducting | NISQ/Hybrid | - | - | Low |
| ISARA (company) | Canada | Software | NISQ/Hybrid | - | - | Low |
| KETS Quantum Security | United Kingdom | Quantum Comms | Security | - | - | Low |
| Kiutra | Germany | Hardware-Unspec | Research/Pilot | - | - | Low |
| LightSolver | Israel | Software | NISQ/Hybrid | - | - | Medium |
| Menten AI | United States | Software | Research/Pilot | - | Bio | Low |
| Multiverse Computing | Spain | Software | Research/Pilot | AI | - | Low |
| Nomad Atomics | Australia | Quantum Sensing | Adjacent | - | - | Low |
| Nord Quantique | Canada | Superconducting | FT | - | - | Low |
| Nu Quantum | United Kingdom | Networking | Research/Pilot | - | - | Low |
| Optalysys | United Kingdom | Photonic | NISQ/Hybrid | - | - | Low |
| ORCA Computing | United Kingdom | Photonic | Research/Pilot | - | Pilots,Cloud | Low |
| Origin Quantum | China | Superconducting | NISQ/Hybrid | - | - | High |
| Ostendo Technologies | United States | Software | Research/Pilot | - | - | Low |
| Oxford Quantum Circuits | United Kingdom | Superconducting | Research/Pilot | - | - | Low |
| ParityQC | Austria | Software | NISQ/Hybrid | Compiler | - | Low |
| Pasqal | France | Neutral Atom | NISQ/Hybrid | - | Pilots,Cloud | Low |
| PhaseCraft | United Kingdom | Software | NISQ/Hybrid | - | - | Low |
| Phasecraft | United Kingdom | Software | NISQ/Hybrid | - | Materials | Low |
| Photonic | Canada | Photonic | Research/Pilot | - | - | Low |
| planqc | Germany | Neutral Atom | Research/Pilot | - | - | Low |
| Post-Quantum | United Kingdom | Software | NISQ/Hybrid | AI | - | Low |
| Pqshield Ltd | United Kingdom | Software | Research/Pilot | - | - | Low |
| ProteinQure | Canada | Software | Research/Pilot | - | Bio | Low |
| PsiQuantum | United States | Photonic | FT | - | - | Low |
| Qblox | Netherlands | Hardware-Unspec | Research/Pilot | Control | - | Low |
| QC Ware Corp. | United States | Software | NISQ/Hybrid | - | EnterpriseSW | Low |
| Q-CTRL | Australia | Software | NISQ/Hybrid | Control | Cloud | Low |
| Qedma | Israel | Software | NISQ/Hybrid | Mitigation | - | Medium |
| Qilimanjaro Quantum Tech | Spain | Hardware-Unspec | NISQ/Hybrid | - | - | Low |
| Qlm Technology Ltd | United Kingdom | Quantum Sensing | Adjacent | - | - | Low |
| Qnami | Switzerland | Diamond/NV | Adjacent | - | - | Low |
| Qnity | Brazil | Quantum Sensing | Adjacent | - | - | Medium |
| QNu Labs | India | Quantum Comms | Security | - | - | Medium |
| QpiAI | India | Software | NISQ/Hybrid | AI | - | Medium |
| Quandela | France | Photonic | NISQ/Hybrid | - | Cloud | Low+SovCloud |
| Quantasphere | Saudi Arabia | Quantum Comms | Security | - | - | Medium |
| Quantinuum | United Kingdom | Trapped Ion | NISQ/Hybrid | - | Pilots,Cloud | Low |
| Quantum Brilliance | Australia | Diamond/NV | Research/Pilot | - | - | Low |
| Quantum Circuits | United States | Superconducting | NISQ/Hybrid | AI | - | Low |
| Quantum Machines | Israel | Hardware-Unspec | NISQ/Hybrid | Control | - | Medium |
| Quantum Motion | United Kingdom | Silicon Spin | Research/Pilot | - | - | Low |
| Quantum Source | Israel | Photonic | Research/Pilot | - | - | Medium |
| Quantum Xchange | United States | Photonic | Security | - | - | Low |
| QuantWare | Netherlands | Superconducting | Research/Pilot | - | - | Low |
| Qubitekk | United States | Hardware-Unspec | Research/Pilot | - | - | Low |
| QuEra | United States | Hardware-Unspec | FT | - | - | Low |
| QuEra Computing | United States | Neutral Atom | NISQ/Hybrid | - | - | Low |
| QuintessenceLabs | Australia | Software | Security | - | - | Low |
| QuiX | Netherlands | Photonic | Research/Pilot | - | - | Low |
| QunaSys | Japan | Software | NISQ/Hybrid | - | Pharma,Cloud,Materials | Low |
| Qunnect | United States | Quantum Comms | Security | - | - | Low |
| Quobly | France | Silicon | Research/Pilot | - | - | Low |
| QuSecure | United States | Software | Research/Pilot | - | - | Low |
| QxBranch | United States | Software | NISQ/Hybrid | - | - | Low |
| Rigetti Computing | United States | Superconducting | NISQ/Hybrid | - | Cloud | Low |
| Riverlane | United Kingdom | Hardware-Unspec | FT | QEC | - | Low |
| SandboxAQ | United States | Software | NISQ/Hybrid | AI | Cloud | Low |
| SeeQC | Italy | Software | Research/Pilot | - | - | Low |
| SEEQC | United States | Hardware-Unspec | Research/Pilot | - | - | Low |
| Sense Photonics | United States | Photonic | Research/Pilot | - | - | Low |
| Sigma-i | Japan | Software | Research/Pilot | AI | - | Low |
| Silicon Quantum Computing | Australia | Silicon | Research/Pilot | - | - | Low |
| Sparrow Quantum | Denmark | Photonic | Research/Pilot | - | - | Low |
| SpeQtral | Singapore | Quantum Comms | Security | - | - | Low |
| Strangeworks | United States | Hardware-Unspec | NISQ/Hybrid | - | - | Low |
| Terra Quantum | Switzerland | Software | NISQ/Hybrid | - | - | Low |
| UbiQD | United States | Hardware-Unspec | Research/Pilot | - | - | Low |
| Universal Quantum | United Kingdom | Trapped Ion | Research/Pilot | - | - | Low |
| Xanadu | Canada | Photonic | NISQ/Hybrid | - | Cloud | Low |
| Zapata Computing | United States | Software | NISQ/Hybrid | - | EnterpriseSW | Low |
