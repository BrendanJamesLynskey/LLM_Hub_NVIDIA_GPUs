# NVIDIA GPU Architectures

Deep technical tour of NVIDIA GPUs from Pascal to Blackwell &mdash; SMs, tensor cores, memory hierarchy, NVLink, packaging, power, plus per-architecture low-level deep dives and the DGX Spark workstation.

**Live index:** https://brendanjameslynskey.github.io/LLM_Hub_NVIDIA_GPUs/

## Presentations in this series

| # | Title | Status | Description |
|---|-------|--------|-------------|
| 01 | [The NVIDIA GPU Family Tree — Pascal to Blackwell](https://brendanjameslynskey.github.io/NVIDIA_GPU_01_Architecture_Overview/) | live | Family timeline, process nodes, dies, transistor counts, memory types and what each generation unlocked. Interactive family explorer. |
| 02 | [Inside the SM — How NVIDIA's Streaming Multiprocessor Evolved](https://brendanjameslynskey.github.io/NVIDIA_GPU_02_SM_Evolution/) | live | SM internals across Pascal, Volta, Turing, Ampere, Hopper, Ada and Blackwell — schedulers, register file, tensor cores, TMA, clusters. |
| 03 | [Tensor Cores — Five Generations](https://brendanjameslynskey.github.io/NVIDIA_GPU_03_Tensor_Cores/) | live | Every generation from Volta's 4×4×4 FP16 to Blackwell's MX-FP4 — formats, MMA shapes, sparsity, Transformer Engine. |
| 04 | [Memory Hierarchy](https://brendanjameslynskey.github.io/NVIDIA_GPU_04_Memory_Hierarchy/) | live | Registers, shared, L1/L2, HBM2e/3/3e, GDDR6/6X/7, LPDDR5x unified, Hopper TMA. Decode-speed estimator. |
| 05 | [NVLink &amp; NVSwitch](https://brendanjameslynskey.github.io/NVIDIA_GPU_05_NVLink_NVSwitch/) | live | Scale-up interconnect from NVLink 1 (Pascal) to NVLink 5 (NVL72), NVLink-C2C, the rack-scale superpod. |
| 06 | [Ampere — A100, RTX 30, the LLM Era](https://brendanjameslynskey.github.io/NVIDIA_GPU_06_Ampere/) | live | GA100 + GA10x — 3rd-gen tensor cores (TF32, BF16, 2:4 sparsity), MIG, NVLink 3 with NVSwitch 2. |
| 07 | [Hopper — H100, FP8, Transformer Engine](https://brendanjameslynskey.github.io/NVIDIA_GPU_07_Hopper/) | live | GH100, H100/H200/GH200 — 4th-gen tensor cores, native FP8, TMA, thread-block clusters and DSMEM, DPX, NVLink 4. |
| 08 | [Ada Lovelace — RTX 40, L40S, Consumer-Class AI](https://brendanjameslynskey.github.io/NVIDIA_GPU_08_Ada_Lovelace/) | live | AD102 + RTX 40 / L40S / L4 — 4th-gen RT cores, DLSS 3, the FP8 split, no-NVLink consequences. |
| 09 | [Blackwell — Dual-Die, FP4, NVL72](https://brendanjameslynskey.github.io/NVIDIA_GPU_09_Blackwell/) | live | B100/B200/GB200 — dual-die NV-HBI, 5th-gen tensor cores with MX-FP4, 2nd-gen Transformer Engine, RAS engine, NVLink 5, NVL72 superpod. |
| 10 | [Software Stack &amp; Performance](https://brendanjameslynskey.github.io/NVIDIA_GPU_10_Software_and_Performance/) | live | CUDA stack — driver, cuBLAS, cuDNN, CUTLASS, Transformer Engine, NCCL, Triton, TensorRT-LLM. End-to-end LLM tok/s calculator. |
| 11 | [DGX, HGX, MGX — Datacenter Reference Platforms](https://brendanjameslynskey.github.io/NVIDIA_GPU_11_Datacenter_Platforms/) | live | Datacenter platforms, OAM, BasePOD and SuperPOD blueprints, NVL72, the OEM ecosystem and DGX Cloud. |
| 12 | [GeForce, RTX Pro, Tesla, A/H/L/B — Decoding the Lineup](https://brendanjameslynskey.github.io/NVIDIA_GPU_12_Consumer_Workstation_Products/) | live | Field guide to every NVIDIA product family — naming logic, EULA boundaries, driver branches, the same-die-different-card patterns. |
| 13 | [Networking — InfiniBand, ConnectX, BlueField](https://brendanjameslynskey.github.io/NVIDIA_GPU_13_Networking_InfiniBand_BlueField/) | live | Cross-node fabric — ConnectX HCAs, Quantum IB and Spectrum-X switches, BlueField DPUs, GPUDirect RDMA / Storage, NCCL, SHARP. |
| 14 | [PCIe &amp; GPUDirect](https://brendanjameslynskey.github.io/NVIDIA_GPU_14_PCIe_and_GPUDirect/) | live | PCIe 3 to 6, Resizable BAR, IOMMU, ACS, NUMA pinning, GPUDirect P2P/RDMA/Storage. Topology lint. |
| 15 | [Grace — NVIDIA's ARM CPU, GH200, GB200](https://brendanjameslynskey.github.io/NVIDIA_GPU_15_Grace_CPU_and_GH_GB/) | live | Grace 72-core Neoverse V2, NVLink-C2C 900 GB/s, GH200, GB200, Extended GPU Memory, DGX Spark. |
| 16 | [Jetson — Edge AI &amp; Robotics](https://brendanjameslynskey.github.io/NVIDIA_GPU_16_Jetson_and_Edge/) | live | Orin Nano (7W) through AGX Orin (60W) and Jetson Thor — JetPack, L4T, Holoscan, Isaac, DeepStream. |
| 17 | [Profiling &amp; Debug — Nsight, NVTX, CUPTI](https://brendanjameslynskey.github.io/NVIDIA_GPU_17_Profiling_and_Debug/) | live | Nsight Systems, Nsight Compute, NVTX, CUPTI, DCGM, nvbandwidth — workflow from 'cluster slow' to 'fix line 42'. |
| 18 | [Sharing the GPU — MIG, MPS, vGPU](https://brendanjameslynskey.github.io/NVIDIA_GPU_18_GPU_Sharing_MIG_MPS_vGPU/) | live | Hardware-partitioned MIG, MPS multiplexing, vGPU virtualisation, Kubernetes time-slicing — isolation, performance, licensing trade-offs. |
| 19 | [TensorRT-LLM — NVIDIA's Optimised Inference Engine](https://brendanjameslynskey.github.io/NVIDIA_GPU_19_TensorRT_LLM/) | live | Engine builder, in-flight batching, paged KV-cache, FP8/FP4 quantisation, speculative decoding, TP/PP/EP. |
| 20 | [NeMo, NIM &amp; AI Enterprise](https://brendanjameslynskey.github.io/NVIDIA_GPU_20_NeMo_NIM_AI_Enterprise/) | live | NeMo Framework, Aligner (RLHF/DPO/PPO), Curator, Guardrails, NIM microservices, Base Command, Run.ai, AI Enterprise bundle. |
| 21 | [PTX &amp; SASS — The Real GPU ISAs](https://brendanjameslynskey.github.io/NVIDIA_GPU_21_PTX_and_SASS/) | live | PTX portable IR and per-arch SASS — HMMA / WGMMA tensor-core ops, LDMATRIX, BAR.SYNC, predication, ptxas optimisations. |
| 22 | [Warp Scheduling &amp; SIMT](https://brendanjameslynskey.github.io/NVIDIA_GPU_22_Warp_Scheduling_SIMT/) | live | SM partitions, warp schedulers, instruction latencies, occupancy vs ILP, divergence, predication, independent thread scheduling. |
| 23 | [HBM Internals](https://brendanjameslynskey.github.io/NVIDIA_GPU_23_HBM_Internals/) | live | HBM2e/3/3e/4 internals — TSVs, channels and pseudo-channels, banks, refresh, ECC modes, the HBM PHY, CoWoS packaging. |
| 24 | [Power &amp; Thermal — 1000 W on a Card](https://brendanjameslynskey.github.io/NVIDIA_GPU_24_Power_and_Thermal/) | live | 12V-2x6, multi-phase VRMs, multi-rail, transient response, GPU Boost, P-states, vapour chambers, direct-to-chip liquid cooling. |
| 25 | [Process &amp; Packaging](https://brendanjameslynskey.github.io/NVIDIA_GPU_25_Process_and_Packaging/) | live | TSMC process lineage 16FF to N3/A16, 830 mm² reticle limit, NV-HBI, CoWoS-S/L/R, defect density, the CoWoS supply bottleneck. |
| 26 | [Inside Pascal — First HBM &amp; NVLink](https://brendanjameslynskey.github.io/NVIDIA_GPU_26_Pascal_Low_Level/) | live | GP100 (P100) and GP102/104/106 — block diagram, FP-heavy SM, FP16x2 packed math, TSMC 16FF+, HBM2, GDDR5X, NVLink 1.0. |
| 27 | [Inside Volta — First Tensor Cores](https://brendanjameslynskey.github.io/NVIDIA_GPU_27_Volta_Low_Level/) | live | GV100 — TSMC 12FF, four-partition SM with split FP/INT, first-gen tensor cores at 125 TFLOPS, independent thread scheduling, NVLink 2.0 / NVSwitch 1. |
| 28 | [Inside Turing — RT Cores, INT8/INT4 Tensor Cores](https://brendanjameslynskey.github.io/NVIDIA_GPU_28_Turing_Low_Level/) | live | TU102/104/106/116/117 — 1st-gen RT cores, 2nd-gen tensor cores (INT8/INT4), GDDR6, NVLink 2.0 bridge, Tesla T4. |
| 29 | [Inside Ampere — 3rd-Gen Tensor Cores, MIG](https://brendanjameslynskey.github.io/NVIDIA_GPU_29_Ampere_Low_Level/) | live | GA100 (TSMC 7N) and GA10x (Samsung 8N), TF32/BF16/2:4 sparsity, the 40 MB L2 leap, async copy, MIG, NVLink 3.0. |
| 30 | [Inside Ada — AD102, 96 MB L2, 4th-Gen RT](https://brendanjameslynskey.github.io/NVIDIA_GPU_30_Ada_Low_Level/) | live | AD102–107 on TSMC 4N — doubled-FP32 SM, 4th-gen tensor cores, 4th-gen RT with OMM/DMM, OFA, 96 MB L2, GDDR6X, the 12VHPWR saga. |
| 31 | [Inside Hopper — FP8, TMA, Clusters](https://brendanjameslynskey.github.io/NVIDIA_GPU_31_Hopper_Low_Level/) | live | GH100 / H100 / H200 / GH200 — 4th-gen tensor cores at 1979 TFLOPS, WGMMA, TMA, thread-block clusters and DSMEM, DPX, NVLink 4. |
| 32 | [Inside Blackwell — Dual-Die, MX-FP4, NVLink 5](https://brendanjameslynskey.github.io/NVIDIA_GPU_32_Blackwell_Low_Level/) | live | Dual-die B100/B200 with NV-HBI on CoWoS-L, 5th-gen tensor cores at 9 PFLOPS MX-FP4, 2nd-gen Transformer Engine, NVLink 5, NVL72, RTX 50. |
| 33 | [Inside the DGX Spark — GB10 Hardware](https://brendanjameslynskey.github.io/NVIDIA_GPU_33_DGX_Spark_Hardware/) | live | GB10 SoC with 20 ARM cores + Blackwell GPU, NVLink-C2C, 128 GB unified LPDDR5x at 273 GB/s, ~1 PFLOP sparse FP4 at 170 W. |
| 34 | [Setting Up DGX Spark](https://brendanjameslynskey.github.io/NVIDIA_GPU_34_DGX_Spark_Setup/) | live | Unboxing, OOBE, DGX OS (Ubuntu ARM64), CUDA toolkit, Container Toolkit, SSH, networking, NGC login, first NIM/Ollama/vLLM model. |
| 35 | [LLM Inference on DGX Spark — Numbers](https://brendanjameslynskey.github.io/NVIDIA_GPU_35_DGX_Spark_Inference/) | live | Realistic tok/s 1B&ndash;671B, framework choice (Ollama/vLLM/NIM/TRT-LLM), quant choice (BF16/FP8/MX-FP4/AWQ-INT4), KV placement. |
| 36 | [DGX Spark Development Workflow](https://brendanjameslynskey.github.io/NVIDIA_GPU_36_DGX_Spark_DevWorkflow/) | live | VS Code Remote SSH, NGC containers, PyTorch on ARM64, JupyterHub, QLoRA at 70B, dataset streaming, HF→MX-FP4→NIM, custom Triton. |
| 37 | [DGX Spark vs Alternatives](https://brendanjameslynskey.github.io/NVIDIA_GPU_37_DGX_Spark_vs_Alternatives/) | live | Mac Studio M3 Ultra, RTX 5090, RTX PRO 6000 Blackwell, used DGX Station A100, cloud H100/B200, two-Spark pair — capacity, bandwidth, cost-per-token. |

## Where this fits

Part of the [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) &mdash; an index of presentation series for AI/LLM engineers.
