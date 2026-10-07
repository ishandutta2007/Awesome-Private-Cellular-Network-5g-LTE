# Awesome Private Cellular Network (5G & LTE)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

> A curated list of SaaS products, commercial platforms, and open-source GitHub projects for deploying, orchestrating, and testing **Private 5G and LTE Cellular Networks**, self-hosted 5G Cores, and Open RAN (O-RAN) infrastructure.

A comprehensive resource for network engineers, telecom researchers, and enterprises building private wireless networks for industrial IoT, smart campuses, and mission-critical connectivity without relying on public carrier infrastructure.

---

## Table of Contents
- [Market Overview](#market-overview)
- [SaaS & Managed Private Cellular Platforms](#saas--managed-private-cellular-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
  - [Open-Source Standings & Star Badges](#open-source-standings--star-badges)
  - [5G Core Networks](#5g-core-networks)
  - [RAN & gNodeB/eNodeB Implementations](#ran--gnodebenodeb-implementations)
  - [Simulators, Emulators & Testing Tools](#simulators-emulators--testing-tools)
  - [Testbeds & Wireless Research Platforms](#testbeds--wireless-research-platforms)
- [Architecture & Frameworks](#architecture--frameworks)
- [How to Contribute](#how-to-contribute)
- [Disclaimer & Security Considerations](#disclaimer--security-considerations)

---

## Market Overview

The global **Private Cellular Network (5G & LTE) market size** is estimated at **US$ 3.8 Billion to US$ 4.5 Billion** and is projected to reach over **US$ 20 Billion by 2030** with a CAGR exceeding 20%. The market sector is **moderately fragmented**, featuring a dynamic split between mega-cap public cloud & telecom vendors (AWS, Cisco, Nokia, Ericsson, HPE/Athonet) and high-growth specialized startups (Celona, FreedomFi/Nova Labs, Betacom, Druid Software).

---

## SaaS & Managed Private Cellular Platforms

Below are leading commercial and managed private cellular platforms sorted in **descending order by company size** (market valuation or annual corporate revenue).

| Platform / Vendor | Company & Market Size | Starting Tier Price | Free Tier / Trial Limit |
| :--- | :--- | :--- | :--- |
| **[AWS Private 5G](https://aws.amazon.com/private5g/)** | Amazon / AWS<br>*(~$100B+ AWS Rev / $2.3T Corp)* | $10.00 / hour per active Radio Unit (60-day minimum commitment) | AWS Free Tier ($300 credits valid for 30 days) |
| **[Cisco Private 5G](https://www.cisco.com/)** | Cisco Systems<br>*(~$57.0 Billion Annual Rev)* | Custom Enterprise Contract (Starting ~$1,500/month per site) | Custom Enterprise Demo & Managed PoC |
| **[Athonet](https://www.athonet.com/)** | Hewlett Packard Enterprise (HPE)<br>*(~$29.0 Billion HPE Rev)* | Per-SIM / Core License Subscription (Starting ~$1,000/month) | HPE Innovation Lab Demo & Custom Enterprise PoC |
| **[Ericsson Cradlepoint](https://cradlepoint.com/)** | Ericsson<br>*(~$25.0 Billion Annual Rev)* | Cradlepoint NetCloud $250/year per router package | 30-day NetCloud trial with partner hardware |
| **[Nokia Digital Automation Cloud](https://www.nokia.com/)** | Nokia<br>*(~$24.0 Billion Annual Rev)* | Hardware Appliance + SLA License (Starting ~$2,000/month) | Custom Enterprise Proof-of-Concept (PoC) |
| **[Mavenir](https://www.mavenir.com/)** | Mavenir<br>*(~$1.0 Billion Valuation)* | Cloud Core Software Subscription (Starting ~$1,200/month) | Custom Enterprise Demo & Carrier PoC |
| **[FreedomFi](https://www.freedomfi.com/)** | Nova Labs / Helium<br>*(~$300 Million Valuation)* | Hardware Gateway ($499 upfront) + CBRS Radio Cost | No free hardware (Open-source core stack free forever) |
| **[Celona](https://www.celona.io/)** | Celona<br>*(~$270 Million Valuation)* | Subscription bundled per AP (Starting ~$1,200/year per AP) | Celona 5G Airkit & 30-Day Enterprise Evaluation Kit |
| **[Betacom](https://www.betacom.com/)** | Betacom<br>*(~$50 Million Est. Valuation)* | 5G-as-a-Service Managed Subscription (Starting ~$1,800/month) | Custom Enterprise Site Assessment & Demo |
| **[Druid Software](https://www.druidsoftware.com/)** | Druid Software<br>*(~$30 Million Est. Valuation)* | Raemis Core License per gNodeB (Starting ~$800/month) | Custom Partner Sandbox & 14-day Developer PoC |

---

## Open-Source GitHub Projects

Private cellular is one of the most active open-source domains in telecommunications. Complete, production-ready 5G Core and RAN stacks can be deployed on commodity COTS hardware or software-defined radios (SDRs).

### Open-Source Standings & Star Badges

Projects are sorted in **descending order by GitHub star count**. Each badge links directly to the repository's stargazers page.

| Repository | GitHub Star Count Badge | Category / Primary Focus |
| :--- | :---: | :--- |
| **[srsRAN](https://github.com/srsran/srsRAN)** | [![GitHub stars](https://img.shields.io/github/stars/srsran/srsRAN?style=social&color=white)](https://github.com/srsran/srsRAN/stargazers) | Legacy 4G LTE eNodeB & EPC SDR Stack |
| **[Open5GS](https://github.com/open5gs/open5gs)** | [![GitHub stars](https://img.shields.io/github/stars/open5gs/open5gs?style=social&color=white)](https://github.com/open5gs/open5gs/stargazers) | 5G SA Core & 4G EPC (C Implementation) |
| **[free5GC](https://github.com/free5gc/free5gc)** | [![GitHub stars](https://img.shields.io/github/stars/free5gc/free5gc?style=social&color=white)](https://github.com/free5gc/free5gc/stargazers) | 3GPP R15/R16 Cloud-Native 5G Core (Go) |
| **[Magma](https://github.com/magma/magma)** | [![GitHub stars](https://img.shields.io/github/stars/magma/magma?style=social&color=white)](https://github.com/magma/magma/stargazers) | Converged Mobile Core & Federated Gateway |
| **[srsRAN Project](https://github.com/srsran/srsRAN_Project)** | [![GitHub stars](https://img.shields.io/github/stars/srsran/srsRAN_Project?style=social&color=white)](https://github.com/srsran/srsRAN_Project/stargazers) | Commercial-Grade 5G NR CU/DU gNodeB Stack |
| **[UERANSIM](https://github.com/aligungr/UERANSIM)** | [![GitHub stars](https://img.shields.io/github/stars/aligungr/UERANSIM?style=social&color=white)](https://github.com/aligungr/UERANSIM/stargazers) | 5G UE & gNodeB State-Machine Simulator |
| **[docker_open5gs](https://github.com/herlesupreeth/docker_open5gs)** | [![GitHub stars](https://img.shields.io/github/stars/herlesupreeth/docker_open5gs?style=social&color=white)](https://github.com/herlesupreeth/docker_open5gs/stargazers) | Containerized Docker Compose Open5GS Setup |
| **[OMEC UPF](https://github.com/omec-project/upf)** | [![GitHub stars](https://img.shields.io/github/stars/omec-project/upf?style=social&color=white)](https://github.com/omec-project/upf/stargazers) | High-Performance 5G/4G User Plane (ONF SD-Core) |
| **[OpenAirInterface (OAI)](https://github.com/OPENAIRINTERFACE/openairinterface5g)** | [![GitHub stars](https://img.shields.io/github/stars/OPENAIRINTERFACE/openairinterface5g?style=social&color=white)](https://github.com/OPENAIRINTERFACE/openairinterface5g/stargazers) | 3GPP 4G/5G Full Stack (RAN, Core, O-RAN) |
| **[towards5gs-helm](https://github.com/Orange-OpenSource/towards5gs-helm)** | [![GitHub stars](https://img.shields.io/github/stars/Orange-OpenSource/towards5gs-helm?style=social&color=white)](https://github.com/Orange-OpenSource/towards5gs-helm/stargazers) | Helm Charts for 5G Core Deployments on Kubernetes |
| **[Ella Core](https://github.com/ellanetworks/core)** | [![GitHub stars](https://img.shields.io/github/stars/ellanetworks/core?style=social&color=white)](https://github.com/ellanetworks/core/stargazers) | Lightweight eBPF-Powered Enterprise 5G Core |
| **[OCUDU](https://github.com/OCUDU/OCUDU)** | [![GitHub stars](https://img.shields.io/github/stars/OCUDU/OCUDU?style=social&color=white)](https://github.com/OCUDU/OCUDU/stargazers) | Disaggregated O-RAN CU/DU Implementation |
| **[open5gs-operator](https://github.com/Gradiant/open5gs-operator)** | [![GitHub stars](https://img.shields.io/github/stars/Gradiant/open5gs-operator?style=social&color=white)](https://github.com/Gradiant/open5gs-operator/stargazers) | Kubernetes Operator for Automated Open5GS Lifecycle |

---

### 5G Core Networks

- **[Open5GS](https://github.com/open5gs/open5gs)** — The leading open-source 5G core network (AGPL-3.0). Implements complete 5G SA (Standalone) and 4G LTE EPC standards. Capable of running on Raspberry Pi 5 up to high-density x86 servers, achieving over 200 Mbps throughput with ~30ms latency.
- **[Ella Core](https://github.com/ellanetworks/core)** — Production-geared, lightweight 5G core network (Apache-2.0). Features an eBPF-based data plane delivering 5+ Gbps throughput and under 1.5ms latency with minimal hardware requirements (2 CPU cores, 2GB RAM).
- **[free5GC](https://github.com/free5gc/free5gc)** — Cloud-native microservices-based 5G core network implementation in Go (Apache-2.0). Fully compliant with 3GPP Release 15/16 specs.
- **[Magma](https://github.com/magma/magma)** — Open-source mobile core network platform (BSD-3-Clause) managed by the Linux Foundation. Supports LTE EPC and 5G SA with Federation Gateway (FEG) for multi-network orchestration.
- **[ONF SD-Core / OMEC](https://github.com/omec-project/)** — Open-source disaggregated 4G/5G mobile core (Apache-2.0) powering the ONF Aether project. Optimized for cloud-native enterprise edge deployments.

---

### RAN & gNodeB/eNodeB Implementations

- **[srsRAN Project](https://github.com/srsran/srsRAN_Project)** — Commercial-grade open-source 5G RAN stack (AGPL-3.0) featuring a complete 5G NR gNodeB implementation scalable from small boards to enterprise servers.
- **[srsRAN (Legacy 4G/5G)](https://github.com/srsran/srsRAN)** — Classic software-defined radio (SDR) UE and eNodeB/gNodeB suite for 4G LTE and early 5G testing.
- **[OpenAirInterface (OAI)](https://github.com/OPENAIRINTERFACE/openairinterface5g)** — Comprehensive 3GPP cellular platform (CSSL) covering full 4G LTE and 5G NR gNodeB, CU/DU split, and O-RAN Open Fronthaul integrations with DPDK support.
- **[OCUDU](https://github.com/OCUDU/OCUDU)** — Open-source 3GPP F1 interface implementation for Centralized Unit (CU) and Distributed Unit (DU) disaggregation in O-RAN architectures.

---

### Simulators, Emulators & Testing Tools

- **[UERANSIM](https://github.com/aligungr/UERANSIM)** — Open-source 5G UE and gNodeB simulator (GPL-3.0) designed to test 5G core network functions, control plane signaling, and user plane data traffic without physical SDR radios.
- **[docker_open5gs](https://github.com/herlesupreeth/docker_open5gs)** — Ready-to-use Docker and Docker-Compose deployment recipes for Open5GS integrated with UERANSIM and Kamailio IMS for VoNR/VoLTE testing.
- **[towards5gs-helm](https://github.com/Orange-OpenSource/towards5gs-helm)** — Helm charts provided by Orange for orchestrating cloud-native 5G core networks (free5GC, Open5GS) on Kubernetes clusters.
- **[open5gs-operator](https://github.com/Gradiant/open5gs-operator)** — K8s operator for managing full lifecycle deployments of Open5GS NFs on cloud infrastructure.
- **[O-RAN SC (Software Community)](https://o-ran-sc.org/)** — Open-source implementation of Near-Real-Time RAN Intelligent Controller (Near-RT RIC), non-RT RIC, and xApps/rApps for radio resource management.

---

### Testbeds & Wireless Research Platforms

- **[Colosseum](https://www.colosseum.net/)** — World's largest wireless network emulator with SDR devices for AI-driven radio management, 5G/6G, and O-RAN research.
- **[POWDER](https://powderwireless.net/)** — Reconfigurable outdoor wireless testbed at the University of Utah for mobile network research and software-defined network experimentation.
- **[Arena](https://arena.nec-labs.com/)** — Indoor ceiling-grid SDR testbed with 24 synchronized radios and 64 antennas for sub-6 GHz 5G research.
- **[ARA Wireless Living Lab](https://arawireless.org/)** — Real-world wireless living lab for smart agriculture and rural broadband testing, featuring Open5GS integration with commercial RANs.

---

## Architecture & Frameworks

Building custom private 5G/LTE networks typically involves combining components from across the stack:

1. **5G Core Network**: Select **Open5GS** (c-based, maximum performance), **Ella Core** (eBPF-native data plane), **free5GC** (cloud-native Go microservices), or **ONF SD-Core** (enterprise edge).
2. **Radio Access Network (RAN)**: Pair with **srsRAN Project** for performance gNodeB, **OpenAirInterface** for custom sub-6 GHz / O-RAN research, or commercial CBRS gNodeBs (Baicells, Celona, MTI).
3. **Simulation & Validation**: Validate control plane and data paths using **UERANSIM** and **docker_open5gs** before connecting physical hardware.
4. **Cloud & Kubernetes Orchestration**: Deploy via **towards5gs-helm** or **open5gs-operator** for automated scaling and resilience.

---

## How to Contribute

Contributions are welcome! Please follow these guidelines:

1. Fork this repository.
2. Edit `README.md` keeping formatting clean and links valid.
3. Ensure open-source additions include valid GitHub links, proper categorization, and factual descriptions.
4. Open a Pull Request with a short summary of changes.

---

## Disclaimer & Security Considerations

- **Regulatory & Spectrum Compliance**: Private cellular deployments operating in CBRS (Band 48), sub-6 GHz, or mmWave spectrum require compliance with local spectrum allocation rules (e.g., FCC SAS in the US). Always verify radio licensing requirements before transmitting.
- **Network Hardening**: Open-source and enterprise 5G cores must be properly secured. Hardening steps include securing Service-Based Interfaces (SBI), enforcing PFCP authentication, configuring strict NGAP filtering, and preventing null-ciphering NAS fallbacks.
- **Hardware Requirements**: Software radio simulation requires a minimum of 2 CPU cores and 4GB RAM. Production performance deployments handling gigabit traffic require 8+ CPU cores with AVX-512 extensions or hardware DPDK offload.

---

<p center>
  Made for network engineers, telecom researchers, and enterprise IT leaders building sovereign 5G/LTE infrastructure.
</p>
