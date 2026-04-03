# Review Article - Convolutional Neural Networks on Dedicated Hardware: A Comprehensive Survey of VLSI, FPGA and ASIC Implementations Across Real World Application Domains

> A comprehensive survey examining CNN hardware acceleration across five real-world application domains — consolidating quantitative results from FPGA, ASIC, and VLSI implementations into unified comparison tables and identifying cross-domain optimisation strategies and open research challenges.

![Status](https://img.shields.io/badge/Status-Under%20Review-yellow)
![Type](https://img.shields.io/badge/Type-Survey%20Article-blue)
![Domains](https://img.shields.io/badge/Domains-5%20Application%20Areas-orange)
![Focus](https://img.shields.io/badge/Focus-VLSI%20%7C%20FPGA%20%7C%20ASIC-green)



## 📄 Publication Details

| Field | Details |
|:---|:---|
| **Title** | Convolutional Neural Networks on Dedicated Hardware: A Comprehensive Survey of VLSI, FPGA and ASIC Implementations Across Real World Application Domains |
| **Status** | Manuscript under review |
| **Type** | Review Article |


## 👥 Authors

| Name | Affiliation |
|:---|:---|
| **Preetham SK** | School of Electrical Engineering |
| Dr. Lavanya V | Associate Professor, School of Electrical Engineering |
| Dr. Meera P S | Associate Professor, School of Electrical Engineering |


## 🔍 Overview

Convolutional Neural Networks have established themselves as the dominant computational paradigm in modern artificial intelligence — achieving state-of-the-art performance across perception, classification, and segmentation tasks. However, deploying CNNs beyond controlled environments demands hardware platforms capable of sustaining high computational throughput under strict constraints of power consumption, latency, and physical form factor.

This paper examines **CNN hardware acceleration across five real-world application domains** — bringing together implementations realised through VLSI, FPGA, and ASIC technologies to compare approaches, identify universal optimisation patterns, and highlight the most significant open challenges in the field.

Rather than treating each application domain in isolation, the core contribution is a **cross-domain comparative analysis** — the first structured framework that identifies which hardware optimisation strategies generalise broadly and which are shaped by domain-specific constraints.


## 🧠 Motivation

Standard CPUs process operations sequentially and lack the memory bandwidth and parallel compute capacity that CNN inference demands. A well-known architecture like AlexNet already contains 60 million parameters requiring billions of multiply-accumulate operations per inference pass — making dedicated hardware acceleration one of the most active research areas in the field.

The hardware options span a wide performance-flexibility spectrum:
- **GPUs** — 6 to 17× speedup over CPUs; dominant for training
- **FPGAs** — Reconfigurable logic matched to CNN structure; energy-efficient inference
- **ASICs** — Google TPU: 15–30× throughput over CPUs/GPUs through 65,536-element MAC array at 8-bit precision; DaDianNao: 656× performance of single-core GPU at 184× lower power

Existing survey literature either focuses on a single hardware platform or a single application domain. This work uniquely consolidates both dimensions simultaneously.


## 📚 Survey Scope — Five Application Domains

### Domain 1 — Image Processing
Covers CNN workloads for pixel-level operations, object recognition, and 3D reconstruction. Examines processing element design, data reuse strategies, and approximate computing approaches. Key result: FPGA-based accelerators achieve **587.52 GOPs** at **142.95 GOPs/W** energy efficiency for image processing workloads.

### Domain 2 — Advanced Driver Assistance Systems (ADAS)
Covers multi-task CNN deployment for autonomous driving — simultaneous object detection, lane detection, semantic segmentation, and depth estimation. Key result: Multi-task ADAS platforms deliver **25.4 frames per second** across four simultaneous perception tasks on reconfigurable MPSoC architectures.

### Domain 3 — Medical Imaging and Healthcare Diagnostics
Covers CNN accelerators for electrogram classification, tumour detection, retinal analysis, and wearable diagnostic devices. Key result: Dedicated CNN accelerators reach **1.145 TFLOP/s** at **442.948 MHz**, enabling real-time electrogram classification with power dissipation as low as **34.9 µW** — suitable for implantable and wearable medical devices.

### Domain 4 — Internet of Things and Industrial Robotics
Covers edge AI deployments on resource-constrained hardware for real-time industrial inspection, gesture recognition, and embedded robotics. Focus on ultra-low-power CNN inference for battery-operated IoT nodes and industrial automation systems.

### Domain 5 — Smart Surveillance and Remote Sensing
Covers on-board satellite processing, aerial image analysis, and surveillance CNN accelerators. Key result: Lightweight CNN architectures in 16-bit fixed-point precision on space-grade FPGAs **outperform conventional floating-point designs** in both resource utilisation and detection efficiency.


## 💡 Principal Contributions

**1. Hardware Optimisation Taxonomy**
A structured taxonomy of CNN hardware optimisation techniques across three levels:
- *Algorithm level* — Quantisation, pruning, knowledge distillation, architecture search
- *Circuit level* — Approximate computing, voltage scaling, power gating, cell sizing
- *System level* — Dataflow optimisation, memory hierarchy design, hardware-software co-design

**2. Unified Comparison Tables**
Quantitative results from FPGA, ASIC, and VLSI implementations across all five domains consolidated into unified benchmark tables — enabling direct cross-platform and cross-domain comparison for the first time.

**3. Cross-Domain Comparative Analysis (Section VII)**
The core novel contribution: a structured analysis identifying which optimisation strategies generalise across all five domains and which are domain-specific. Key findings:
- Quantisation and pruning generalise broadly but acceptable accuracy trade-offs differ substantially across domains
- Hardware-software co-design is universally effective but implementation complexity varies by domain
- Medical and space applications impose strict accuracy constraints that prevent aggressive approximation
- IoT applications prioritise power over throughput; ADAS applications prioritise latency over area

**4. Open Research Challenges**
Five open research challenges identified at the intersection of CNN algorithms and dedicated hardware — providing a structured perspective on the path toward efficient, scalable, and robust real-time intelligent systems.


## 📊 Selected Quantitative Highlights

| Domain | Platform | Key Metric |
|:---|:---|:---|
| Image Processing | FPGA | 587.52 GOPs at 142.95 GOPs/W |
| ADAS | MPSoC | 25.4 fps across 4 simultaneous tasks |
| Medical Imaging | ASIC | 1.145 TFLOP/s at 442.948 MHz, 34.9 µW |
| Remote Sensing | FPGA (space-grade) | Fixed-point outperforms floating-point |
| General (GPU reference) | GPU | 6–17× speedup over CPU |
| General (ASIC reference) | Google TPU | 15–30× throughput over CPU/GPU |



## 🎯 Index Terms

Convolutional neural networks · FPGA acceleration · VLSI design · ASIC · hardware-software co-design · edge AI · deep learning · image processing · ADAS · medical imaging · IoT · remote sensing · quantisation · real-time inference



## 🔗 Related Work

| Output | Details |
|:---|:---|
| **Survey Article** | Manuscript under review |
| **Related Work** | Fixed-Point Softmax Processing Unit for DNN Inference (Patent Under Review) |



## 🤝 Connect

| **Author** | Preetham SK |
|:---|:---|
| **Programme** | B.Tech. Electrical and Electronics Engineering, VIT Chennai |
| **LinkedIn** | [linkedin.com/in/preethamsk16](https://www.linkedin.com/in/preethamsk16) |
| **GitHub** | [github.com/PreethamSK163](https://github.com/PreethamSK163) |
| **Portfolio** | [preethamsk163.github.io](https://preethamsk163.github.io) |
| **Email** | preethamsk163@gmail.com |
