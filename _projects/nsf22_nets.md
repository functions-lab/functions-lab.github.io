---
layout: page
title: NSF CISE Core
description: "Medium: Softwarizing Millimeter-wave Radio Access Networks (RANs) at the Edge"
img: assets/img/sponsor/icon_nsf.png
importance: 7
category: current
related_publications: false
---

### **Project Information**

- **Award Numbers**: CNS-2211944, CNS-2211945
- **Project Duration**: 2022/10–2026/09
- **Program**: NSF CISE, CNS Core
- **Principal Investigator**: [Prof. Tingjun Chen](https://functions-lab.github.io/) (Duke University)
- **Co-Principal Investigator**: [Prof. Lin Zhong](https://www.linzhong.org/) (Yale University)
- **Postdocs**: Dr. Xiao Zhang (Duke); Dr. Parthiban Annamalai (Yale)
- **Graduate Students**: Wei Cheng, Zhihui Gao, Yiming Li, Zhenzhou Qi, Samuel Rivera, Chung-Hsuan Tung, Zehao Wang (Duke); Guojun Chen, In Gim, Ramla Ijaz, Zhiyao Ma, George Typaldos (Yale)
- **Undergraduate Students**: Scarlett Francini, Zeyu Li, Yi-Chyun Wong (Duke); Archit Kumar, Jordan Miller, Sebastian Orozco, Miranda Selin, Skylar Wang, Felix Zou (Yale)


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
We designed real-time baseband processing frameworks for single-cell (**Savannah**) and multi-cell (**Nexus**) scenarios leveraging heterogneous compute resources including CPUs (Intel's Xeon processors) and ASICs (Intel's ACC100 eASICs), with comprehensive power-latency profiling, modeling, and optimization (*MobiCom'26*, *MobiCom'24*, *WiNTECH'23*).
We have also studeid dynamic resource provisioning in elastic massive MIMO vRAN systems to dynamically allocate CPU cores for varying computational loads (*HotMobile'25*).
We also developed *DecodeX*, a software suite for benchmarking LDPC decoding performance across CPU, GPU, and ASIC platforms (*HotMobile'26*).

<div class="row justify-content-center my-1">
    <div class="col-md-8">
      {% include figure.liquid
         path="assets/img/projects/mobicom2024_savannah.png"
         title="MobiCom2024 Savannah"
         class="img-fluid rounded shadow-sm" %}
      <div class="caption text-center mt-2">
        Over-the-air (OTA) evaluation of Savannah using USRP SDRs in Lab (sub-6 GHz) and the PAWR COSMOS testbed (28 GHz).
      </div>
    </div>
</div>

- **Software-defined Python-enhanced RFSoC for wideband radio applications:**
We designed and implemented **SPEAR**, an SDR platform based on the Xilinx RFSoC ZCU216 evaluation board capable of supporting real-time, multi-channel (up to 16T16R), wideband (up to 1.25 GHz per channel) radio applications employing the direct RF radio architecture (*MILCOM'25*, *WiNTECH'24*).

<div class="row justify-content-center my-1">
    <div class="col-md-8">
      {% include figure.liquid
         path="assets/img/projects/milcom2025_spear+.png"
         title="MILCOM2025 SPEAR+"
         class="img-fluid rounded shadow-sm" %}
      <div class="caption text-center mt-2">
        Experimental evaluation of SPEAR+: (a/b) A ZCU216 board connected to two antenna arrays, forming an OTA link at 800 MHz. (c) A ZCU216 board connected to two CHARM modules, forming an OTA link at 135 GHz.
      </div>
    </div>
</div>

- **Radio resource allocation and scheduling for communication and sensing:**
We developed **Mambas**, an analog multi-user beamforming tailored for mmWave networks employing the array of subarrays (ASA) architecture, supporting simultaneous communication with multiple users located in close proximity, even within the half-power beamwidth of the ASA (*MobiCom'24*).
We developed **Chameleon**, a framework that augments and rapidly switches beamformers during each demodulation reference signal (DMRS) symbol to achieve integrated sensing and communication (ISAC) in 5G mmWave networks, where each beamformer introduces an additional sensing beam toward target angles while maintaining the communication beams toward multiple users (*RFSA'26*).
We also studied sectorized wireless mesh networks with beam-steering infrastrucuture nodes, characterized their capacity region and sectorization gain via a flow extension ratio, and developed a distributed optimization algorithm that computes near-optimal node sectorization with a 2/3 approximation guarantee to maximize network flow (*TON'25*, *MobiHoc'23*).

- **Modeling and optimization of optical fronthaul:**
We studied both component- and network-level modeling and optimization of reconfigurable optical fronthaul that serves as the underlying infrastructure connecting base stataions with (edge) data centers.
Through a series of lab experiments and field trials, we demonstrated reliable quality of transmission (QoT) estimation in the optical layer and co-existence of heterogeneous fronthaul traffics including 5G, wideband spectrum sensing based on analog radio-over-fiber (ARoF), and 400 GbE coherent optics (*JOCN'26*, *JLT'25*, *JLT'24*, *OFC'25*, *OFC'24*, *OFC'23*, *ECOC'23*).

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

- **Agora**: [https://github.com/Agora-wireless/Agora](https://github.com/Agora-wireless/Agora).


### **Broader Impacts**

This project fuels the ongoing revolution of mobile network virtualization and accelerate the development and deployment of next-generation network systems.
Specifically, it expedites the adoption of mmWave radios, resulting in more capable, more efficient, and more cost-effective mobile networks.
We leverage our ongoing collaborations with industry leaders to ensure a timely transfer of technologies into industry and a broad impact on the commercial development of mobile network, edge and cloud computing.
By softwarizing wireless network functions at the lowest layer, this project provides a meeting ground for software systems and wireless communication research and creates timely content for teaching Computer Science majors about wireless physical layer.
The project also provides a platform to engage undergraduate students and high-school students in wireless and computing research.


### **Publications**
1. Z. Qi, C.-H. Tung, Z. Gao, and T. Chen, “Nexus: Efficient and Scalable Multi-Cell mmWave Baseband Processing with Heterogeneous Compute,” in *Proc. ACM International Conference on Mobile Computing and Networking (MobiCom’26)*, 2026.

1. Z. Gao, Z. Liu, and T. Chen, “Chameleon: Integrated Sensing and Communication with Sub-Symbol Beam Switching in mmWave Networks,” in *Proc. IEEE/MTT-S RF Systems & Applications Symposium (RFSA’26)*, 2026.

1. Z. Qi, Y. Yao, Y. Li, C.-H. Tung, J. Zheng, D. Zhuo, and T. Chen, “DecodeX: Exploring and Benchmarking of LDPC Decoding across CPU, GPU, and ASIC Platforms,” in *Proc. ACM Workshop on Mobile Computing Systems and Applications (HotMobile’26)*, 2026.

1. Z. Wang, A. D’Amico, G. Borraccini, A. Raj, Y.K. Huang, S. Han, T. Wang, M. Ruffini, D. Kilper, and T. Chen, “Scalable ML Models and Cascaded Learning for Efficient Multi-Span OSNR and GSNR Prediction,” *IEEE/Optica Journal of Optical Communications and Networking (JOCN)*, vol. 18, no. 1, pp. A88–A99, Jan. 2026. **Invited Paper to the JOCN Special Issue on Invited/Top-Rated Papers from IEEE/Optica OFC’25**

1. W. Cheng, Z. Gao, J. Guajardo, H. Beshary, A. Niknejad, and T. Chen, “SPEAR+: Streaming-Based Multi-Channel SDR Implementation Using the RFSoC Platform,” in *Proc. IEEE Military Communications Conference (MILCOM’25)*, 2025.

1. P. Promponas, T. Chen, and L. Tassiulas, “On the Optimization and Stability of Sectorized Wireless Networks,” *IEEE/ACM Transactions on Networking (TON)*, vol. 33, no. 6, pp. 3228–3243, Dec. 2025.

1. T. Sasai, G. Borraccini, Y.-K. Huang, H. Nishizawa, Z. Wang, T. Chen, Y. Sone, M. Takahashi, T. Matsumura, M. Nakamura, E. Yamazaki, K. Takasugi, T. Wang, and Y. Kisaka, “Optical Link Tomography: First Field Trial and 4D Extension,” *IEEE/Optica Journal of Lightwave Technology (JLT)*, vol. 43, no. 24, pp. 10776–10787, Oct. 2025. **Invited Paper to the JLT Special Issue on Postdeadline Papers from IEEE/Optica OFC’24**

1. Z. Wang, A. Raj, G. Borraccini, S. Han, Y.-K. Huang, T. Wang, M. Ruffini, D. Kilper, and T. Chen, “Scalable Machine Learning Models for Optical Transmission System Management,” in *Proc. IEEE/Optica Optical Fiber Communication Conference (OFC’25) (invited)*, Paper M1J.3, 2025.

1. Z. Wang, G. Borraccini, A. D’Amico, Y.-K. Huang, T. Wang, D. Kilper, K. Asahi, and T. Chen, “Multi-Span OSNR and GSNR Prediction using Cascaded Learning,” in *Proc. IEEE/Optica Optical Fiber Communication Conference (OFC’25)*, Paper Tu3I.6, 2025.

1. P. Annamalai, M. Kim, A. Anurag, and L. Zhong, “Exploring Intelligent Dynamic Resource Provisioning for Elastic Massive MIMO vRAN,” in *Proc. ACM Workshop on Mobile Computing Systems and Applications (HotMobile’25)*, 2025.

1. Z. Ma, C. Li, and L. Zhong, “MappedTrace: Tracing Pointer Remotely with Compiler-generated Maps,” *arXiv preprint arXiv:2501.10668*, Jan. 2025.

1. Z. Qi, C.-H. Tung, A. Kalia, and T. Chen, “Savannah: Efficient mmWave Baseband Processing with Minimal and Heterogeneous Resources,” in *Proc. ACM International Conference on Mobile Computing and Networking (MobiCom’24)*, 2024.

1. Z. Gao, Z. Qi, and T. Chen, “Mambas: Maneuvering Analog Multi-User Beamforming Using an Array of Subarrays in mmWave Networks,” in *Proc. ACM International Conference on Mobile Computing and Networking (MobiCom’24)*, 2024.

1. W. Cheng, Z. Gao, and T. Chen, “SPEAR: Software-defined Python-Enhanced RFSoC for Wideband Radio Applications,” in *Proc. ACM Workshop on Wireless Network Testbeds, Experimental Evaluation & CHaracterization (WiNTECH’24)*, 2024.

1. Z. Wang, Y.-K. Huang, S. Han, T. Wang, D. Kilper, and T. Chen, “Multi-Span Optical Power Spectrum Prediction Using ML-based EDFA Models and Cascaded Learning,” in *Proc. IEEE/Optica Optical Fiber Com- munication Conference (OFC’24)*, Paper M1H.6, 2024. **Top-Scored Paper Corning** and **Outstanding Student Paper Competition Finalist**

1. Z. Wang, Y.-K. Huang, E. Ip, Z. Qi, G. Zussman, D. Kilper, K. Asahi, H. Kageshima, Y. Aono, and T. Chen, “Field Trial of Coexistence and Simultaneous Switching of Real-Time Fiber Sensing and Coherent 400 GbE in a Dense Urban Environment,” *IEEE/Optica Journal of Lightwave Technology (JLT)*, vol. 42, no. 4, pp. 1304–1311, Feb. 2024. **Invited Paper to the JLT Special Issue on Top-Scored Papers from IEEE/Optica OFC’23**

1. Z. Qi, Z. Gao, C.-H. Tung, and T. Chen, “Programmable Millimeter-wave MIMO Radios with Real-Time Baseband Processing,” in *Proc. ACM Workshop on Wireless Network Testbeds, Experimental Evaluation & CHaracterization (WiNTECH’23)*, 2023.

1. P. Promponas, T. Chen, and L. Tassiulas, “Optimizing Sectorized Wireless Networks: Model, Analysis, and Algorithm,” in *Proc. ACM International Symposium on Theory, Algorithmic Foundations, and Protocol Design for Mobile Networks and Mobile Computing (MobiHoc’23)*, 2023.

1. T. Mano, T. Ferreira de Lima, Y.-K. Huang, Z. Wang, W. Ishida, E. Ip, A. D’Amico, S. Okamoto, T. Inoue, H. Nishizawa, V. Curri, G. Zussman, D. Kilper, T. Chen, T. Wang, K. Asahi, and K. Takasugi, “First Field Demonstration of Automatic WDM Optical Path Provisioning over Alien Access Links for Data Center Exchange,” in *Proc. European Conference on Optical Communication (ECOC’23)*, Paper Tu.B.5.2, 2023. **Highest Scoring and Best Paper**

1. Y.-K. Huang, Z. Wang, E. Ip, Z. Qi, G. Zussman, D. Kilper, K. Asahi, H. Kageshima, Y. Aono, and T. Chen, “Field Trial of Coexistence and Simultaneous Switching of Real-Time Fiber Sensing and 400 GbE Supporting DCI and 5G Mobile Services,” in *Proc. IEEE/Optica Optical Fiber Communication Conference (OFC’23)*, Paper W3H.4, 2023. **Top-Scored Paper**

1. Y. Yu, S. Lee, A. Khandelwal and L. Zhong, “GCS: Generalized Cache Coherence For Efficient Synchronization,” *arXiv preprint arXiv:2301.02576*, Jan. 2023.