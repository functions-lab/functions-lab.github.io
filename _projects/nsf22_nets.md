---
layout: page
title: NSF CISE Core
description: "Medium: Softwarizing Millimeter-wave Radio Access Networks (RANs) at the Edge"
img: assets/img/sponsor/icon_nsf.png
importance: 7
category: current
related_publications: true
---

### **Project Information**

- **Award Numbers:** CNS-2211944, CNS-2211945
- **Project Duration:** 2022/10–2026/09
- **Program:** NSF CISE, CNS Core
- **Principal Investigator:** [Prof. Tingjun Chen](https://functions-lab.github.io/) (Duke University)
- **Co-Principal Investigator:** [Prof. Lin Zhong](https://www.linzhong.org/) (Yale University)
- **Graduate Students:** Wei Cheng, Zhihui Gao, Yiming Li, Zhenzhou Qi, Samuel Rivera, Chung-Hsuan Tung, Zehao Wang (Duke University)
- **Undergraduate Students:** Scarlett Francini, Zeyu Li, Yi-Chyun Wong (Duke University)


### **Project Overview**

Emerging applications in augmented reality, connected autonomous vehicles, and industrial IoT systems impose demanding requirements on next-generation mobile networks that can hardly be met alone with radio resources below 7 GHz.
Therefore, 5G and beyond networks have embraced radios operating in millimeter-wave (mmWave) frequency bands, which offer 25 times or more bandwidth worldwide. On the other hand, mmWave radio networks require the dense deployment of infrastructure nodes to achieve desirable coverage, because mmWave radio signals suffer from high propagation loss and are vulnerable to blockage and mobility. Unfortunately, mmWave infrastructure nodes, e.g., gNodeB in 5G, are made of specialized, dedicated hardware and as a result, their dense deployment would incur formidable capital and operational cost.
The goal of the proposed project is to reduce the cost of mmWave radio infrastructure nodes by softwarizing their radio access network (RAN) functions and serving them from data centers close to end users, i.e., edge data centers, therefore facilitating network densification. More importantly, it will allow for previously impossible flexibility in network implementation and configuration as well as efficiency in resource allocation across the network and the edge data center.
At the societal level, this project will fuel the ongoing revolution of mobile network virtualization and accelerate the development and deployment of next-generation network systems.

The key insight toward addressing the challenges associated with softwarizing mmWave RANs at the edge is to exploit the massive data parallelism inside the mmWave baseband and its inherent structures, with programmable hardware in all domains.
The project targets the following scientific contributions in three interrelated research thrusts.
(i) A low-latency software realization of the mmWave physical layer for commodity server clusters suitable for edge deployment.
(ii) Adaptive RAN configuration and in-network compression schemes that cope with the limited fronthaul capacity in practice, without substantially increasing the cost of mmWave infrastructure nodes.
(iii) Novel sensing and imaging schemes based on mmWave radio signals intended for communications.
These include sensing with a single mmWave infrastructure node and sensing that leverages multiple coordinated mmWave nodes to achieve previously impossible coverage and resolution.


### **Key Results and Outcomes**

- **Softwarization of baseband processing in mmWave vRANs:** 
We designed real-time baseband processing frameworks for single-cell (**Savannah**) and multi-cell (**Nexus**) scenarios leveraging heterogneous compute resources including CPUs (Intel's Xeon processors) and ASICs (Intel's ACC100 eASICs), with comprehensive power-latency profiling, modeling, and optimization {% cite qi2026nexus qi2024savannah qi2023programmable %}.
We also developed **DecodeX**, a software suite for benchmarking LDPC decoding performance across CPU, GPU, and ASIC platforms {% cite qi2026decodex %}

<div class="row justify-content-center my-1">
    <div class="col-md-8">
      {% include figure.liquid
         path="assets/img/projects/mobicom2024_savannah.png"
         title="MobiCom2024 Savannah"
         class="img-fluid rounded shadow-sm" %}
      <div class="caption text-center mt-2">
        Over-the-air (OTA) evaluation of Savannah {% cite qi2024savannah %} using USRP SDRs in Lab (sub-6 GHz) and the PAWR COSMOS testbed (28 GHz).
      </div>
    </div>
</div>

- **Software-defined Python-enhanced RFSoC for wideband radio applications:**
We designed and implemented **SPEAR**, an SDR platform based on the Xilinx RFSoC ZCU216 evaluation board capable of supporting real-time, multi-channel (up to 16T16R), wideband (up to 1.25 GHz per channel) radio applications employing the direct RF radio architecture {% cite cheng2025spear+ cheng2024spear %}.

<div class="row justify-content-center my-1">
    <div class="col-md-8">
      {% include figure.liquid
         path="assets/img/projects/milcom2025_spear+.png"
         title="MILCOM2025 SPEAR+"
         class="img-fluid rounded shadow-sm" %}
      <div class="caption text-center mt-2">
        Experimental evaluation of SPEAR+ {% cite cheng2025spear+ %}: (a/b) A ZCU216 board connected to two antenna arrays, forming an OTA link at 800 MHz. (c) A ZCU216 board connected to two CHARM modules, forming an OTA link at 135 GHz.
      </div>
    </div>
</div>

- **Radio resource allocation and scheduling for communication and sensing:**
We developed **Mambas**, an analog multi-user beamforming tailored for mmWave networks employing the array of subarrays (ASA) architecture, supporting simultaneous communication with multiple users located in close proximity, even within the half-power beamwidth of the ASA {% cite gao2024mambas %}.
We developed **Chameleon**, a framework that augments and rapidly switches beamformers during each demodulation reference signal (DMRS) symbol to achieve integrated sensing and communication (ISAC) in 5G mmWave networks, where each beamformer introduces an additional sensing beam toward target angles while maintaining the communication beams toward multiple users {% cite gao2025chameleon %}.
We also studied sectorized wireless mesh networks with beam-steering infrastrucuture nodes, characterized their capacity region and sectorization gain via a flow extension ratio, and developed a distributed optimization algorithm that computes near-optimal node sectorization with a 2/3 approximation guarantee to maximize network flow {% cite promponas2023optimizing promponas2025on %}.

- **Modeling and optimization of optical fronthaul:**
We studied both component- and network-level modeling and optimization of reconfigurable optical fronthaul that serves as the underlying infrastructure connecting base stataions with (edge) data centers.
Through a series of lab experiments and field trials, we demonstrated reliable quality of transmission (QoT) estimation in the optical layer and co-existence of heterogeneous fronthaul traffics including 5G, wideband spectrum sensing based on analog radio-over-fiber (ARoF), and 400 GbE coherent optics {% cite wang2026scalable sasai2025optical wang2025multi wang2024multi wang2024field mano2023first huang2023field %}.

<div class="row justify-content-center my-1">
    <div class="col-md-10">
      {% include figure.liquid
         path="assets/img/projects/jlt2023_coexistence.png"
         title="JLT2023 Coexistence"
         class="img-fluid rounded shadow-sm" %}
      <div class="caption text-center mt-2">
        Field trial using the COSMOS testbed with dark fiber connecting two edge sites, supporting coexistence of 400 GbE coherent optics, analog radio-over-fiber (ARoF), and DAS-based fiber sensing signals.
      </div>
    </div>
</div>


### **Code and Dataset**

- **Savannah**/**Nexus**: [https://github.com/functions-lab/Savannah](https://github.com/functions-lab/Savannah).

- **DecodeX**: [https://github.com/functions-lab/DecodeX](https://github.com/functions-lab/DecodeX).

- **SPEAR**/**SPERA+**: [https://github.com/functions-lab/SPEAR](https://github.com/functions-lab/SPEAR).

- **Mambas**: [https://github.com/functions-lab/MAMBAS-MobiCom2024](https://github.com/functions-lab/MAMBAS-MobiCom2024).


### **Broader Impacts**

This project fuels the ongoing revolution of mobile network virtualization and accelerate the development and deployment of next-generation network systems.
Specifically, it expedites the adoption of mmWave radios, resulting in more capable, more efficient, and more cost-effective mobile networks.
We leverage our ongoing collaborations with industry leaders to ensure a timely transfer of technologies into industry and a broad impact on the commercial development of mobile network, edge and cloud computing.
By softwarizing wireless network functions at the lowest layer, this project provides a meeting ground for software systems and wireless communication research and creates timely content for teaching Computer Science majors about wireless physical layer.
The project also provides a platform to engage undergraduate students and high-school students in wireless and computing research.