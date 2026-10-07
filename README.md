# Awesome-Private-Cellular-Network-5g-LTE

# Top Private Cellular Network (5G/LTE) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Private 5G/LTE Deployments, Open-Source RAN & Self-Hosted Core Networks*  
**Last updated: October 2026**

This repository tracks notable **commercial private cellular platforms** and **open-source projects** that enable organizations to deploy their own 5G/LTE networks for industrial IoT, campus connectivity, and mission-critical applications — without relying on public carrier infrastructure.

**Examples** include AWS Private 5G, Celona, Betacom, FreedomFi, Cisco Private 5G, Nokia Digital Automation Cloud, Ericsson Cradlepoint, Druid Software, Mavenir, and Athonet (the category leaders).

**Open-source emphasis**: Private cellular is one of the strongest open-source domains in telecommunications. **Open5GS**, **srsRAN**, **OpenAirInterface**, **Ella Core**, and **Magma** collectively provide complete 5G core and RAN stacks deployable on commodity hardware. **ONF SD-Core** and **O-RAN SC** bring disaggregated, cloud-native architectures. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AWS Private 5G](https://aws.amazon.com/private5g/)**  
  **AWS's managed private 5G service** — deploy and scale private cellular networks on AWS . **Fully managed infrastructure** . **Best for AWS-native private 5G** .

- **[Celona](https://www.celona.io/)**  
  **Enterprise private 5G platform** — plug-and-play private cellular for enterprises . **Best for simple enterprise deployments** .

- **[Betacom](https://www.betacom.com/)**  
  **Private 5G managed services** — design, deploy, and operate private networks . **Best for managed private 5G** .

- **[FreedomFi](https://www.freedomfi.com/)**  
  **Private 5G for enterprises** — CBRS-based private networks . **Best for CBRS deployments** .

- **[Cisco Private 5G](https://www.cisco.com/)**  
  **Cisco's private 5G solution** — integrated with Cisco networking portfolio . **Best for Cisco ecosystem** .

- **[Nokia Digital Automation Cloud](https://www.nokia.com/)**  
  **Nokia's private wireless platform** — industrial-grade private LTE/5G . **Best for industrial deployments** .

- **[Ericsson Cradlepoint](https://cradlepoint.com/)**  
  **Wireless WAN and private 5G** — enterprise connectivity solutions . **Best for enterprise WAN** .

- **[Druid Software](https://www.druidsoftware.com/)**  
  **Private cellular core software** — Raemis core for private networks . **Best for private core** .

- **[Mavenir](https://www.mavenir.com/)**  
  **Cloud-native private networks** — 5G core and RAN solutions . **Best for cloud-native deployments** .

- **[Athonet](https://www.athonet.com/)**  
  **Private cellular core platform** — enterprise private networks . **Best for enterprise private core** .

## Open-Source GitHub Projects

### 5G Core Networks

- **[Open5GS](https://github.com/open5gs/open5gs)**  
  **The leading open-source 5G core network**, AGPL-3.0 licensed with **3,000+ GitHub stars** . **Complete 5G SA and LTE EPC implementation** following 3GPP standards . **Open5GSBox** demonstrates fully deployable 5G SA with integrated RAN on Raspberry Pi 5 and x86 hardware, achieving **up to 212 Mbps downlink and 97 Mbps uplink** with ~30ms latency  . **The de facto open-source 5G core** — used in the Conakry, Guinea deployment with **2.8 GB memory and 45-second startup for 15 containers**  . **Best for production private 5G deployments** .

- **[Ella Core](https://github.com/ellanetworks/core)**  
  **Production-geared open-source 5G core for private networks**, Apache-2.0 licensed . **Single binary with embedded database** — requires only **2 CPU cores, 2GB RAM, and 10GB disk**  . **eBPF-based data plane delivering over 5 Gbps throughput and under 1.5ms latency**  . **Validated with multiple gNodeBs** including Baicells Stellar 227, Vankom VKScell-g3, and Ettus B210 with srsRAN  . **The simplest path to a production 5G core** — web UI, REST API, Prometheus metrics, and audit logs included . **Best for private networks where simplicity and performance matter** .

- **[Magma](https://github.com/magma/magma)**  
  **Open-source mobile core network platform**, BSD-3-Clause licensed . **Supports LTE EPC and 5G SA with Federation Gateway (FEG)** for multi-network orchestration  . **Community-tested with srsRAN eNB/gNB and USRP B210 radios**  . **The de facto open-source core for federated networks** — used in research and community deployments . **Best for federated private networks and research** .

- **[Free5GC](https://github.com/free5gc/free5gc)**  
  **Open-source 5G core network**, Apache-2.0 licensed . **Microservices-based architecture** with cloud-native principles . **Best for cloud-native 5G core** .

- **[ONF SD-Core](https://github.com/omec-project/)**  
  **Open-source disaggregated mobile core**, Apache-2.0 licensed . **Supports 4G LTE and 5G SA/NSA** . **Part of ONF's Aether project** with 15 live deployments including DARPA  . **Best for disaggregated cloud-native core** .

### RAN & gNodeB/eNodeB

- **[srsRAN Project](https://github.com/srsran/srsRAN_Project)**  
  **The leading open-source 5G RAN**, AGPL-3.0 licensed . **5G gNodeB and 4G eNodeB implementation** with **commercial-grade performance** . **Open5GBox** achieves **212 Mbps DL / 97 Mbps UL with ~30ms latency** on COTS hardware  . **Scalable from Raspberry Pi 5 to x86 servers**  . **The de facto open-source RAN** — used in Open5GBox and countless private deployments . **Best for production private 5G RAN** .

- **[OpenAirInterface (OAI)](https://github.com/OPENAIRINTERFACE/openairinterface5g)**  
  **The veteran open-source cellular platform**, CSSL licensed . **Full 4G LTE and 5G NR stack** — RAN, core network, and OAM  . **Supports FR1 (sub-6 GHz) bands n40, n41, n77, n78** with 100 MHz bandwidth and 4×2 MIMO  . **O-RAN O-SC Open Fronthaul implementation** with libxran and DPDK  . **Hardware requirements**: minimum 2 CPU cores, 4GB RAM for simulated radio; 8-10 cores and 5GB+ for performance deployments  . **Active development under OpenAirInterface Software Alliance** with 11 full-time staff  . **Best for research and advanced experimentation** .

- **[OCUDU](https://github.com/OCUDU/OCUDU)**  
  **Open-source Centralized Unit / Distributed Unit implementation** for disaggregated RAN . **Achieves higher E2E throughput than OAI** in both DL and UL directions  . **F1 interface implementation** with CU-CP, CU-UP, and DU components  . **Best for disaggregated O-RAN deployments** .

### Testbeds & Research Platforms

- **[Colosseum](https://www.colosseum.net/)**  
  **Open-access large-scale wireless testbed** — remote access 24/7/365 . **High-fidelity RF channel emulator with SDR devices**  . **Used for 5G Beyond & 6G, Digital Twin, O-RAN, and AI-driven radio resource management research**  . **Best for large-scale wireless research** .

- **[Arena](https://arena.nec-labs.com/)**  
  **Open-access wireless testing platform** — 24 synchronized SDR devices and 64 antennas in office environment  . **Best for sub-6 GHz 5G and Beyond research** .

- **[POWDER](https://powderwireless.net/)**  
  **Platform for Open Wireless Data-driven Experimental Research** — remotely accessible, software-defined platform  . **Best for wireless and mobile research** .

- **[ARA Wireless Living Lab](https://arawireless.org/)**  
  **Publicly-available wireless living lab** — used for first end-to-end integration of **Open5GS with Ericsson commercial RAN**  . **Best for real-world open-source core validation** .

### Additional Strong Open-Source Options

- **UERANSIM** — 5G UE and RAN simulator for testing 5G core networks .
- **O-RAN SC** — O-RAN Software Community with Near-RT RIC and xApps  .
- **ONF SD-RAN** — Open-source RAN project .
- **ONF SD-Fabric** — Programmable network fabric for 5G  .
- **Open5GS WebUI** — Web interface for Open5GS subscriber management  .
- **srsRAN 4G** — Legacy 4G eNodeB and EPC implementation .

**Frameworks for building custom private cellular solutions**: Combine **Open5GS** or **Ella Core** for the 5G core with **srsRAN** or **OpenAirInterface** for the RAN . Use **Magma** for federated multi-network deployments . Deploy **ONF SD-Core** for disaggregated cloud-native architecture . Leverage **Colosseum**, **Arena**, or **POWDER** for research testbeds . Note that true commercial private 5G with managed SLAs, carrier-grade support, and integrated hardware remains primarily commercial territory; open-source stacks provide strong core, RAN, and testbed foundations that require integration and RF expertise for complete deployments .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Private cellular deployments require **spectrum licenses** (CBRS, licensed bands) and compliance with local telecommunications regulations. **Verify licensing requirements before transmitting** .
- **Security hardening is critical** — research demonstrates attack vectors including AMF SBI exposure, PFCP exposure, NGAP source filtering, and NAS null-ciphering preference. Each requires reversible hardening actions .
- **Hardware requirements vary by deployment** — simulated radio needs 2 cores/4GB RAM; performance deployments need 8-10 cores and 5GB+ with AVX512 support . Raspberry Pi 5 can run small deployments .
- **Open-source cores have different strengths** — Open5GS for production, Ella Core for simplicity, Magma for federation. Choose based on your use case .
- The open-source ecosystem provides strong core, RAN, and testbed foundations, but **carrier-grade support, managed SLAs, and integrated hardware** remain primarily commercial offerings.

---

**Made for network engineers, telecom researchers, and organizations seeking private cellular sovereignty.**
Let's make private 5G/LTE networks more open, transparent, and accessible.
