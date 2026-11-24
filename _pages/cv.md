---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description:
toc:
  sidebar: left
---

## Research Interests

Machine Learning Systems; Efficient Serving of Large Language Models and Video Generation / World Models; KV-Cache and State Management; Memory-Efficient Generative Systems.

## Education

**University of California, Los Angeles (UCLA)** — Los Angeles, CA<br>
_M.S. in Computer Science_ · GPA 3.95/4.00 · Sep. 2025 – Present

**University of California, Los Angeles (UCLA)** — Los Angeles, CA<br>
_B.S. in Computer Science_ · GPA 3.75/4.00 · Sep. 2021 – Mar. 2025

## Research Experience

**BranchFlow: State Management for Interactive Video Generation**<br>
_UCLA & DiDi Global_ · Los Angeles, CA / Beijing, China · Jun. 2026 – Present

- Led the project and proposed _BranchFlow_, a new serving abstraction for interactive video generation that enables _arbitrary-time rollback_, branching, and exact resumption without retaining the full historical KV cache.
- Showed that tracking KV at model-layer granularity bounds the cost of restoring any historical state independently of history length; built on this a hierarchical state cache with layer-wise eviction and storage policies.
- Extended the evaluation from user-driven rollback to state-restoration scenarios, designing a workload and evaluation for each scenario.

**AdaptiveRL: Serving Adaptively Layer-Skipped LLMs**<br>
_DiDi Global_ · Beijing, China · Aug. 2026 – Present

- Led the serving-side research for AdaptiveRL, investigating when algorithm-level computation savings from adaptive layer skipping can translate into end-to-end LLM serving gains.
- Identified system overheads, developed a serving design that preserves its computational advantage under continuous batching and inference workloads, and conducted experiments from open source traces.

**Pythia: Efficient Agent-Native LLM Serving**<br>
_UCLA_ · Los Angeles, CA · Mar. 2026 – Apr. 2026

- Contributed to the experimental evaluation of an LLM serving system that exploits workflow predictability in multi-step agentic workloads.
- Implemented and tested a workflow prediction algorithm using collected agentic traces.

**Self-Evolving LLM Agents: Closing the Discovery-to-Application Loop**<br>
_UCLA_ · Los Angeles, CA · Jul. 2025 – Dec. 2025

- Developed an autonomous-agent framework for recursively verifying intermediate results and iteratively refining solutions in open-ended tasks.
- Conducted systematic benchmarking and failure analysis using Minecraft as a case to study whether current agents can transfer discovered knowledge into successful downstream task execution.

## Industry Experience

**DiDi Global** · _Machine Learning Research Intern_ · Jun. 2026 – Sep. 2026

- Researched World-Action Models, focusing on infrastructure optimization and serving-pipeline design for generative models.
- Contributed to the VeRL framework by integrating audio and image support for Omni-family models and maintaining CI/CD infrastructure.

**VMware** · _Machine Learning Engineer Intern_ · Jun. 2023 – Sep. 2023

- Improved machine translation through K-BERT and automatic post-editing (APE) integration, evaluating translation quality using COMET.
- Developed a code-assistance prototype using the OpenAI API and self-designed vector databases, automating code suggestions through prompt engineering.

**Momenta** · _R&D Intern_ · Jun. 2022 – Sep. 2022

- Designed road tests to evaluate perception algorithms for the Mpilot Level 1 autonomous-driving system.
- Developed Python tools to analyze satellite data collected from road-test videos and support system evaluation.

## Open-Source Contributions

**[VeRL](https://github.com/verl-project/verl) / [VeRL-Omni](https://github.com/verl-project/verl-omni)** · _Open-Source Contributor_ · Mar. 2026 – Sep. 2026

- Added Qwen2.5-Omni model-bridge support to Megatron-Bridge, enabling integration of the multimodal model into the distributed training framework ([PR #2296](https://github.com/NVIDIA-NeMo/Megatron-Bridge/pull/2296)).
- Contributed end-to-end support for fully asynchronous RL with Qwen3-Omni audio models in VeRL-Omni, spanning model integration, rollout, data processing, and testing ([PR #413](https://github.com/verl-project/verl-omni/pull/413)).

**[vLLM-Omni](https://github.com/vllm-project/vllm-omni)** · _Open-Source Contributor_ · Oct. 2026 – Present

- Designing writer election and a sealed, read-only `memfd` host store, so that worker processes on one node share a single host copy of model weights instead of each loading its own; covered by multiprocess CPU tests and A100 end-to-end tests.

## Publications

See the [Publications](/publications/) page.
