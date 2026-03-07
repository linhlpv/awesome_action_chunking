# Awesome Action Chunking in Reinforcement Learning
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

A curated list of papers on **action chunking**, **chunked control**, **action-sequence policies**, and **macro-actions** in reinforcement learning, offline RL, imitation learning, and robot learning.  If you find this repository helpful, please consider giving it a ⭐!

This list was initialized on **March 7, 2026**. Accepted papers are organized by **year -> venue**. Preprints stay in **Preprints / Under Review** until an official venue acceptance is verified. The entries below were re-audited on **March 7, 2026** against official proceedings pages, OpenReview forum pages, arXiv records, and DOI landing pages.

Maintainer:
- [Linh Le](https://linhlpv.github.io/) (A2I2, Deakin University)

Please feel free to open an issue or submit a pull request by following [CONTRIBUTING.md](./CONTRIBUTING.md).

## 📑 Citation

```bibtex
@article{le2026actionchunking,
  title={Awesome Action Chunking Papers},
  author={Linh Le},
  journal={https://github.com/linhlpv/awesome-action-chunking},
  year={2026}
}
```

## Scope

- Focus on papers where predicting, evaluating, or executing **multi-step action chunks** is central.
- Include explicit action chunking papers and a small number of canonical adjacent papers such as **ACT**, **Diffusion Policy**, **BeT**, and **BAKU** that are frequently used as baselines or building blocks in this literature.
- Keep older options, macro-actions, and temporal abstraction papers in a separate **Foundations and Related Work** section.
- Exclude generic planning or policy papers where chunked actions are not a meaningful part of the method.

## Table of Contents

- [Preprints / Under Review](#preprints--under-review)
- [2026](#2026)
- [2025](#2025)
- [2024](#2024)
- [2023](#2023)
- [2022](#2022)
- [Other Relevant Non-Top-Tier / Workshop Papers](#other-relevant-non-top-tier--workshop-papers)
- [Foundations and Related Work](#foundations-and-related-work)
- [Contributing](#contributing)

## Preprints / Under Review

### 2026

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [SEAR: Sample Efficient Action Chunking Reinforcement Learning](https://arxiv.org/abs/2603.01891) | SEAR | 2026/03 | Online RL, long-horizon manipulation | - | arXiv 2026 |
| [Learning Native Continuation for Action Chunking Flow Policies](https://arxiv.org/abs/2602.12978) | Legato | 2026/02 | Real-time flow/VLA control | - | arXiv 2026 |
| [Sample-Efficient Real-World Dexterous Policy Fine-Tuning via Action-Chunked Critics and Normalizing Flows](https://arxiv.org/abs/2602.09580) | SOFT-FLOW | 2026/02 | Dexterous real-world RL fine-tuning | - | arXiv 2026 |

### 2025

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Decoupled Q-Chunking](https://arxiv.org/abs/2512.10926) | DQC | 2025/12 | Offline-to-online RL, long-horizon manipulation | [Code](https://github.com/ColinQiyangLi/dqc) | arXiv 2025 |
| [Mixture of Horizons in Action Chunking](https://arxiv.org/abs/2511.19433) | MoH | 2025/11 | VLA, long-horizon manipulation | [Code](https://github.com/Timsty1/MixtureOfHorizons) | arXiv 2025 |
| [Temporal Action Selection for Action Chunking](https://arxiv.org/abs/2511.04421) | TAS | 2025/11 | Imitation learning, reactive control | - | arXiv 2025 |
| [VLA Model Post-Training via Action-Chunked PPO and Self Behavior Cloning](https://arxiv.org/abs/2509.25718) | Action-Chunked PPO + SBC | 2025/09 | VLA post-training, RL | - | arXiv 2025 |
| [Leave No Observation Behind: Real-time Correction for VLA Action Chunks](https://arxiv.org/abs/2509.23224) | A2C2 | 2025/09 | VLA, real-time chunk correction | - | arXiv 2025 |
| [CO-RFT: Efficient Fine-Tuning of Vision-Language-Action Models through Chunked Offline Reinforcement Learning](https://arxiv.org/abs/2508.02219) | Chunked RL | 2025/08 | VLA fine-tuning, offline RL | - | arXiv 2025 |
| [Learning Bimanual Manipulation via Action Chunking and Inter-Arm Coordination with Transformers](https://arxiv.org/abs/2503.13916) | Inter-arm ACT | 2025/03 | Bimanual manipulation | - | arXiv 2025 |

### 2024

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [VQ-ACE: Efficient Policy Search for Dexterous Robotic Manipulation via Action Chunking Embedding](https://arxiv.org/abs/2411.03556) | VQ-ACE | 2024/11 | Dexterous manipulation, RL/MPC | - | arXiv 2024 |

## 2026

### AAAI 2026

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Actor-Critic for Continuous Action Chunks: A Reinforcement Learning Framework for Long-Horizon Robotic Manipulation with Sparse Reward](https://arxiv.org/abs/2508.11143) | AC3 | 2025/08 | Sparse-reward robotic manipulation | - | AAAI 2026 |

### ICLR 2026

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Action Chunking and Data Augmentation Yield Exponential Improvements for Imitation Learning in Continuous Spaces](https://openreview.net/forum?id=jiWXDvw1Lf) | AC theory | 2026/01 | Theory + imitation learning, continuous control | - | ICLR 2026 |
| [Real-Time Robot Execution with Masked Action Chunking](https://arxiv.org/abs/2601.20130) | REMAC | 2026/01 | Real-time VLA, robot manipulation | - | ICLR 2026 |
| [Scalable Offline Model-Based RL with Action Chunks](https://arxiv.org/abs/2512.08108) | MAC | 2025/12 | Offline model-based RL, long-horizon control | - | ICLR 2026 |
| [Chunking the Critic: A Transformer-based Soft Actor-Critic with N-Step Returns](https://arxiv.org/abs/2503.03660) | T-SAC | 2025/03 | Off-policy RL, long-horizon control | - | ICLR 2026 |

## 2025

### NeurIPS 2025

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Reinforcement Learning with Action Chunking](https://arxiv.org/abs/2507.07969) | Q-chunking | 2025/07 | Offline-to-online RL, long-horizon manipulation | [Code](https://github.com/ColinQiyangLi/qc) | NeurIPS 2025 |
| [Real-Time Execution of Action Chunking Flow Policies](https://arxiv.org/abs/2506.07339) | RTC | 2025/06 | Real-time VLA, asynchronous execution | [Code](https://github.com/Physical-Intelligence/real-time-chunking-kinetix) | NeurIPS 2025 |

### IROS 2025

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [PD-VLA: Accelerating Vision-Language-Action Model Integrated with Action Chunking via Parallel Decoding](https://arxiv.org/abs/2503.02310) | PD-VLA | 2025/03 | VLA acceleration, robot manipulation | - | IROS 2025 |

### ICLR 2025

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Bidirectional Decoding: Improving Action Chunking via Guided Test-Time Sampling](https://arxiv.org/abs/2408.17355) | BID | 2024/08 | Robot imitation learning, chunk reactivity | [Code](https://github.com/Jubayer-Hamid/bid_lerobot) | ICLR 2025 |

## 2024

### NeurIPS 2024

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [BAKU: An Efficient Transformer for Multi-Task Policy Learning](https://arxiv.org/abs/2406.07539) | BAKU | 2024/06 | Multi-task robot policy learning | [Code](https://github.com/siddhanthaldar/BAKU) | NeurIPS 2024 |

### CoRL 2024

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [InterACT: Inter-dependency Aware Action Chunking with Hierarchical Attention Transformers for Bimanual Manipulation](https://arxiv.org/abs/2409.07914) | InterACT | 2024/09 | Bimanual manipulation | - | CoRL 2024 |

## 2023

### RSS 2023

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware](https://arxiv.org/abs/2304.13705) | ACT | 2023/04 | Fine-grained bimanual manipulation | [Code](https://github.com/tonyzhaozh/act) | RSS 2023 |
| [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/abs/2303.04137) | Diffusion Policy | 2023/03 | Visuomotor control, receding-horizon action sequences | [Code](https://github.com/real-stanford/diffusion_policy) | RSS 2023 |

## 2022

### NeurIPS 2022

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Behavior Transformers: Cloning $k$ modes with one stone](https://arxiv.org/abs/2206.11251) | BeT | 2022/06 | Behavior cloning, multimodal action chunks | [Code](https://github.com/notmahi/bet) | NeurIPS 2022 |

## Other Relevant Non-Top-Tier / Workshop Papers

These papers are directly relevant, but they are not currently part of the main top-tier accepted-paper timeline above.

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [ExACT: An End-to-End Autonomous Excavator System Using Action Chunking With Transformers](https://arxiv.org/abs/2405.05861) | ExACT | 2024/05 | Autonomous excavation, imitation learning | - | ICRA Workshop 2024 |
| [Bi-ACT: Bilateral Control-Based Imitation Learning via Action Chunking with Transformer](https://arxiv.org/abs/2401.17698) | Bi-ACT | 2024/01 | Bilateral imitation learning | - | AIM 2024 |
| [RoboAgent: Towards Sample Efficient Robot Manipulation with Semantic Augmentations and Action Chunking](https://robot-learning.ml/2023/files/paper39.pdf) | MT-ACT / RoboAgent | 2023/12 | Multi-task robot manipulation | - | NeurIPS 2023 Workshop on Robot Learning |
| [One ACT Play: Single Demonstration Behavior Cloning with Action Chunking Transformers](https://arxiv.org/abs/2309.10175) | One ACT Play | 2023/09 | Single-demo behavior cloning | - | arXiv 2023 |

## Foundations and Related Work

This section is intentionally selective. It captures foundational temporal abstraction, macro-action, and hierarchical RL papers that are useful background for action chunking research.

| Paper | Method | Date | Domain/Task | Code | Venue |
| --- | --- | --- | --- | --- | --- |
| [Macro-Action-Based Deep Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2004.08646) | MacDec RL | 2020/04 | Multi-agent RL, asynchronous macro-actions | - | CoRL 2019 |
| [Data-Efficient Hierarchical Reinforcement Learning](https://arxiv.org/abs/1805.08296) | HIRO | 2018/05 | Hierarchical RL, continuous control | - | NeurIPS 2018 |
| [FeUdal Networks for Hierarchical Reinforcement Learning](https://proceedings.mlr.press/v70/vezhnevets17a.html) | FeUdal Networks | 2017/03 | Hierarchical RL, long-horizon credit assignment | - | ICML 2017 |
| [The Option-Critic Architecture](https://arxiv.org/abs/1609.05140) | Option-Critic | 2016/09 | Options, temporal abstraction | - | AAAI 2017 |
| [Deep Reinforcement Learning With Macro-Actions](https://arxiv.org/abs/1606.04615) | Deep RL + macro-actions | 2016/06 | Deep RL, Atari, temporal abstraction | - | arXiv 2016 |
| [Hierarchical Reinforcement Learning with the MAXQ Value Function Decomposition](https://doi.org/10.1613/jair.639) | MAXQ | 2000/05 | Hierarchical RL, value decomposition | - | JAIR 2000 |
| [Between MDPs and Semi-MDPs: A Framework for Temporal Abstraction in Reinforcement Learning](https://doi.org/10.1016/S0004-3702%2899%2900052-1) | Options framework | 1999/08 | Temporal abstraction, semi-MDPs | - | Artificial Intelligence 1999 |

## Contributing

Please follow [CONTRIBUTING.md](./CONTRIBUTING.md). Pull requests for missing papers, fixed venues, broken links, and code repositories are welcome.

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=linhlpv/awesome-action-chunking&type=Date)](https://star-history.com/#linhlpv/awesome-action-chunking&Date)
