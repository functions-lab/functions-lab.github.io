---
layout: page
title: NSF SWIFT
description: "SHIELD: A Software-Hardware Approach for Spectrum Coexistence with Rapid Interferer Learning, Detection, and Mitigation"
img: assets/img/sponsor/icon_nsf.png
importance: 1
category: past
related_publications: true
---

### **Project Information**

- **Award Numbers**: CNS-2128638, CNS-2128530, CNS-2128535
- **Project Duration**: 2021/10–2025/09
- **Program**: NSF Spectrum and Wireless Innovation enabled by Future Technologies (SWIFT)
- **Principal Investigator**: [Prof. Tingjun Chen](https://functions-lab.github.io/) (Duke University)
- **Co-Principal Investigator**: [Prof. Arun Natarajan](https://engineering.yale.edu/research-and-faculty/faculty-directory/arun-natarajan) (Oregon State University), [Prof. Leandros Tassiulas](https://engineering.yale.edu/research-and-faculty/faculty-directory/leandros-tassiulas) (Yale University)
- **Postdocs**: 
- **Graduate Students**: Wei Cheng, Zhihui Gao, Yiming Li, Zhenzhou Qi, Chung-Hsuan Tung, Zehao Wang (Duke);
- **Undergraduate Students**: Scarlett Francini, Zeyu Li, Yi-Chyun Wong, Yunjia Zhang, Junyao Zheng (Duke);


### **Project Overview**

The last two decades have witnessed enormous increase in wireless data transfer, impacting every aspect of our lives and our nation's economy. This has led to a spectrum crunch in frequency bands below 6 GHz that are the most useful for intermediate and long-range wireless communications. Even as new spectrum is allocated for different wireless networks and systems, satisfying the increasing demand of high data rates will lead to coexistence of active users (that generate signals) and passive users (that sense signals for weather sensing, astronomy, and other applications). Inevitably, interference occurs when these users share the same frequency band or when active users operate in bands close to that used by passive users. Therefore, there is a critical need for an approach to efficiently manage and reduce such interference, which will allow for further improved spectrum usage. This project will address this challenge and focus on a cross-layer software-hardware approach for spectrum coexistence with rapid interferer learning, detection, and mitigation. On a societal scale, the proposed research can improve spectrum utilization and increase access to in-demand wireless data without adversely impacting existing users, which will have direct economic impact. The broader impacts also include major outreach activities involving high school students and aiming at broadening the participation of women and underrepresented minorities, as well as incorporation of new hardware, software, and network architecture into undergraduate and graduate classes.

Specifically, this interdisciplinary project will bridge the gap between the broad areas of integrated circuits, communications, networking, and machine learning, and will focus on enabling rapid interferer learning, detection, and mitigation for spectrum coexistence based on the co-design of novel RF hardware and network control architecture. The main activities include:
(i) Extensive spectrum measurements and data collection for characterizing the spectrum usage and properties of potential interferers,
(ii) Development of a novel reconfigurable 0.4–4.0 GHz MIMO receiver architecture leveraging a concurrent auxiliary receiver for rapid interference detection and N-path sequence-mixing for nulling specific interferers, and
(iii) Design of an intelligent control plane, which integrates software-defined networking and machine learning techniques, for efficient spectrum monitoring, management, and resource allocation across spatially distributed receivers. The developed hardware and software will be evaluated in the lab setting and in real-world environments through their integration in a city-scale wireless testbed.


### **Key Results and Outcomes**


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


### **Code and Dataset**

- **Geo2SigMap**: [https://github.com/functions-lab/geo2sigmap](https://github.com/functions-lab/geo2sigmap).

- **SPEAR**/**SPERA+**: [https://github.com/functions-lab/SPEAR](https://github.com/functions-lab/SPEAR).


### **Broader Impacts**

This project focuses on a cross-layer software-hardware approach for spectrum coexistence with rapid interferer learning, detection, and mitigation.
On a societal scale, the proposed research can improve spectrum utilization and increase access to in-demand wireless data without adversely impacting existing users, which will have direct economic impact.
The broader impacts also include major outreach activities involving high school students and aiming at broadening the participation students in the STEM fields, as well as incorporation of new hardware, software, and network architecture into undergraduate and graduate classes.


### **Publications**

1. C.-H. Tung, Z. Qi, and T. Chen, “RISE: Real-Time Image Processing for Spectral Energy Detection and Localization,” in *Proc. IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN’26)*, 2026.

1. C. E. Caicedo Bastidas, J. Doshi, M. R. Choudhury, A. K. Huliyar, A. Adhikari, K. Hermstein, A. Singh, T. Chen, K. Jamieson, F. Moshary, I. Seskar, D. Raychaudhuri, Gil Zussman, “COSMOS ZMS: A Radio Dynamic Zone Management System Using the COSMOS Platform,” in *Proc. IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN’26)*, 2026.

1. P. Promponas, T. Chen, and L. Tassiulas, “On the Optimization and Stability of Sectorized Wireless Networks,” *IEEE/ACM Transactions on Networking (TON)*, vol. 33, no. 6, pp. 3228–3243, Dec. 2025.

1. A. Undavalli, K. Rashed, A. R. Hossain, G. Cauwenberghs, S. Chakrabartty, A. Natarajan, and A. Nagulu, “Fully Analog, Multi-Lag, RF Correlators for Code-Domain Radars Using Margin Propagation,” *IEEE Journal of Solid-State Circuits (JSSC)*, vol. 60, no. 11, pp. 4033-4048, Nov. 2025.

1. Y. Li, S. Francini, Z. Gao, and T. Chen, “Demo: ClickDT: Building Scalable and High-Resolution Wireless Digital Twins with a Few Clicks,” in *Proc. IEEE Military Communications Conference (MILCOM’25)*, 2025.

1. Z. Gao, Z. Liu, and T. Chen, “BatStation: Toward In-Situ Radar Sensing on 5G Base Stations with Zero-Shot Template Generation,” *arXiv:2509.06898 [cs.NI]*, Sept. 2025.

1. Y. Li, Z. Gao, J. Palathinkal, M. Ghosh, and T. Chen, “A Generalized Deep Learning Model for Signal Coverage Prediction in the CBRS Band,” in *Proc. IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN’25)*, 2025.

1. A. Undavalli, K. Rashed, A. R. Hossain, G. Cauwenberghs, S. Chakrabartty, A. Natarajan, and A. Nagulu, “A 4GS/s Fully Analog 256×256 MP-Based Cross-Correlator with 1000 TOPS/W Compute Efficiency and 1.3TOPS/mm2 Compute Density in 22nm SOI CMOS,” in *Proc. IEEE International Solid-State Circuits Conference (ISSCC)*, 2025.

1. K. Rashed, A. Undavalli, S. Chakrabartty, A. Nagulu, and A. Natarajan, “A Scalable and Instantaneously Wideband RF Correlator Based on Margin Computing,” *IEEE Journal of Solid-State Circuits (JSSC)*, vol. 59, no. 11, pp. 3612-3626, Nov. 2024.

1. W. Cheng, Z. Gao, and T. Chen, “SPEAR: Software-defined Python-Enhanced RFSoC for Wideband Radio Applications,” in *Proc. ACM Workshop on Wireless Network Testbeds, Experimental Evaluation & CHaracterization (WiNTECH’24)*, 2024.

1. Z. Gao, Y. Zhang, and T. Chen, “DeepMon: Wi-Fi Monitoring Using Sub-Nyquist Sampling Rate Receivers with Deep Learning,” in *Proc. ACM Workshop on Machine Learning for Next-Generation Networks (ML-NextG’24)*, 2024.

1. T. Crump, S. Kompella, C. Kam, and L. Tassiulas, “SAR Data Generation Using Denoising Diffusion Probabilistic Models,” in *Proc. IEEE Military Communications Conference (MILCOM’24)*, 2024.

1. Y. Li, Z. Li, Z. Gao, and T. Chen, “Geo2SigMap: High-Fidelity RF Signal Mapping Using Geographic Databases,” in *Proc. IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN’24)*, 2024.

1. K. Rashed, A. Undavalli, S. Chakrabartty, A. Nagulu, and A. Natarajan, “A Scalable and Instantaneously Wideband 5GS/s RF Correlator Based on Charge Thresholding Achieving 8-bit ENOB and 152 TOPS/W Compute Efficiency,” in *Proc. IEEE International Solid-State Circuits Conference (ISSCC)*, 2024.

1. Z. Wang, Y.-K. Huang, E. Ip, Z. Qi, G. Zussman, D. Kilper, K. Asahi, H. Kageshima, Y. Aono, and T. Chen, “Field Trial of Coexistence and Simultaneous Switching of Real-Time Fiber Sensing and Coherent 400 GbE in a Dense Urban Environment,” *IEEE/Optica Journal of Lightwave Technology (JLT)*, vol. 42, no. 4, pp. 1304–1311, Feb. 2024. **Invited Paper to the JLT Special Issue on Top-Scored Papers from IEEE/Optica OFC’23**

1. H. Nishizawa, T. Mano, T. Ferreira de Lima, Y.-K. Huang, Z. Wang, W. Ishida, M. Kawashima, E. Ip, A. D’Amico, S. Okamoto, T. Inoue, K. Anazawa, V. Curri, G. Zussman, D. Kilper, T. Chen, T. Wang, K. Asahi, K. Takasugi, “Fast WDM Provisioning with Minimal Probing: The First Field Experiments for DC Exchanges,” *IEEE/Optica Journal of Optical Communications and Networking (JOCN)*, vol. 16, no. 2, pp. 233–242, Feb. 2024.

1. Z. Gao, Y. Chen, and T. Chen, “Swirls: Sniffing Wi-Fi Using Radios with Low Sampling Rates,” in *Proc. ACM International Symposium on Theory, Algorithmic Foundations, and Protocol Design for Mobile Networks and Mobile Computing (MobiHoc’23)*, 2023.

1. P. Promponas, T. Chen, and L. Tassiulas, “Optimizing Sectorized Wireless Networks: Model, Analysis, and Algorithm,” in *Proc. ACM International Symposium on Theory, Algorithmic Foundations, and Protocol Design for Mobile Networks and Mobile Computing (MobiHoc’23)*, 2023.

1. A. Mudvari, K. Poularakis, and L. Tassiulas, “Robust SDN Synchronization in Mobile Networks Using Deep Reinforcement and Transfer Learning,” in *Proc. IEEE International Conference on Communications (ICC’23)*, 2023.

1. P. Promponas and L. Tassiulas, “Network Slicing: Market Mechanism and Competitive Equilibria,” in *Proc. IEEE Conference on Computer Communications (INFOCOM'23)*, 2023.

1. T. Mano, T. Ferreira de Lima, Y.-K. Huang, Z. Wang, W. Ishida, E. Ip, A. D’Amico, S. Okamoto, T. Inoue, H. Nishizawa, V. Curri, G. Zussman, D. Kilper, T. Chen, T. Wang, K. Asahi, and K. Takasugi, “First Field Demonstration of Automatic WDM Optical Path Provisioning over Alien Access Links for Data Center Exchange,” in *Proc. European Conference on Optical Communication (ECOC’23)*, Paper Tu.B.5.2, 2023. **Highest Scoring and Best Paper**

1. Y.-K. Huang, Z. Wang, E. Ip, Z. Qi, G. Zussman, D. Kilper, K. Asahi, H. Kageshima, Y. Aono, and T. Chen, “Field Trial of Coexistence and Simultaneous Switching of Real-Time Fiber Sensing and 400 GbE Supporting DCI and 5G Mobile Services,” in *Proc. IEEE/Optica Optical Fiber Communication Conference (OFC’23)*, Paper W3H.4, 2023. **Top-Scored Paper**
