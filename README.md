# Diffusion Language Models — Categorized

_404 papers, auto-categorized by topic. Counts indicate papers per category; categories are first-match.
Spot-check abstracts in `out/diffusion_lm_full.json` to verify._

## Summary

- **survey** (2): Surveys / tutorials / position papers (TITLE-only).
- **safety-privacy** (16): Memorization / data extraction / privacy / watermarking / backdoor / jailbreak.
- **domain-applications** (18): Non-language domains (molecular / robotics / time series / KG / recommender / scientific) — TITLE-only so we don't catch papers that merely mention an app.
- **multimodal** (17): Vision-language / multimodal diffusion.
- **reasoning** (80): Reasoning / math / code / planning capability of diffusion LMs.
- **rl-alignment** (43): RL / preference / reward / alignment for diffusion LMs.
- **controllable-generation** (21): Controllable / conditional / constrained generation; infilling; editing.
- **theory-analysis** (22): Theory, likelihood, convergence, sample complexity, comparison studies.
- **hybrid-architecture** (31): Hybrid AR+diffusion or novel architectures (block/latent/flow/state-space).
- **training-objective** (35): Training objectives, schedules, pretraining recipes, fine-tuning method.
- **sampling-efficiency** (58): Faster inference: fewer steps, parallel decoding, KV cache, distillation for speed.
- **benchmarks-evaluation** (2): New benchmarks or evaluation methodologies.
- **other** (59): Did not match any category — manual review needed.

## survey (2)

_Surveys / tutorials / position papers (TITLE-only)._

- [2026/03] **Advances in GRPO for Generation Models: A Survey** *arXiv* [[paper](https://arxiv.org/abs/2603.06623)]
  <sub>Large-scale flow matching models have achieved strong performance across generative tasks such as text-to-image, video, 3D, and speech synthesis. However, aligning their outputs with human preferences…</sub>
- [2025/07] **A Survey on Latent Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2507.06203)]
  <sub>Large Language Models (LLMs) have demonstrated impressive reasoning capabilities, especially when guided by explicit chain-of-thought (CoT) reasoning that verbalizes intermediate steps. While CoT impr…</sub>

## safety-privacy (16)

_Memorization / data extraction / privacy / watermarking / backdoor / jailbreak._

- [2026/05] **Extracting Training Data from Diffusion Language Models via Infilling** *arXiv* [[paper](https://arxiv.org/abs/2605.24173)]
  <sub>Memorization in large language models has been studied almost exclusively through prefix-conditioned extraction, a natural choice for autoregressive models. However, diffusion language models (DLMs) c…</sub>
- [2026/05] **Backdooring Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.19262)]
  <sub>Masked diffusion language models (MDLMs) are emerging as a compelling new paradigm for text generation, but their training-time security remains largely unexplored. Existing backdoor attacks on Gaussi…</sub>
- [2026/05] **Machine Unlearning for Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.18253)]
  <sub>Recent masked diffusion language models (MDLMs), such as LLaDA and Dream, have achieved performance comparable to autoregressive large language models. Unlike autoregressive models, which generate tex…</sub>
- [2026/05] **Membership Inference Attacks on Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.16445)]
  <sub>Masked Diffusion Language Models MDLMs replace autoregressive generation with iterative demasking and their privacy properties are largely unstudied. We study membership inference attacks MIA on fine…</sub>
- [2026/05] **Adaptive Steering and Remasking for Safe Generation in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.13043)]
  <sub>Diffusion Language Models (DLMs) provide a promising alternative to autoregressive language models by generating text through iterative denoising and bidirectional refinement. However, this iterative…</sub>
- [2026/05] **TrajDLM: Topology-Aware Block Diffusion Language Model for Trajectory Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.10020)]
  <sub>Generating high-fidelity synthetic GPS trajectories is increasingly important for applications in transportation, urban planning, and what-if scenario simulation, especially as privacy concerns limit…</sub>
- [2026/05] **The Safety-Aware Denoiser for Text Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2605.08116)]
  <sub>Recent work on text diffusion models offers a promising alternative to autoregressive generation, but controlling their safety remains underexplored. Existing safety approaches are geared toward autor…</sub>
- [2026/05] **Conditional generation of antibody sequences with classifier-guided germline-absorbing discrete diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.06720)]
  <sub>Antibody therapeutics are among the most successful modern medicines, yet computationally designing antibodies with desirable binding and developability properties remains challenging. While protein l…</sub>
- [2026/05] **Chainwash: Multi-Step Rewriting Attacks on Diffusion Language Model Watermarks** *arXiv* [[paper](https://arxiv.org/abs/2605.05503)]
  <sub>Statistical watermarking is a common approach for verifying whether text was written by a language model. Most existing schemes assume autoregressive generation, where tokens are produced left to righ…</sub>
- [2026/04] **Language Diffusion Models are Associative Memories Capable of Retrieving Unseen Data** *arXiv* [[paper](https://arxiv.org/abs/2604.26841)]
  <sub>When do language diffusion models memorize their training data, and how to quantitatively assess their true generative regime? We address these questions by showing that Uniform-based Discrete Diffusi…</sub>
- [2026/03] **Characterizing Memorization in Diffusion Language Models: Generalized Extraction and Sampling Effects** *arXiv* [[paper](https://arxiv.org/abs/2603.02333)]
  <sub>Autoregressive language models (ARMs) have been shown to memorize and occasionally reproduce training data verbatim, raising concerns about privacy and copyright liability. Diffusion language models (…</sub>
- [2026/02] **Self-Purification Mitigates Backdoors in Multimodal Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.22246)]
  <sub>Multimodal Diffusion Language Models (MDLMs) have recently emerged as a competitive alternative to their autoregressive counterparts. Yet their vulnerability to backdoor attacks remains largely unexpl…</sub>
- [2026/02] **Step-Wise Refusal Dynamics in Autoregressive and Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.02600)]
  <sub>Diffusion language models (DLMs) have recently emerged as a promising alternative to autoregressive (AR) models, offering parallel decoding and controllable sampling dynamics while achieving competiti…</sub>
- [2026/01] **LR-DWM: Efficient Watermarking for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.12376)]
  <sub>Watermarking (WM) is a critical mechanism for detecting and attributing AI-generated content. Current WM methods for Large Language Models (LLMs) are predominantly tailored for autoregressive (AR) mod…</sub>
- [2025/07] **Jailbreaking Large Language Diffusion Models: Revealing Hidden Safety Flaws in Diffusion-Based Text Generation** *arXiv* [[paper](https://arxiv.org/abs/2507.19227)]
  <sub>Large Language Diffusion Models (LLDMs) exhibit comparable performance to LLMs while offering distinct advantages in inference speed and mathematical reasoning tasks.The precise and rapid generation c…</sub>
- [2025/06] **Agentic Surgical AI: Surgeon Style Fingerprinting and Privacy Risk Quantification via Discrete Diffusion in a Vision-Language-Action Framework** *arXiv* [[paper](https://arxiv.org/abs/2506.08185)]
  <sub>Surgeons exhibit distinct operating styles shaped by training, experience, and motor behavior-yet most surgical AI systems overlook this personalization signal. We propose a novel agentic modeling app…</sub>

## domain-applications (18)

_Non-language domains (molecular / robotics / time series / KG / recommender / scientific) — TITLE-only so we don't catch papers that merely mention an app._

- [2026/05] **Generative Representation Learning on Hyper-relational Knowledge Graphs via Masked Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.24064)]
  <sub>Hyper-relational knowledge graphs (HKGs) effectively represent complex facts. While inferring new knowledge in HKGs is a critical problem, current methods cast it as a simple link prediction, assuming…</sub>
- [2026/05] **SCRIPT: Scalable Diffusion Policy with Multi-stage Training for Language-driven Physics-based Humanoid Control** *arXiv* [[paper](https://arxiv.org/abs/2605.22894)]
  <sub>Controlling physics-based humanoids from natural-language instructions is a critical step toward general-purpose embodied agents. However, existing methods remain constrained by a tension between sema…</sub>
- [2026/05] **Towards A Generative Protein Evolution Machine with DPLM-Evo** *arXiv* [[paper](https://arxiv.org/abs/2605.00182)]
  <sub>Proteins are shaped by gradual evolution under biophysical and functional constraints. Protein language models learn rich evolutionary constraints from large-scale sequences, and discrete diffusion-ba…</sub>
- [2026/04] **RADD: Retrieval-Augmented Discrete Diffusion for Multi-Modal Knowledge Graph Completion** *arXiv* [[paper](https://arxiv.org/abs/2604.25693)]
  <sub>Most multi-modal knowledge graph completion (MMKGC) models use one embedding scorer to do both retrieval over the full entity set and final decision making. We argue that this coupling is a core bottl…</sub>
- [2026/04] **One Pass for All: A Discrete Diffusion Model for Knowledge Graph Triple Set Prediction** *arXiv* [[paper](https://arxiv.org/abs/2604.18344)]
  <sub>Knowledge Graphs (KGs) are composed of triples, and the goal of Knowledge Graph Completion (KGC) is to infer the missing factual triples. Traditional KGC tasks predict missing elements in a triple giv…</sub>
- [2026/04] **FRIGID: Scaling Diffusion-Based Molecular Generation from Mass Spectra at Training and Inference Time** *arXiv* [[paper](https://arxiv.org/abs/2604.16648)]
  <sub>In this work, we present FRIGID, a framework with a novel diffusion language model that generates molecular structures conditioned on mass spectra via intermediate fingerprint representations and dete…</sub>
- [2026/04] **CAGenMol: Condition-Aware Diffusion Language Model for Goal-Directed Molecular Generation** *arXiv* [[paper](https://arxiv.org/abs/2604.11483)]
  <sub>Goal-directed molecular generation requires satisfying heterogeneous constraints such as protein--ligand compatibility and multi-objective drug-like properties, yet existing methods often optimize the…</sub>
- [2026/04] **MolDA: Molecular Understanding and Generation via Large Language Diffusion Model** *arXiv* [[paper](https://arxiv.org/abs/2604.04403)]
  <sub>Large Language Models (LLMs) have significantly advanced molecular discovery, but existing multimodal molecular architectures fundamentally rely on autoregressive (AR) backbones. This strict left-to-r…</sub>
- [2026/02] **MolHIT: Advancing Molecular-Graph Generation with Hierarchical Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.17602)]
  <sub>Molecular generation with diffusion models has emerged as a promising direction for AI-driven drug discovery and materials science. While graph diffusion models have been widely adopted due to the dis…</sub>
- [2026/02] **Reward-Guided Discrete Diffusion via Clean-Sample Markov Chain for Molecule and Biological Sequence Design** *arXiv* [[paper](https://arxiv.org/abs/2602.09424)]
  <sub>Discrete diffusion models have recently emerged as a powerful class of generative models for chemistry and biology data. In these fields, the goal is to generate various samples with high rewards (e.g…</sub>
- [2025/12] **HD-Prot: A Protein Language Model for Joint Sequence-Structure Modeling with Continuous Structure Tokens** *arXiv* [[paper](https://arxiv.org/abs/2512.15133)]
  <sub>Proteins inherently possess a consistent sequence-structure duality. The abundance of protein sequence data, which can be readily represented as discrete tokens, has driven fruitful developments in pr…</sub>
- [2025/11] **LLaDA-Rec: Discrete Diffusion for Parallel Semantic ID Generation in Generative Recommendation** *arXiv* [[paper](https://arxiv.org/abs/2511.06254)]
  <sub>Generative recommendation represents each item as a semantic ID, i.e., a sequence of discrete tokens, and generates the next item through autoregressive decoding. While effective, existing autoregress…</sub>
- [2025/10] **DiffGRM: Diffusion-based Generative Recommendation Model** *WWW 2025* [[paper](https://arxiv.org/abs/2510.21805)]
  <sub>Generative recommendation (GR) is an emerging paradigm that represents each item via a tokenizer as an n-digit semantic ID (SID) and predicts the next item by autoregressively generating its SID condi…</sub>
- [2025/10] **HyperDiffusionFields (HyDiF): Diffusion-Guided Hypernetworks for Learning Implicit Molecular Neural Fields** *arXiv* [[paper](https://arxiv.org/abs/2510.18122)]
  <sub>We introduce HyperDiffusionFields (HyDiF), a framework that models 3D molecular conformers as continuous fields rather than discrete atomic coordinates or graphs. At the core of our approach is the Mo…</sub>
- [2025/08] **Cross-Modality Controlled Molecule Generation with Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2508.14748)]
  <sub>Current SMILES-based diffusion models for molecule generation typically support only unimodal constraint. They inject conditioning signals at the start of the training process and require retraining a…</sub>
- [2025/05] **CFP-Gen: Combinatorial Functional Protein Generation via Diffusion Language Models** *ICML 2025 poster* [[paper](https://arxiv.org/abs/2505.22869)]
  <sub>Existing PLMs generate protein sequences based on a single-condition constraint from a specific modality, struggling to simultaneously satisfy multiple constraints across different modalities. In this…</sub>
- [2025/05] **MolEditRL: Structure-Preserving Molecular Editing via Discrete Diffusion and Reinforcement Learning** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2505.20131)]
  <sub>Molecular editing aims to modify a given molecule to optimize desired chemical properties while preserving structural similarity. However, current approaches typically rely on string-based or continuo…</sub>
- [2025/02] **Agentic End-to-End De Novo Protein Design for Tailored Dynamics Using a Language Diffusion Model** *arXiv* [[paper](https://arxiv.org/abs/2502.10173)]
  <sub>Proteins are dynamic molecular machines whose biological functions, spanning enzymatic catalysis, signal transduction, and structural adaptation, are intrinsically linked to their motions. Designing p…</sub>

## multimodal (17)

_Vision-language / multimodal diffusion._

- [2026/05] **Inference-Time Alignment of Diffusion Models via Trust-Region Iterative Twisted Sequential Monte Carlo** *arXiv* [[paper](https://arxiv.org/abs/2605.25123)]
  <sub>We study inference-time alignment for diffusion-based generative models, aiming to steer a base model toward high-reward outputs without updating its weights. Recent Sequential Monte Carlo (SMC)-based…</sub>
- [2026/05] **Dependency-Aware Discrete Diffusion for Scene Graph Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.09065)]
  <sub>Scene graphs (SGs) represent objects and their relationships as structured graphs, enabling applications in image generation, robotics, and 3D understanding. Recent work suggests that conditioning ima…</sub>
- [2026/04] **Fast-dVLM: Efficient Block-Diffusion VLM via Direct Conversion from Autoregressive VLM** *arXiv* [[paper](https://arxiv.org/abs/2604.06832)]
  <sub>Vision-language models (VLMs) predominantly rely on autoregressive decoding, which generates tokens one at a time and fundamentally limits inference throughput. This limitation is especially acute in…</sub>
- [2026/04] **Dynin-Omni: Omnimodal Unified Large Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2604.00007)]
  <sub>We present Dynin-Omni, the first masked-diffusion-based omnimodal foundation model that unifies text, image, and speech understanding and generation, together with video understanding, within a single…</sub>
- [2026/03] **Towards GUI Agents: Vision-Language Diffusion Models for GUI Grounding** *arXiv* [[paper](https://arxiv.org/abs/2603.26211)]
  <sub>Autoregressive (AR) vision-language models (VLMs) have long dominated multimodal understanding, reasoning, and graphical user interface (GUI) grounding. Recently, discrete diffusion vision-language mo…</sub>
- [2026/03] **LLaDA-o: An Effective and Length-Adaptive Omni Diffusion Model** *arXiv* [[paper](https://arxiv.org/abs/2603.01068)]
  <sub>We present \textbf{LLaDA-o}, an effective and length-adaptive omni diffusion model for multimodal understanding and generation. LLaDA-o is built on a Mixture of Diffusion (MoD) framework that decouple…</sub>
- [2026/02] **The Design Space of Tri-Modal Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.21472)]
  <sub>Discrete diffusion models have emerged as strong alternatives to autoregressive language models, with recent work initializing and fine-tuning a base unimodal model for bimodal generation. Diverging f…</sub>
- [2026/02] **Analyzing Diffusion and Autoregressive Vision Language Models in Multimodal Embedding Space** *arXiv* [[paper](https://arxiv.org/abs/2602.06056)]
  <sub>Embedding models are a fundamental component of modern AI systems such as semantic search and retrieval-augmented generation. Recent advances in large foundation models have substantially accelerated…</sub>
- [2026/02] **Training-Free Self-Correction for Multimodal Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.02927)]
  <sub>Masked diffusion models have emerged as a powerful framework for text and multimodal generation. However, their sampling procedure updates multiple tokens simultaneously and treats generated tokens as…</sub>
- [2025/12] **Co-GRPO: Co-Optimized Group Relative Policy Optimization for Masked Diffusion Model** *arXiv* [[paper](https://arxiv.org/abs/2512.22288)]
  <sub>Recently, Masked Diffusion Models (MDMs) have shown promising potential across vision, language, and cross-modal generation. However, a notable discrepancy exists between their training and inference…</sub>
- [2025/12] **SDAR-VL: Stable and Efficient Block-wise Diffusion for Vision-Language Understanding** *arXiv* [[paper](https://arxiv.org/abs/2512.14068)]
  <sub>Block-wise discrete diffusion offers an attractive balance between parallel generation and causal dependency modeling, making it a promising backbone for vision-language modeling. However, its practic…</sub>
- [2025/12] **WAM-Diff: A Masked Diffusion VLA Framework with MoE and Online Reinforcement Learning for Autonomous Driving** *arXiv* [[paper](https://arxiv.org/abs/2512.11872)]
  <sub>End-to-end autonomous driving systems based on vision-language-action (VLA) models integrate multimodal sensor inputs and language instructions to generate planning and control signals. While autoregr…</sub>
- [2025/10] **From Denoising to Refining: A Corrective Framework for Vision-Language Diffusion Model** *arXiv* [[paper](https://arxiv.org/abs/2510.19871)]
  <sub>Discrete diffusion models have emerged as a promising direction for vision-language tasks, offering bidirectional context modeling and theoretical parallelization. However, their practical application…</sub>
- [2025/10] **Discrete Diffusion Models with MLLMs for Unified Medical Multimodal Generation** *arXiv* [[paper](https://arxiv.org/abs/2510.06131)]
  <sub>Recent advances in generative medical models are constrained by modality-specific scenarios that hinder the integration of complementary evidence from imaging, pathology, and clinical notes. This frag…</sub>
- [2025/09] **Discrete Diffusion for Reflective Vision-Language-Action Models in Autonomous Driving** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.20109)]
  <sub>End-to-End (E2E) solutions have emerged as a mainstream approach for autonomous driving systems, with Vision-Language-Action (VLA) models representing a new paradigm that leverages pre-trained multimo…</sub>
- [2025/03] **Di$\mathtt{[M]}$O: Distilling Masked Diffusion Models into One-step Generator** *arXiv* [[paper](https://arxiv.org/abs/2503.15457)]
  <sub>Masked Diffusion Models (MDMs) have emerged as a powerful generative modeling technique. Despite their remarkable results, they typically suffer from slow inference with several steps. In this paper,…</sub>
- [2025/03] **POSTA: A Go-to Framework for Customized Artistic Poster Generation** *CVPR 2025* [[paper](https://arxiv.org/abs/2503.14908)]
  <sub>Poster design is a critical medium for visual communication. Prior work has explored automatic poster design using deep learning techniques, but these approaches lack text accuracy, user customization…</sub>

## reasoning (80)

_Reasoning / math / code / planning capability of diffusion LMs._

- [2026/05] **Looped Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.26106)]
  <sub>Masked diffusion models (MDMs) have emerged as a promising alternative to autoregressive models for language modeling, yet the effective design of transformer architectures for MDMs remains underexplo…</sub>
- [2026/05] **The Path Matters: Learning a Token-Commitment Policy for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.24697)]
  <sub>Diffusion large language models promise faster generation by refining many token positions in parallel, but this parallelism introduces a hidden control problem: which proposed tokens should be transf…</sub>
- [2026/05] **Learned Relay Representations for Forward-Thinking Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2605.22967)]
  <sub>When Masked Diffusion Models (MDMs) generate sequences through iterative refinement, the rich internal computation over masked positions is discarded, forcing every subsequent refinement step to recom…</sub>
- [2026/05] **Multi-Token Residual Prediction** *arXiv* [[paper](https://arxiv.org/abs/2605.18817)]
  <sub>Diffusion Language Models (DLMs) generate text by iteratively denoising masked token sequences, offering a tradeoff between parallelism and quality compared to autoregressive models. In current practi…</sub>
- [2026/05] **Beyond Execution: Static-Analysis Rewards and Hint-Conditioned Diffusion RL for Code Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.17174)]
  <sub>Reinforcement Learning (RL) is an important paradigm for aligning Diffusion Language Models (DLMs) toward functional correctness in code generation. However, these models often encounter a ``capabilit…</sub>
- [2026/05] **Constrained Code Generation with Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.16829)]
  <sub>Discrete diffusion models are a powerful, emerging paradigm for code generation. They construct programs through iterative refinement of partially corrupted token sequences and enable parallel token r…</sub>
- [2026/05] **DACA-GRPO: Denoising-Aware Credit Assignment for Reinforcement Learning in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.16342)]
  <sub>Diffusion large language models are a compelling alternative to autoregressive models, yet existing RL methods for diffusion treat all denoising steps as equally important and rely on biased, high-var…</sub>
- [2026/05] **From Table to Cell: Attention for Better Reasoning with TABALIGN** *arXiv* [[paper](https://arxiv.org/abs/2605.14465)]
  <sub>Multi-step LLM reasoning over structured tables fails because planning and execution share no explicit cell-grounding contract. Existing methods constrain the planner to a left-to-right factorization…</sub>
- [2026/05] **Factorization-Error-Free Discrete Diffusion Language Model via Speculative Decoding** *arXiv* [[paper](https://arxiv.org/abs/2605.14305)]
  <sub>Discrete diffusion language models improve generation efficiency through parallel token prediction, but standard $X_0$ prediction methods introduce factorization errors by approximating the clean toke…</sub>
- [2026/05] **Beyond Mode-Seeking RL: Trajectory-Balance Post-Training for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.13935)]
  <sub>Diffusion language models are a promising alternative to autoregressive models, yet post-training methods for them largely adapt reward-maximizing objectives. We identify a central failure mode in thi…</sub>
- [2026/05] **Discrete Diffusion for Complex and Congested Multi-Agent Path Finding with Sparse Social Attention** *arXiv* [[paper](https://arxiv.org/abs/2605.13296)]
  <sub>Multi-Agent Path Finding (MAPF) is a coordination problem that requires computing globally consistent, collision-free trajectories from individual start positions to assigned goal positions under comb…</sub>
- [2026/05] **LEAP: Unlocking dLLM Parallelism via Lookahead Early-Convergence Token Detection** *arXiv* [[paper](https://arxiv.org/abs/2605.10980)]
  <sub>Diffusion Language Models (dLLMs) have garnered significant attention for their potential in highly parallel processing. The parallel capabilities of existing dLLMs stem from the assumption of conditi…</sub>
- [2026/05] **Relative Score Policy Optimization for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.10218)]
  <sub>Diffusion large language models (dLLMs) offer a promising route to parallel and efficient text generation, but improving their reasoning ability requires effective post-training. Reinforcement learnin…</sub>
- [2026/05] **Edit-Based Refinement for Parallel Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.09603)]
  <sub>Masked diffusion language models enable parallel token generation and offer improved decoding efficiency over autoregressive models. However, their performance degrades significantly when generating m…</sub>
- [2026/05] **Layer Collapse in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.06366)]
  <sub>Diffusion language models (DLMs) have recently emerged as competitive alternatives to autoregressive (AR) language models, yet differences in their activation dynamics remain poorly understood. We cha…</sub>
- [2026/05] **Leveraging Pretrained Language Models as Energy Functions for Glauber Dynamics Text Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.04291)]
  <sub>We present a discrete diffusion-based language model using Glauber dynamics from statistical physics. Our main insight is that instead of trying to train a discrete state space diffusion model using G…</sub>
- [2026/04] **On the Trainability of Masked Diffusion Language Models via Blockwise Locality** *arXiv* [[paper](https://arxiv.org/abs/2604.24832)]
  <sub>Masked diffusion language models (MDMs) have recently emerged as a promising alternative to standard autoregressive large language models (AR-LLMs), yet their optimization can be substantially less st…</sub>
- [2026/04] **DPRM: A Plug-in Doob h transform-induced Token-Ordering Module for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.24357)]
  <sub>Diffusion language models generate without a fixed left-to-right order, making token ordering a central algorithmic choice: which tokens should be revealed, retained, revised or verified at each step?…</sub>
- [2026/04] **Stability-Weighted Decoding for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.17068)]
  <sub>Diffusion large language models (dLLMs) enable parallel text generation by iteratively denoising a fully masked sequence, unmasking a subset of masked tokens at each step. Existing decoding strategies…</sub>
- [2026/04] **Reasoning on the Manifold: Bidirectional Consistency for Self-Verification in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.16565)]
  <sub>While Diffusion Large Language Models (dLLMs) offer structural advantages for global planning, efficiently verifying that they arrive at correct answers via valid reasoning traces remains a critical c…</sub>
- [2026/04] **Dataset-Level Metrics Attenuate Non-Determinism: A Fine-Grained Non-Determinism Evaluation in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.13413)]
  <sub>Diffusion language models (DLMs) have emerged as a promising paradigm for large language models (LLMs), yet the non-deterministic behavior of DLMs remains poorly understood. The existing non-determini…</sub>
- [2026/04] **Early Decisions Matter: Proximity Bias and Initial Trajectory Shaping in Non-Autoregressive Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.10567)]
  <sub>Diffusion-based language models (dLLMs) have emerged as a promising alternative to autoregressive language models, offering the potential for parallel token generation and bidirectional context modeli…</sub>
- [2026/04] **DiffuMask: Diffusion Language Model for Token-level Prompt Pruning** *arXiv* [[paper](https://arxiv.org/abs/2604.06627)]
  <sub>In-Context Learning and Chain-of-Thought prompting improve reasoning in large language models (LLMs). These typically come at the cost of longer, more expensive prompts that may contain redundant info…</sub>
- [2026/04] **$S^3$: Stratified Scaling Search for Test-Time in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.06260)]
  <sub>Test-time scaling investigates whether a fixed diffusion language model (DLM) can generate better outputs when given more inference compute, without additional training. However, naive best-of-$K$ sam…</sub>
- [2026/04] **DualDiffusion: A Speculative Decoding Strategy for Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2604.05250)]
  <sub>Masked Diffusion Models (MDMs) offer a promising alternative to autoregressive language models by enabling parallel token generation and bidirectional context modeling. However, their inference speed…</sub>
- [2026/03] **EntropyCache: Decoded Token Entropy Guided KV Caching for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.18489)]
  <sub>Diffusion-based large language models (dLLMs) rely on bidirectional attention, which prevents lossless KV caching and requires a full forward pass at every denoising step. Existing approximate KV cach…</sub>
- [2026/03] **Mask Is What DLLM Needs: A Masked Data Training Paradigm for Diffusion LLMs** *arXiv* [[paper](https://arxiv.org/abs/2603.15803)]
  <sub>Discrete diffusion models offer global context awareness and flexible parallel generation. However, uniform random noise schedulers in standard DLLM training overlook the highly non-uniform informatio…</sub>
- [2026/03] **DOS: Dependency-Oriented Sampler for Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.15340)]
  <sub>Masked diffusion language models (MDLMs) have recently emerged as a new paradigm in language modeling, offering flexible generation dynamics and enabling efficient parallel decoding. However, existing…</sub>
- [2026/03] **Think First, Diffuse Fast: Improving Diffusion Language Model Reasoning via Autoregressive Plan Conditioning** *arXiv* [[paper](https://arxiv.org/abs/2603.13243)]
  <sub>Diffusion large language models (dLLMs) generate text via iterative denoising but consistently underperform on multi-step reasoning. We hypothesize this gap stems from a coordination problem: AR model…</sub>
- [2026/03] **Latent-DARM: Bridging Discrete Diffusion And Autoregressive Models For Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2603.09184)]
  <sub>Most multi-agent systems rely exclusively on autoregressive language models (ARMs) that are based on sequential generation. Although effective for fluent text, ARMs limit global reasoning and plan rev…</sub>
- [2026/03] **Evo: Autoregressive-Diffusion Large Language Models with Evolving Balance** *arXiv* [[paper](https://arxiv.org/abs/2603.06617)]
  <sub>We introduce \textbf{Evo}, a duality latent trajectory model that bridges autoregressive (AR) and diffusion-based language generation within a continuous evolutionary generative framework. Rather than…</sub>
- [2026/03] **Diffusion Language Models Are Natively Length-Aware** *arXiv* [[paper](https://arxiv.org/abs/2603.06123)]
  <sub>Unlike autoregressive language models, which terminate variable-length generation upon predicting an End-of-Sequence (EoS) token, Diffusion Language Models (DLMs) operate over a fixed maximum-length c…</sub>
- [2026/03] **Free Lunch for Pass@$k$? Low Cost Diverse Sampling for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.04893)]
  <sub>Diverse outputs in text generation are necessary for effective exploration in complex reasoning tasks, such as code generation and mathematical problem solving. Such Pass@$k$ problems benefit from dis…</sub>
- [2026/03] **LFPO: Likelihood-Free Policy Optimization for Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2603.01563)]
  <sub>Reinforcement Learning with Verifiable Rewards (RLVR) has achieved remarkable success in improving autoregressive models, especially in domains requiring correctness like mathematical reasoning and co…</sub>
- [2026/03] **MetaState: Persistent Working Memory Enhances Reasoning in Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.01331)]
  <sub>Discrete diffusion language models (dLLMs) generate text by iteratively denoising a masked sequence. However, standard dLLMs condition each denoising step solely on the current hard-masked sequence, w…</sub>
- [2026/03] **Reasoning or Rationalization? The Role of Justifications in Masked Diffusion Models for Fact Verification** *arXiv* [[paper](https://arxiv.org/abs/2603.01190)]
  <sub>Unlike autoregressive models, which generate tokens sequentially and benefit from reasoning-before-answering strategies such as Chain-of-Thought, Masked Diffusion Language Models (MDLMs) refine all se…</sub>
- [2026/02] **Test-Time Scaling with Diffusion Language Models via Reward-Guided Stitching** *arXiv* [[paper](https://arxiv.org/abs/2602.22871)]
  <sub>Reasoning with large language models often benefits from generating multiple chains-of-thought, but existing aggregation strategies are typically trajectory-level (e.g., selecting the best trace or vo…</sub>
- [2026/02] **Stop-Think-AutoRegress: Language Modeling with Latent Diffusion Planning** *COLM 2025* [[paper](https://arxiv.org/abs/2602.20528)]
  <sub>The Stop-Think-AutoRegress Language Diffusion Model (STAR-LDM) integrates latent diffusion planning with autoregressive generation. Unlike conventional autoregressive language models limited to token-…</sub>
- [2026/02] **Discrete Diffusion Models Exploit Asymmetry to Solve Lookahead Planning Tasks** *arXiv* [[paper](https://arxiv.org/abs/2602.19980)]
  <sub>While Autoregressive (AR) Transformer-based Generative Language Models are frequently employed for lookahead tasks, recent research suggests a potential discrepancy in their ability to perform plannin…</sub>
- [2026/02] **AnCoder: Anchored Code Generation via Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.17688)]
  <sub>Diffusion language models offer a compelling alternative to autoregressive code generation, enabling global planning and iterative refinement of complex program logic. However, existing approaches fai…</sub>
- [2026/02] **VDLM: Variable Diffusion LMs via Robust Latent-to-Text Rendering** *arXiv* [[paper](https://arxiv.org/abs/2602.15870)]
  <sub>Autoregressive language models decode left-to-right with irreversible commitments, limiting revision during multi-step reasoning. We propose \textbf{VDLM}, a modular variable diffusion language model…</sub>
- [2026/02] **Scaling Beyond Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.15014)]
  <sub>Diffusion language models are a promising alternative to autoregressive models due to their potential for faster generation. Among discrete diffusion approaches, Masked diffusion currently dominates,…</sub>
- [2026/02] **Can I Have Your Order? Monte-Carlo Tree Search for Slot Filling Ordering in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.12586)]
  <sub>While plan-and-infill decoding in Masked Diffusion Models (MDMs) shows promise for mathematical and code reasoning, performance remains highly sensitive to slot infilling order, often yielding substan…</sub>
- [2026/02] **Search or Accelerate: Confidence-Switched Position Beam Search for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.10953)]
  <sub>Diffusion Language Models (DLMs) generate text by iteratively denoising a masked sequence, repeatedly deciding which positions to commit at each step. Standard decoding follows a greedy rule: unmask t…</sub>
- [2026/02] **Advancing Block Diffusion Language Models for Test-Time Scaling** *arXiv* [[paper](https://arxiv.org/abs/2602.09555)]
  <sub>Recent advances in block diffusion language models have demonstrated competitive performance and strong scalability on reasoning tasks. However, existing BDLMs have limited exploration under the test-…</sub>
- [2026/02] **UnMaskFork: Test-Time Scaling for Masked Diffusion via Deterministic Action Branching** *arXiv* [[paper](https://arxiv.org/abs/2602.04344)]
  <sub>Test-time scaling strategies have effectively leveraged inference-time compute to enhance the reasoning abilities of Autoregressive Large Language Models. In this work, we demonstrate that Masked Diff…</sub>
- [2026/02] **Reasoning with Latent Tokens in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.03769)]
  <sub>Discrete diffusion models have recently become competitive with autoregressive models for language modeling, even outperforming them on reasoning tasks requiring planning and global coherence, but the…</sub>
- [2026/02] **Search-Augmented Masked Diffusion Models for Constrained Generation** *arXiv* [[paper](https://arxiv.org/abs/2602.02727)]
  <sub>Discrete diffusion models generate sequences by iteratively denoising samples corrupted by categorical noise, offering an appealing alternative to autoregressive decoding for structured and symbolic g…</sub>
- [2026/01] **Thinking Out of Order: When Output Order Stops Reflecting Reasoning Order in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.22035)]
  <sub>Autoregressive (AR) language models enforce a fixed left-to-right generation order, creating a fundamental limitation when the required output structure conflicts with natural reasoning (e.g., produci…</sub>
- [2026/01] **Plan, Verify and Fill: A Structured Parallel Decoding Approach for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.12247)]
  <sub>Diffusion Language Models (DLMs) present a promising non-sequential paradigm for text generation, distinct from standard autoregressive (AR) approaches. However, current decoding strategies often adop…</sub>
- [2026/01] **Discrete Feynman-Kac Correctors** *arXiv* [[paper](https://arxiv.org/abs/2601.10403)]
  <sub>Discrete diffusion models have recently emerged as a promising alternative to the autoregressive approach for generating discrete sequences. Sample generation via gradual denoising or demasking proces…</sub>
- [2026/01] **Bridging the Discrete-Continuous Gap: Unified Multimodal Generation via Coupled Manifold Discrete Absorbing Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2601.04056)]
  <sub>The bifurcation of generative modeling into autoregressive approaches for discrete data (text) and diffusion approaches for continuous data (images) hinders the development of truly unified multimodal…</sub>
- [2026/01] **CD4LM: Consistency Distillation and aDaptive Decoding for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.02236)]
  <sub>Autoregressive large language models achieve strong results on many benchmarks, but decoding remains fundamentally latency-limited by sequential dependence on previously generated tokens. Diffusion la…</sub>
- [2026/01] **Deferred Commitment Decoding for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.02076)]
  <sub>Diffusion language models (DLMs) have recently emerged as a strong alternative to autoregressive models by enabling parallel text generation. To improve inference efficiency and KV-cache compatibility…</sub>
- [2025/12] **Optimizing Decoding Paths in Masked Diffusion Models by Quantifying Uncertainty** *arXiv* [[paper](https://arxiv.org/abs/2512.21336)]
  <sub>Masked Diffusion Models (MDMs) offer flexible, non-autoregressive generation, but this freedom introduces a challenge: final output quality is highly sensitive to the decoding order. We are the first…</sub>
- [2025/12] **Context-Aware Initialization for Reducing Generative Path Length in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2512.19004)]
  <sub>Diffusion Large Language Models (DLLMs) enable fully parallel token decoding but often remain impractical at inference time due to the many denoising iterations required to refine an information-free,…</sub>
- [2025/11] **Lookahead Unmasking Elicits Accurate Decoding in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2511.05563)]
  <sub>Masked Diffusion Models (MDMs) as language models generate by iteratively unmasking tokens, yet their performance crucially depends on the inference time order of unmasking. Prevailing heuristics, suc…</sub>
- [2025/11] **Effective Test-Time Scaling of Discrete Diffusion through Iterative Refinement** *arXiv* [[paper](https://arxiv.org/abs/2511.05562)]
  <sub>Test-time scaling through reward-guided generation remains largely unexplored for discrete diffusion models despite its potential as a promising alternative. In this work, we introduce Iterative Rewar…</sub>
- [2025/10] **Parallel Sampling from Masked Diffusion Models via Conditional Independence Testing** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2510.21961)]
  <sub>Masked diffusion models (MDMs) offer a compelling alternative to autoregressive models (ARMs) for discrete text generation because they enable parallel token sampling, rather than sequential, left-to-…</sub>
- [2025/10] **MRO: Enhancing Reasoning in Diffusion Language Models via Multi-Reward Optimization** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2510.21473)]
  <sub>Recent advances in diffusion language models (DLMs) have presented a promising alternative to traditional autoregressive large language models (LLMs). However, DLMs still lag behind LLMs in reasoning…</sub>
- [2025/10] **No Compute Left Behind: Rethinking Reasoning and Sampling with Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2510.19990)]
  <sub>Masked diffusion language models (MDLMs) are trained to in-fill positions in randomly masked sequences, in contrast to next-token prediction models. Discussions around MDLMs focus on two benefits: (1)…</sub>
- [2025/10] **Planner and Executor: Collaboration between Discrete Diffusion And Autoregressive Models in Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2510.15244)]
  <sub>Current autoregressive language models (ARMs) achieve high accuracy but require long token sequences, making them costly. Discrete diffusion language models (DDLMs) enable parallel and flexible genera…</sub>
- [2025/10] **Latent Refinement Decoding: Enhancing Diffusion-Based Language Models by Refining Belief States** *arXiv* [[paper](https://arxiv.org/abs/2510.11052)]
  <sub>Autoregressive (AR) models remain the standard for natural language generation but still suffer from high latency due to strictly sequential decoding. Recent diffusion-inspired approaches, such as Lla…</sub>
- [2025/10] **SDAR: A Synergistic Diffusion-AutoRegression Paradigm for Scalable Sequence Generation** *arXiv* [[paper](https://arxiv.org/abs/2510.06303)]
  <sub>We propose SDAR, a Synergistic Diffusion-Autoregression paradigm that unifies the training efficiency of autoregressive models with the parallel inference capability of diffusion. Instead of costly en…</sub>
- [2025/10] **Every Step Counts: Decoding Trajectories as Authorship Fingerprints of dLLMs** *arXiv* [[paper](https://arxiv.org/abs/2510.05148)]
  <sub>Discrete Diffusion Large Language Models (dLLMs) have recently emerged as a competitive paradigm for non-autoregressive language modeling. Their distinctive decoding mechanism enables faster inference…</sub>
- [2025/10] **Consolidating Reinforcement Learning for Multimodal Discrete Diffusion Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2510.02880)]
  <sub>Optimizing discrete diffusion model (DDM) with rewards remains a challenge: the non-autoregressive paradigm makes importance sampling intractable and rollout complex, puzzling reinforcement learning m…</sub>
- [2025/09] **LLaDA-MoE: A Sparse MoE Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2509.24389)]
  <sub>We introduce LLaDA-MoE, a large language diffusion model with the Mixture-of-Experts (MoE) architecture, trained from scratch on approximately 20T tokens. LLaDA-MoE achieves competitive performance wi…</sub>
- [2025/09] **Taming Masked Diffusion Language Models via Consistency Trajectory Reinforcement Learning with Fewer Decoding Step** *arXiv* [[paper](https://arxiv.org/abs/2509.23924)]
  <sub>Masked diffusion language models (MDLMs) have recently emerged as a promising alternative to autoregressive (AR) language models, offering properties such as parallel decoding, flexible generation ord…</sub>
- [2025/09] **Inpainting-Guided Policy Optimization for Diffusion Large Language Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.10396)]
  <sub>Masked diffusion large language models (dLLMs) are emerging as promising alternatives to autoregressive LLMs, offering competitive performance while supporting unique generation capabilities such as i…</sub>
- [2025/09] **Revolutionizing Reinforcement Learning Framework for Diffusion Large Language Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.06949)]
  <sub>We propose TraceRL, a trajectory-aware reinforcement learning framework for diffusion language models (DLMs) that incorporates preferred inference trajectory into post-training, and is applicable acro…</sub>
- [2025/09] **Dream-Coder 7B: An Open Diffusion Language Model for Code** *arXiv* [[paper](https://arxiv.org/abs/2509.01142)]
  <sub>We present Dream-Coder 7B, an open-source discrete diffusion language model for code generation that exhibits emergent any-order generation capabilities. Unlike traditional autoregressive (AR) models…</sub>
- [2025/09] **Any-Order Flexible Length Masked Diffusion** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.01025)]
  <sub>Masked diffusion models (MDMs) have recently emerged as a promising alternative to autoregressive models over discrete domains. MDMs generate sequences in an any-order, parallel fashion, enabling fast…</sub>
- [2025/08] **Dream 7B: Diffusion Large Language Models** *arXiv* [[paper](https://arxiv.org/abs/2508.15487)]
  <sub>We introduce Dream 7B, the most powerful open diffusion large language model to date. Unlike autoregressive (AR) models that generate tokens sequentially, Dream 7B employs discrete diffusion modeling…</sub>
- [2025/08] **Reinforced Context Order Recovery for Adaptive Reasoning and Planning** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2508.13070)]
  <sub>Modern causal language models, followed by rapid developments in discrete diffusion models, can now produce a wide variety of interesting and useful content. However, these families of models are pred…</sub>
- [2025/08] **Diffusion LLMs Can Do Faster-Than-AR Inference via Discrete Diffusion Forcing** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2508.09192)]
  <sub>Diffusion Large Language Models (dLLMs) have emerged as a promising alternative to autoregressive (AR) LLMs for text generation, with the potential to decode multiple tokens in a single iteration. How…</sub>
- [2025/06] **DiffuCoder: Understanding and Improving Masked Diffusion Models for Code Generation** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2506.20639)]
  <sub>Diffusion large language models (dLLMs) are compelling alternatives to autoregressive (AR) models because their denoising models operate over the entire sequence. The global planning and iterative ref…</sub>
- [2025/05] **Anchored Diffusion Language Model** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2505.18456)]
  <sub>Diffusion Language Models (DLMs) promise parallel generation and bidirectional context, yet they underperform autoregressive (AR) models in both likelihood modeling and generated text quality. We iden…</sub>
- [2025/04] **Reviving Any-Subset Autoregressive Models with Principled Parallel Sampling and Speculative Decoding** *arXiv* [[paper](https://arxiv.org/abs/2504.20456)]
  <sub>In arbitrary-order language models, it is an open question how to sample tokens in parallel from the correct joint distribution. With discrete diffusion models, the more tokens they generate in parall…</sub>
- [2025/03] **Offline Reinforcement Learning with Discrete Diffusion Skills** *arXiv* [[paper](https://arxiv.org/abs/2503.20176)]
  <sub>Skills have been introduced to offline reinforcement learning (RL) as temporal abstractions to tackle complex, long-horizon tasks, promoting consistent behavior and enabling meaningful exploration. Wh…</sub>
- [2025/02] **Implicit Search via Discrete Diffusion: A Study on Chess** *ICLR 2025 Poster* [[paper](https://arxiv.org/abs/2502.19805)]
  <sub>In the post-AlphaGo era, there has been a renewed interest in search techniques such as Monte Carlo Tree Search (MCTS), particularly in their application to Large Language Models (LLMs). This renewed…</sub>

## rl-alignment (43)

_RL / preference / reward / alignment for diffusion LMs._

- [2026/05] **Reinforcement Learning from Denoising Feedback** *arXiv* [[paper](https://arxiv.org/abs/2605.25638)]
  <sub>Policy loss estimation remains a fundamental and long-standing challenge in reinforcement learning (RL) for diffusion language models (dLLMs). We introduce Reinforcement Learning from Denoising Feedba…</sub>
- [2026/05] **Contrastive Distribution Matching for Amortized Sequential Monte Carlo in Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.23346)]
  <sub>Discrete diffusion models have emerged as powerful frameworks for generating structured categorical data. However, efficiently sampling from reward-tilted distributions remains a fundamental challenge…</sub>
- [2026/05] **Steering Without Breaking: Mechanistically Informed Interventions for Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.10971)]
  <sub>Discrete diffusion language models (DLMs) generate text by iteratively denoising all positions in parallel, offering an alternative to autoregressive models. Controlled generation methods for DLMs, im…</sub>
- [2026/05] **TextLDM: Language Modeling with Continuous Latent Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.07748)]
  <sub>Diffusion Transformers (DiT) trained with flow matching in a VAE latent space have unified visual generation across images and videos. A natural next step toward a single architecture for both generat…</sub>
- [2026/05] **Guidance Is Not a Hyperparameter: Learning Dynamic Control in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.07701)]
  <sub>Classifier-Free Guidance (CFG) is a widely used mechanism for controlling diffusion-based generative models, yet its guidance scale is typically treated as a fixed hyperparameter throughout generation…</sub>
- [2026/05] **Don't Retrain, Align: Adapting Autoregressive LMs to Diffusion LMs via Representation Alignment** *arXiv* [[paper](https://arxiv.org/abs/2605.06885)]
  <sub>Diffusion language models (DLMs) have recently demonstrated capabilities that complement standard autoregressive (AR) models, particularly in non-sequential generation and bidirectional editing. Altho…</sub>
- [2026/04] **UDM-GRPO: Stable and Efficient Group Relative Policy Optimization for Uniform Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2604.18518)]
  <sub>Uniform Discrete Diffusion Model (UDM) has recently emerged as a promising paradigm for discrete generative modeling; however, its integration with reinforcement learning remains largely unexplored. W…</sub>
- [2026/04] **Re-Mask and Redirect: Exploiting Denoising Irreversibility in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.08557)]
  <sub>Safety alignment in diffusion language models (dLLMs) relies on a single load-bearing assumption: that committed tokens are permanent. We show that violating this assumption, by re-masking committed r…</sub>
- [2026/04] **DARE: Diffusion Large Language Models Alignment and Reinforcement Executor** *arXiv* [[paper](https://arxiv.org/abs/2604.04215)]
  <sub>Diffusion large language models (dLLMs) are emerging as a compelling alternative to dominant autoregressive models, replacing strictly sequential token generation with iterative denoising and parallel…</sub>
- [2026/03] **Stabilizing Reinforcement Learning for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.06743)]
  <sub>Group Relative Policy Optimization (GRPO) is highly effective for post-training autoregressive (AR) language models, yet its direct application to diffusion large language models (dLLMs) often trigger…</sub>
- [2026/03] **Active Flow Matching** *arXiv* [[paper](https://arxiv.org/abs/2603.00877)]
  <sub>Discrete diffusion and flow matching models capture complex, non-additive and non-autoregressive structure in high-dimensional objective landscapes through parallel, iterative refinement. However, the…</sub>
- [2026/03] **Breaking the Factorization Barrier in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.00045)]
  <sub>Diffusion language models theoretically allow for efficient parallel generation but are practically hindered by the "factorization barrier": the assumption that simultaneously predicted tokens are ind…</sub>
- [2026/02] **Continuous Diffusion Models Can Obey Formal Syntax** *arXiv* [[paper](https://arxiv.org/abs/2602.12468)]
  <sub>Diffusion language models offer a promising alternative to autoregressive models due to their global, non-causal generation process, but their continuous latent dynamics make discrete constraints -- e…</sub>
- [2026/02] **Embedding Inversion via Conditional Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.11047)]
  <sub>We frame embedding inversion as conditional masked diffusion, recovering all tokens in parallel through iterative denoising rather than sequential autoregressive generation. A masked diffusion languag…</sub>
- [2026/02] **Where-to-Unmask: Ground-Truth-Guided Unmasking Order Learning for Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.09501)]
  <sub>Masked Diffusion Language Models (MDLMs) generate text by iteratively filling masked tokens, requiring two coupled decisions at each step: which positions to unmask (where-to-unmask) and which tokens…</sub>
- [2026/02] **Efficient and Stable Reinforcement Learning for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.08905)]
  <sub>Reinforcement Learning (RL) is crucial for unlocking the complex reasoning capabilities of Diffusion-based Large Language Models (dLLMs). However, applying RL to dLLMs faces unique challenges in effic…</sub>
- [2026/02] **LLaDA2.1: Speeding Up Text Diffusion via Token Editing** *arXiv* [[paper](https://arxiv.org/abs/2602.08676)]
  <sub>While LLaDA2.0 showcased the scaling potential of 100B-level block-diffusion models and their inherent parallelization, the delicate equilibrium between decoding speed and generation quality has remai…</sub>
- [2026/02] **Learnable Chernoff Baselines for Inference-Time Alignment** *arXiv* [[paper](https://arxiv.org/abs/2602.07738)]
  <sub>We study inference-time reward-guided alignment for generative models. Existing methods often rely on either architecture-specific adaptations or computationally costly inference procedures. We introd…</sub>
- [2026/02] **DLM-Scope: Mechanistic Interpretability of Diffusion Language Models via Sparse Autoencoders** *arXiv* [[paper](https://arxiv.org/abs/2602.05859)]
  <sub>Sparse autoencoders (SAEs) have become a standard tool for mechanistic interpretability in autoregressive large language models (LLMs), enabling researchers to extract sparse, human-interpretable feat…</sub>
- [2026/02] **D3PIA: A Discrete Denoising Diffusion Model for Piano Accompaniment Generation From Lead sheet** *IEEE International Conference on Acoustics, Speech, and Signal Processing 2026* [[paper](https://arxiv.org/abs/2602.03523)]
  <sub>Generating piano accompaniments in the symbolic music domain is a challenging task that requires producing a complete piece of piano music from given melody and chord constraints, such as those provid…</sub>
- [2026/02] **Symbol-Aware Reasoning with Masked Discrete Diffusion for Handwritten Mathematical Expression Recognition** *arXiv* [[paper](https://arxiv.org/abs/2602.03370)]
  <sub>Handwritten Mathematical Expression Recognition (HMER) requires reasoning over diverse symbols and 2D structural layouts, yet autoregressive models struggle with exposure bias and syntactic inconsiste…</sub>
- [2026/02] **TABES: Trajectory-Aware Backward-on-Entropy Steering for Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.00250)]
  <sub>Masked Diffusion Models (MDMs) have emerged as a promising non-autoregressive paradigm for generative tasks, offering parallel decoding and bidirectional context utilization. However, current sampling…</sub>
- [2026/01] **Zonkey: A Hierarchical Diffusion Language Model with Differentiable Tokenization and Probabilistic Attention** *arXiv* [[paper](https://arxiv.org/abs/2601.21768)]
  <sub>Large language models (LLMs) have revolutionized natural language processing, yet they remain constrained by fixed, non-differentiable tokenizers like Byte Pair Encoding (BPE), which hinder end-to-end…</sub>
- [2026/01] **ILRR: Inference-Time Steering Method for Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.21647)]
  <sub>Discrete Diffusion Language Models (DLMs) offer a promising non-autoregressive alternative for text generation, yet effective mechanisms for inference-time control remain relatively underexplored. Exi…</sub>
- [2026/01] **Pay (Cross) Attention to the Melody: Curriculum Masking for Single-Encoder Melodic Harmonization** *BigData Congress [Services Society] 2027* [[paper](https://arxiv.org/abs/2601.16150)]
  <sub>Melodic harmonization, the task of generating harmonic accompaniments for a given melody, remains a central challenge in computational music generation. Recent single encoder transformer approaches ha…</sub>
- [2026/01] **Top 10 Open Challenges Steering the Future of Diffusion Language Model and Its Variants** *arXiv* [[paper](https://arxiv.org/abs/2601.14041)]
  <sub>The paradigm of Large Language Models (LLMs) is currently defined by auto-regressive (AR) architectures, which generate text through a sequential ``brick-by-brick'' process. Despite their success, AR…</sub>
- [2026/01] **Unlocking the Potentials of Retrieval-Augmented Generation for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.11342)]
  <sub>Diffusion Language Models (DLMs) have recently demonstrated remarkable capabilities in natural language processing tasks. However, the potential of Retrieval-Augmented Generation (RAG), which shows gr…</sub>
- [2026/01] **Agents of Diffusion: Enhancing Diffusion Language Models with Multi-Agent Reinforcement Learning for Structured Data Generation (Extended Version)** *arXiv* [[paper](https://arxiv.org/abs/2601.07152)]
  <sub>Generating high-quality structured data such as JSON records, remains a fundamental challenge for large language models (LLMs), particularly when semantic richness must coexist with strict schema adhe…</sub>
- [2025/12] **LLaDA2.0: Scaling Up Diffusion Language Models to 100B** *arXiv* [[paper](https://arxiv.org/abs/2512.15745)]
  <sub>This paper presents LLaDA2.0 -- a tuple of discrete diffusion large language models (dLLM) scaling up to 100B total parameters through systematic conversion from auto-regressive (AR) models -- establi…</sub>
- [2025/11] **SpecDiff-2: Scaling Diffusion Drafter Alignment For Faster Speculative Decoding** *arXiv* [[paper](https://arxiv.org/abs/2511.00606)]
  <sub>Speculative decoding has become the standard approach for accelerating Large Language Model (LLM) inference. It exploits a lossless draft-then-verify procedure to circumvent the latency of autoregress…</sub>
- [2025/10] **DiSTAR: Diffusion over a Scalable Token Autoregressive Representation for Speech Generation** *arXiv* [[paper](https://arxiv.org/abs/2510.12210)]
  <sub>Recent attempts to interleave autoregressive (AR) sketchers with diffusion-based refiners over continuous speech representations have shown promise, but they remain brittle under distribution shift an…</sub>
- [2025/10] **Controllable Stylistic Text Generation with Train-Time Attribute-Regularized Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2510.06386)]
  <sub>Generating stylistic text with specific attributes is a key problem in controllable text generation. Recently, diffusion models have emerged as a powerful paradigm for both visual and textual generati…</sub>
- [2025/10] **SALSA-V: Shortcut-Augmented Long-form Synchronized Audio from Videos** *arXiv* [[paper](https://arxiv.org/abs/2510.02916)]
  <sub>We propose SALSA-V, a multimodal video-to-audio generation model capable of synthesizing highly synchronized, high-fidelity long-form audio from silent video content. Our approach introduces a masked…</sub>
- [2025/10] **Syntax-Guided Diffusion Language Models with User-Integrated Personalization** *arXiv* [[paper](https://arxiv.org/abs/2510.01028)]
  <sub>Large language models have made revolutionary progress in generating human-like text, yet their outputs often tend to be generic, exhibiting insufficient structural diversity, which limits personalize…</sub>
- [2025/09] **TR2-D2: Tree Search Guided Trajectory-Aware Fine-Tuning for Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2509.25171)]
  <sub>Reinforcement learning with stochastic optimal control offers a promising framework for diffusion fine-tuning, where a pre-trained diffusion model is optimized to generate paths that lead to a reward-…</sub>
- [2025/09] **Don't Settle Too Early: Self-Reflective Remasking for Diffusion Language Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.23653)]
  <sub>Mask-based Diffusion Language Models (DLMs) struggle to revise incorrect tokens: once a token is generated, it typically remains fixed. The key challenge is to identify potential errors in the inputs.…</sub>
- [2025/09] **Tree Reward-Aligned Search for TReASURe in Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2509.23146)]
  <sub>Tree search has recently emerged as a powerful framework for aligning generative models with task-specific rewards at test time. Applying tree search to Masked Diffusion Language Models, however, intr…</sub>
- [2025/09] **Learnable Sampler Distillation for Discrete Diffusion Models** *NeurIPS 2025 spotlight* [[paper](https://arxiv.org/abs/2509.19962)]
  <sub>Discrete diffusion models (DDMs) have shown powerful generation ability for discrete data modalities like text and molecules. However, their practical application is hindered by inefficient sampling,…</sub>
- [2025/09] **Reward-Weighted Sampling: Enhancing Non-Autoregressive Characteristics in Masked Diffusion LLMs** *EMNLP 2025* [[paper](https://arxiv.org/abs/2509.00707)]
  <sub>Masked diffusion models (MDMs) offer a promising non-autoregressive alternative for large language modeling. Standard decoding methods for MDMs, such as confidence-based sampling, select tokens indepe…</sub>
- [2025/08] **Urban In-Context Learning: Bridging Pretraining and Inference through Masked Diffusion for Urban Profiling** *arXiv* [[paper](https://arxiv.org/abs/2508.03042)]
  <sub>Urban profiling aims to predict urban profiles in unknown regions and plays a critical role in economic and social censuses. Existing approaches typically follow a two-stage paradigm: first, learning…</sub>
- [2025/07] **Review, Remask, Refine (R3): Process-Guided Block Diffusion for Text Generation** *arXiv* [[paper](https://arxiv.org/abs/2507.08018)]
  <sub>A key challenge for iterative text generation is enabling models to efficiently identify and correct their own errors. We propose Review, Remask, Refine (R3), a relatively simple yet elegant framework…</sub>
- [2025/05] **Efficient Controllable Diffusion via Optimal Classifier Guidance** *arXiv* [[paper](https://arxiv.org/abs/2505.21666)]
  <sub>The controllable generation of diffusion models aims to steer the model to generate samples that optimize some given objective functions. It is desirable for a variety of applications including image…</sub>
- [2025/02] **E-MD3C: Taming Masked Diffusion Transformers for Efficient Zero-Shot Object Customization** *arXiv* [[paper](https://arxiv.org/abs/2502.09164)]
  <sub>We propose E-MD3C ($\underline{E}$fficient $\underline{M}$asked $\underline{D}$iffusion Transformer with Disentangled $\underline{C}$onditions and $\underline{C}$ompact $\underline{C}$ollector), a hig…</sub>

## controllable-generation (21)

_Controllable / conditional / constrained generation; infilling; editing._

- [2026/05] **ELF: Embedded Language Flows** *arXiv* [[paper](https://arxiv.org/abs/2605.10938)]
  <sub>Diffusion and flow-based models have become the de facto approaches for generating continuous data, e.g., in domains such as images and videos. Their success has attracted growing interest in applying…</sub>
- [2026/05] **Infinite Mask Diffusion for Few-Step Distillation** *arXiv* [[paper](https://arxiv.org/abs/2605.10518)]
  <sub>Masked Diffusion Models (MDMs) have emerged as a promising alternative to autoregressive models in language modeling, offering the advantages of parallel decoding and bidirectional context processing…</sub>
- [2026/05] **Primal-Dual Guided Decoding for Constrained Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.09749)]
  <sub>Discrete diffusion models generate structured sequences by progressively unmasking tokens, but enforcing global property constraints during generation remains an open challenge. We propose primal-dual…</sub>
- [2026/04] **FastDiSS: Few-step Match Many-step Diffusion Language Model on Sequence-to-Sequence Generation--Full Version** *arXiv* [[paper](https://arxiv.org/abs/2604.05551)]
  <sub>Self-conditioning has been central to the success of continuous diffusion language models, as it allows models to correct previous errors. Yet its ability degrades precisely in the regime where diffus…</sub>
- [2026/04] **Unlocking Prompt Infilling Capability for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.03677)]
  <sub>Masked diffusion language models (dLMs) generate text through bidirectional denoising, yet this capability remains locked for infilling prompts. This limitation is an artifact of the current supervise…</sub>
- [2026/04] **Not All Denoising Steps Are Equal: Model Scheduling for Faster Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.02340)]
  <sub>Recent advances in masked diffusion language models (MDLMs) narrow the quality gap to autoregressive LMs, but their sampling remains expensive because generation requires many full-sequence denoising…</sub>
- [2026/03] **Graph Energy Matching: Transport-Aligned Energy-Based Modeling for Graph Generation** *arXiv* [[paper](https://arxiv.org/abs/2603.23398)]
  <sub>Energy-based models for discrete domains, such as graphs, explicitly capture relative likelihoods, naturally enabling composable probabilistic inference tasks like conditional generation or enforcing…</sub>
- [2026/02] **ZUNA: Flexible EEG Superresolution with Position-Aware Diffusion Autoencoders** *arXiv* [[paper](https://arxiv.org/abs/2602.18478)]
  <sub>We present \texttt{ZUNA}, a 380M-parameter masked diffusion autoencoder trained to perform masked channel infilling and superresolution for arbitrary electrode numbers and positions in EEG signals. Th…</sub>
- [2026/02] **Improving Variable-Length Generation in Diffusion Language Models via Length Regularization** *arXiv* [[paper](https://arxiv.org/abs/2602.07546)]
  <sub>Diffusion Large Language Models (DLLMs) are inherently ill-suited for variable-length generation, as their inference is defined on a fixed-length canvas and implicitly assumes a known target length. W…</sub>
- [2026/02] **DreamOn: Diffusion Language Models For Code Infilling Beyond Fixed-size Canvas** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2602.01326)]
  <sub>Diffusion Language Models (DLMs) present a compelling alternative to autoregressive models, offering flexible, any-order infilling without specialized prompting design. However, their practical utilit…</sub>
- [2026/02] **Diffusion LMs Can Approximate Optimal Infilling Lengths Implicitly** *arXiv* [[paper](https://arxiv.org/abs/2602.00476)]
  <sub>Diffusion language models (DLMs) provide a bidirectional generation framework naturally suited for infilling, yet their performance is constrained by the pre-specified infilling length. In this paper,…</sub>
- [2026/01] **Autoregressive Models Rival Diffusion Models at ANY-ORDER Generation** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2601.13228)]
  <sub>Diffusion language models enable any-order generation and bidirectional conditioning, offering appealing flexibility for tasks such as infilling, rewriting, and self-correction. However, their formula…</sub>
- [2025/11] **Graph Diffusion Counterfactual Explanation** *arXiv* [[paper](https://arxiv.org/abs/2511.16287)]
  <sub>Machine learning models that operate on graph-structured data, such as molecular graphs or social networks, often make accurate predictions but offer little insight into why certain predictions are ma…</sub>
- [2025/10] **CANDI: Hybrid Discrete-Continuous Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2510.22510)]
  <sub>While continuous diffusion has shown remarkable success in continuous domains such as image generation, its direct application to discrete data has underperformed compared to purely discrete formulati…</sub>
- [2025/10] **CoDA: Coding LM via Diffusion Adaptation** *arXiv* [[paper](https://arxiv.org/abs/2510.03270)]
  <sub>Diffusion language models promise bidirectional context and infilling capabilities that autoregressive coders lack, yet practical systems remain heavyweight. We introduce CoDA, a 1.7B-parameter diffus…</sub>
- [2025/08] **Amadeus: Autoregressive Model with Bidirectional Attribute Modelling for Symbolic Music** *arXiv* [[paper](https://arxiv.org/abs/2508.20665)]
  <sub>Existing state-of-the-art symbolic music generation models predominantly adopt autoregressive or hierarchical autoregressive architectures, modelling symbolic music as a sequence of attribute tokens w…</sub>
- [2025/08] **Improving Text Style Transfer using Masked Diffusion Language Models with Inference-time Scaling** *European Conference on Artificial Intelligence 2025* [[paper](https://arxiv.org/abs/2508.10995)]
  <sub>Masked diffusion language models (MDMs) have recently gained traction as a viable generative framework for natural language. This can be attributed to its scalability and ease of training compared to…</sub>
- [2025/06] **What Exactly Does Guidance Do in Masked Discrete Diffusion Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2506.10971)]
  <sub>We study masked discrete diffusion models with classifier-free guidance (CFG). Assuming no score error nor discretization error, we derive an explicit solution to the guided reverse dynamics, so that…</sub>
- [2025/05] **Adaptive Classifier-Free Guidance via Dynamic Low-Confidence Masking** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2505.20199)]
  <sub>Classifier-Free Guidance (CFG) significantly enhances controllability in generative models by interpolating conditional and unconditional predictions. However, standard CFG often employs a static unco…</sub>
- [2025/03] **Understanding the Quality-Diversity Trade-off in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2503.10683)]
  <sub>Diffusion models have seen immense success in modelling continuous data across a range of domains such as vision and audio. Despite the challenges of adapting diffusion models to discrete data, recent…</sub>
- [2025/02] **Enabling Autoregressive Models to Fill In Masked Tokens** *arXiv* [[paper](https://arxiv.org/abs/2502.06901)]
  <sub>Historically, LLMs have been trained using either autoregressive (AR) or masked language modeling (MLM) objectives, with AR models gaining dominance in recent years. However, AR models are inherently…</sub>

## theory-analysis (22)

_Theory, likelihood, convergence, sample complexity, comparison studies._

- [2026/05] **From Scores to Gibbs Correctors: Accelerating Uniform-Rate Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2605.27352)]
  <sub>Discrete diffusion models have achieved strong empirical performance in text and other symbolic domains, but, especially for uniform-rate models, they often require many steps to generate a single sam…</sub>
- [2026/05] **On the Error-Correcting Effects of Stochasticity in Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.26582)]
  <sub>Discrete diffusion models achieve strong performance in text and image generation, but their inference remains slow and must inherently balance sampling efficiency and sample quality. In this work, we…</sub>
- [2026/05] **Targeted Remasking: Replacing Token Editing with Token-to-Mask Refinement in Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.26436)]
  <sub>Discrete masked diffusion language models such as LLaDA generate text through iterative denoising, where mask tokens are progressively replaced with predicted tokens. LLaDA2.1 introduced a Token-to-To…</sub>
- [2026/05] **Self-Balancing Gradient Allocation for Heterogeneity-Aware Feature Generation in Click-Through Rate Prediction** *arXiv* [[paper](https://arxiv.org/abs/2605.24986)]
  <sub>Generative pre-training via discrete diffusion provides dense reconstruction supervision across all feature fields simultaneously, mitigating representation collapse from data sparsity in CTR predicti…</sub>
- [2026/05] **TUBE: Tangent Upper Bound on Evidence for Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.24292)]
  <sub>Log-likelihood is a standard metric for evaluating generative models. Unfortunately, in contrast to autoregressive models (ARMs), discrete diffusion models generally do not admit exact computation of…</sub>
- [2026/05] **Dimension-Free Convergence of Discrete Diffusion Models: Adjoint Equations Induce the Right Space** *arXiv* [[paper](https://arxiv.org/abs/2605.17232)]
  <sub>Discrete diffusion has become a leading framework for generative modeling in various applications including language, vision, and biology. Existing convergence theory, however, exhibits fundamental li…</sub>
- [2026/04] **DepCap: Adaptive Block-Wise Parallel Decoding for Efficient Diffusion LM Inference** *arXiv* [[paper](https://arxiv.org/abs/2604.15750)]
  <sub>Diffusion language models (DLMs) have emerged as a promising alternative to autoregressive language generation due to their potential for parallel decoding and global refinement of the entire sequence…</sub>
- [2026/04] **Locally Confident, Globally Stuck: The Quality-Exploration Dilemma in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.00375)]
  <sub>Diffusion large language models (dLLMs) theoretically permit token decoding in arbitrary order, a flexibility that could enable richer exploration of reasoning paths than autoregressive (AR) LLMs. In…</sub>
- [2026/03] **Confidence-Based Decoding is Provably Efficient for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.22248)]
  <sub>Diffusion language models (DLMs) have emerged as a promising alternative to autoregressive (AR) models for language modeling, allowing flexible generation order and parallel generation of multiple tok…</sub>
- [2026/03] **Do Diffusion Models Dream of Electric Planes? Discrete and Continuous Simulation-Based Inference for Aircraft Design** *arXiv* [[paper](https://arxiv.org/abs/2603.13284)]
  <sub>In this paper, we generate conceptual engineering designs of electric vertical take-off and landing (eVTOL) aircraft. We follow the paradigm of simulation-based inference (SBI), whereby we look to lea…</sub>
- [2026/03] **Efficient Self-Evaluation for Diffusion Language Models via Sequence Regeneration** *arXiv* [[paper](https://arxiv.org/abs/2603.02760)]
  <sub>Diffusion large language models (dLLMs) have recently attracted significant attention for their ability to enhance diversity, controllability, and parallelism. However, their non-sequential, bidirecti…</sub>
- [2026/02] **Efficient Sampling with Discrete Diffusion Models: Sharp and Adaptive Guarantees** *arXiv* [[paper](https://arxiv.org/abs/2602.15008)]
  <sub>Diffusion models over discrete spaces have recently shown striking empirical success, yet their theoretical foundations remain incomplete. In this paper, we study the sampling efficiency of score-base…</sub>
- [2026/02] **Improved Sampling Schedules for Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.06849)]
  <sub>Discrete diffusion models have emerged as a powerful paradigm for generative modeling on sequence data; however, the information-theoretic principles governing their reverse processes remain significa…</sub>
- [2026/02] **Generation Order and Parallel Decoding in Masked Diffusion Models: An Information-Theoretic Perspective** *arXiv* [[paper](https://arxiv.org/abs/2602.00286)]
  <sub>Masked Diffusion Models (MDMs) significantly accelerate inference by trading off sequential determinism. However, the theoretical mechanisms governing generation order and the risks inherent in parall…</sub>
- [2025/11] **From Bits to Rounds: Parallel Decoding with Exploration for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2511.21103)]
  <sub>Diffusion Language Models (DLMs) have recently emerged as a strong alternative to autoregressive language models (LMs). DLMs offer comparable accuracy with faster inference speed via parallel decoding…</sub>
- [2025/11] **Demystifying Diffusion Objectives: Reweighted Losses are Better Variational Bounds** *arXiv* [[paper](https://arxiv.org/abs/2511.19664)]
  <sub>We derive a new theoretical interpretation of the reweighted losses that are widely used for training diffusion models. Our method is based on constructing a cascade of time-dependent variational lowe…</sub>
- [2025/11] **Optimal Inference Schedules for Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2511.04647)]
  <sub>A major bottleneck of standard auto-regressive large language models is that their inference process is inherently sequential, resulting in very long and costly inference times. To circumvent this, pr…</sub>
- [2025/11] **Optimal Boundary Control of Diffusion on Graphs via Linear Programming** *arXiv* [[paper](https://arxiv.org/abs/2511.03129)]
  <sub>We propose a linear programming (LP) framework for steady-state diffusion and flux optimization on geometric networks. The state variable satisfies a discrete diffusion law on a weighted, oriented gra…</sub>
- [2025/10] **Information-Theoretic Discrete Diffusion** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2510.24088)]
  <sub>We present an information-theoretic framework for discrete diffusion models that yields principled estimators of log-likelihood using score-matching losses. Inspired by the I-MMSE identity for the Gau…</sub>
- [2025/07] **ReDiSC: A Reparameterized Masked Diffusion Model for Scalable Node Classification with Structured Predictions** *arXiv* [[paper](https://arxiv.org/abs/2507.14484)]
  <sub>In recent years, graph neural networks (GNN) have achieved unprecedented successes in node classification tasks. Although GNNs inherently encode specific inductive biases (e.g., acting as low-pass or…</sub>
- [2025/05] **Almost Linear Convergence under Minimal Score Assumptions: Quantized Transition Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2505.21892)]
  <sub>Continuous diffusion models have demonstrated remarkable performance in data generation across various domains, yet their efficiency remains constrained by two critical limitations: (1) the local adja…</sub>
- [2025/05] **Discrete Markov Bridge** *arXiv* [[paper](https://arxiv.org/abs/2505.19752)]
  <sub>Discrete diffusion has recently emerged as a promising paradigm in discrete data modeling. However, existing methods typically rely on a fixed rate transition matrix during training, which not only li…</sub>

## hybrid-architecture (31)

_Hybrid AR+diffusion or novel architectures (block/latent/flow/state-space)._

- [2026/05] **Triplet-Block Diffusion RWKV** *arXiv* [[paper](https://arxiv.org/abs/2605.25969)]
  <sub>Causal Transformer language models suffer from strictly sequential decoding and a quadratic per-step attention cost. While linear-time causal models and discrete diffusion models each address these we…</sub>
- [2026/05] **FlowLM: Few-Step Language Modeling via Diffusion-to-Flow Adaptation** *arXiv* [[paper](https://arxiv.org/abs/2605.20199)]
  <sub>We present FlowLM, a flow matching language model transformed from pre-trained diffusion language models via efficient fine-tuning. By re-aligning the curved sampling trajectories of diffusion models…</sub>
- [2026/05] **Dynamic Chunking for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.15676)]
  <sub>Block discrete diffusion language models factorize a sequence autoregressively over fixed-size positional blocks, decoupling within-block parallel denoising from across-block conditioning. We argue th…</sub>
- [2026/05] **Discrete Langevin-Inspired Posterior Sampling** *arXiv* [[paper](https://arxiv.org/abs/2605.09302)]
  <sub>We study posterior sampling for inverse problems in discrete state spaces using discrete diffusion models as generative priors. While continuous diffusion models have become widely used for inverse pr…</sub>
- [2026/05] **How to Train Your Latent Diffusion Language Model Jointly With the Latent Space** *arXiv* [[paper](https://arxiv.org/abs/2605.07933)]
  <sub>Latent diffusion models offer an attractive alternative to discrete diffusion for non-autoregressive text generation by operating on continuous text representations and denoising entire sequences in p…</sub>
- [2026/05] **Scaling Categorical Flow Maps** *arXiv* [[paper](https://arxiv.org/abs/2605.07820)]
  <sub>Continuous diffusion and flow matching models could represent a powerful alternative to autoregressive approaches for language modelling (LM), as they unlock a host of advantages currently reserved fo…</sub>
- [2026/05] **Continuous Latent Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2605.06548)]
  <sub>Large language models have achieved remarkable success under the autoregressive paradigm, yet high-quality text generation need not be tied to a fixed left-to-right order. Existing alternatives still…</sub>
- [2026/05] **Binomial flows: Denoising and flow matching for discrete ordinal data** *arXiv* [[paper](https://arxiv.org/abs/2605.00360)]
  <sub>Flow-based generative modeling in continuous spaces exploit Tweedie's formula to express the denoiser (learned in training) as a score function (used in sampling). In contrast, this relation has been…</sub>
- [2026/04] **Factual and Edit-Sensitive Graph-to-Sequence Generation via Graph-Aware Adaptive Noising** *arXiv* [[paper](https://arxiv.org/abs/2604.24104)]
  <sub>Fine-tuned autoregressive models for graph-to-sequence generation (G2S) often struggle with factual grounding and edit sensitivity. To tackle these issues, we propose a non-autoregressive diffusion fr…</sub>
- [2026/04] **When to Commit? Towards Variable-Size Self-Contained Blocks for Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.23994)]
  <sub>Discrete diffusion language models (dLLMs) enable parallel token updates with bidirectional attention, yet practical generation typically adopts blockwise semi-autoregressive decoding. This switch cre…</sub>
- [2026/04] **Towards Faster Language Model Inference Using Mixture-of-Experts Flow Matching** *arXiv* [[paper](https://arxiv.org/abs/2604.15009)]
  <sub>Flow matching retains the generation quality of diffusion models while enabling substantially faster inference, making it a compelling paradigm for generative modeling. However, when applied to langua…</sub>
- [2026/04] **LangFlow: Continuous Diffusion Rivals Discrete in Language Modeling** *arXiv* [[paper](https://arxiv.org/abs/2604.11748)]
  <sub>Continuous diffusion has been the foundation of high-fidelity, controllable, and few-step generation of many data modalities such as images. However, in language modeling, prior continuous diffusion l…</sub>
- [2026/03] **Unrestrained Simplex Denoising for Discrete Data. A Non-Markovian Approach Applied to Graph Generation** *arXiv* [[paper](https://arxiv.org/abs/2603.28572)]
  <sub>Denoising models such as Diffusion or Flow Matching have recently advanced generative modeling for discrete structures, yet most approaches either operate directly in the discrete state space, causing…</sub>
- [2026/03] **GeoBlock: Inferring Block Granularity from Dependency Geometry in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2603.26675)]
  <sub>Block diffusion enables efficient parallel refinement in diffusion language models, but its decoding behavior depends critically on block size. Existing block-sizing strategies rely on fixed rules or…</sub>
- [2026/03] **DualTSR: Unified Dual-Diffusion Transformer for Scene Text Image Super-Resolution** *arXiv* [[paper](https://arxiv.org/abs/2603.14207)]
  <sub>Scene Text Image Super-Resolution (STISR) aims to restore high-resolution details in low-resolution text images, which is crucial for both human readability and machine recognition. Existing methods,…</sub>
- [2026/02] **Insertion Based Sequence Generation with Learnable Order Dynamics** *arXiv* [[paper](https://arxiv.org/abs/2602.18695)]
  <sub>In many domains generating variable length sequences through insertions provides greater flexibility over autoregressive models. However, the action space of insertion models is much larger than that…</sub>
- [2026/02] **VocalNet-MDM: Accelerating Streaming Speech LLM via Self-Distilled Masked Diffusion Modeling** *arXiv* [[paper](https://arxiv.org/abs/2602.08607)]
  <sub>Recent Speech Large Language Models~(LLMs) have achieved impressive capabilities in end-to-end speech interaction. However, the prevailing autoregressive paradigm imposes strict serial constraints, li…</sub>
- [2026/02] **FlashBlock: Attention Caching for Efficient Long-Context Block Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2602.05305)]
  <sub>Generating long-form content, such as minute-long videos and extended texts, is increasingly important for modern generative models. Block diffusion improves inference efficiency via KV caching and bl…</sub>
- [2026/02] **Unifying Masked Diffusion Models with Various Generation Orders and Beyond** *arXiv* [[paper](https://arxiv.org/abs/2602.02112)]
  <sub>Masked diffusion models (MDMs) are a potential alternative to autoregressive models (ARMs) for language generation, but generation quality depends critically on the generation order. Prior work either…</sub>
- [2026/01] **Causal Autoregressive Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2601.22031)]
  <sub>In this work, we propose Causal Autoregressive Diffusion (CARD), a novel framework that unifies the training efficiency of ARMs with the high-throughput inference of diffusion models. CARD reformulate…</sub>
- [2026/01] **Stable-DiffCoder: Pushing the Frontier of Code Diffusion Large Language Model** *arXiv* [[paper](https://arxiv.org/abs/2601.15892)]
  <sub>Diffusion-based language models (DLLMs) offer non-sequential, block-wise generation and richer data reuse compared to autoregressive (AR) models, but existing code DLLMs still lag behind strong AR bas…</sub>
- [2026/01] **Diffusion In Diffusion: Reclaiming Global Coherence in Semi-Autoregressive Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2601.13599)]
  <sub>One of the most compelling features of global discrete diffusion language models is their global bidirectional contextual capability. However, existing block-based diffusion studies tend to introduce…</sub>
- [2025/12] **WeDLM: Reconciling Diffusion Language Models with Standard Causal Attention for Fast Inference** *arXiv* [[paper](https://arxiv.org/abs/2512.22737)]
  <sub>Autoregressive (AR) generation is the standard decoding paradigm for Large Language Models (LLMs), but its token-by-token nature limits parallelism at inference time. Diffusion Language Models (DLLMs)…</sub>
- [2025/11] **TiDAR: Think in Diffusion, Talk in Autoregression** *arXiv* [[paper](https://arxiv.org/abs/2511.08923)]
  <sub>Diffusion language models hold the promise of fast parallel generation, while autoregressive (AR) models typically excel in quality due to their causal structure aligning naturally with language model…</sub>
- [2025/10] **Encoder-Decoder Diffusion Language Models for Efficient Training and Inference** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2510.22852)]
  <sub>Discrete diffusion models enable parallel token sampling for faster inference than autoregressive approaches. However, prior diffusion models use a decoder-only architecture, which requires sampling a…</sub>
- [2025/10] **Continuously Augmented Discrete Diffusion model for Categorical Generative Modeling** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2510.01329)]
  <sub>Standard discrete diffusion models treat all unobserved states identically by mapping them to an absorbing [MASK] token. This creates an 'information void' where semantic information that could be inf…</sub>
- [2025/09] **Sequential Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2509.24007)]
  <sub>Diffusion language models (DLMs) have strong theoretical efficiency but are limited by fixed-length decoding and incompatibility with key-value (KV) caches. Block diffusion mitigates these issues, yet…</sub>
- [2025/06] **Neuro-Symbolic Generative Diffusion Models for Physically Grounded, Robust, and Safe Generation** *arXiv* [[paper](https://arxiv.org/abs/2506.01121)]
  <sub>Despite the remarkable generative capabilities of diffusion models, their integration into safety-critical or scientifically rigorous applications remains hindered by the need to ensure compliance wit…</sub>
- [2025/05] **Unifying Continuous and Discrete Text Diffusion with Non-simultaneous Diffusion Processes** *ACL 2025* [[paper](https://arxiv.org/abs/2505.22165)]
  <sub>Diffusion models have emerged as a promising approach for text generation, with recent works falling into two main categories: discrete and continuous diffusion models. Discrete diffusion models apply…</sub>
- [2025/05] **EZ-VC: Easy Zero-shot Any-to-Any Voice Conversion** *EMNLP 2025* [[paper](https://arxiv.org/abs/2505.16691)]
  <sub>Voice Conversion research in recent times has increasingly focused on improving the zero-shot capabilities of existing methods. Despite remarkable advancements, current architectures still tend to str…</sub>
- [2025/03] **State Fourier Diffusion Language Model (SFDLM): A Scalable, Novel Iterative Approach to Language Modeling** *arXiv* [[paper](https://arxiv.org/abs/2503.17382)]
  <sub>In recent years, diffusion based methods have emerged as a powerful paradigm for generative modeling. Although discrete diffusion for natural language processing has been explored to a lesser extent,…</sub>

## training-objective (35)

_Training objectives, schedules, pretraining recipes, fine-tuning method._

- [2026/05] **Learnability-Informed Fine-Tuning of Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.22939)]
  <sub>We aim to improve the reasoning capabilities of diffusion language models (DLMs). While SFT is a popular post-training recipe for autoregressive models, its use in DLMs faces challenges and can even h…</sub>
- [2026/05] **Uniform Diffusion Models Revisited: Leave-One-Out Denoiser and Absorbing State Reformulation** *arXiv* [[paper](https://arxiv.org/abs/2605.22765)]
  <sub>Discrete diffusion models are often trained through clean-data prediction, but the prediction can be used in different ways to define the reverse dynamics. In Masked Diffusion Models (MDM) these choic…</sub>
- [2026/05] **Continuous Diffusion Scales Competitively with Discrete Diffusion for Language** *arXiv* [[paper](https://arxiv.org/abs/2605.18530)]
  <sub>While diffusion has drawn considerable recent attention from the language modeling community, continuous diffusion has appeared less scalable than discrete approaches. To challenge this belief we revi…</sub>
- [2026/05] **Uncertainty Quantification for Large Language Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2605.14570)]
  <sub>Large Language Diffusion Models (LLDMs) are emerging as an alternative to autoregressive models, offering faster inference through higher parallelism. Similar to autoregressive LLMs, they remain prone…</sub>
- [2026/05] **Support Before Frequency in Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.13999)]
  <sub>Discrete diffusion models are increasingly competitive for language modeling, yet it remains unclear how their denoising objectives organize learning. Although these objectives target the full data di…</sub>
- [2026/05] **Discrete Stochastic Localization for Non-autoregressive Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.12836)]
  <sub>Continuous diffusion is a natural framework for non-autoregressive generation but has generally lagged behind masked discrete diffusion models (MDMs) on discrete sequence generation. We argue that the…</sub>
- [2026/05] **Differences in Text Generated by Diffusion and Autoregressive Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.12522)]
  <sub>Diffusion language models (DLMs) are promising alternatives to autoregressive language models (ARMs), yet the intrinsic differences in their generated text remain underexplored. We first find empirica…</sub>
- [2026/05] **Self-Distilled Trajectory-Aware Boltzmann Modeling: Bridging the Training-Inference Discrepancy in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.11854)]
  <sub>Diffusion Language Models (DLMs) have recently emerged as a promising alternative to autoregressive language models, offering stronger global awareness and highly parallel generation. However, post-tr…</sub>
- [2026/05] **BitLM: Unlocking Multi-Token Language Generation with Bitwise Continuous Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.11577)]
  <sub>Autoregressive language models generate text one token at a time, yet natural language is inherently structured in multi-token units, including phrases, n-grams, and collocations that carry meaning jo…</sub>
- [2026/05] **TD3B: Transition-Directed Discrete Diffusion for Allosteric Binder Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.09810)]
  <sub>Protein function is often controlled by ligands that bias the direction of state transitions, such as agonists and antagonists, rather than stabilizing a single conformation. This is especially import…</sub>
- [2026/05] **DiffRetriever: Parallel Representative Tokens for Retrieval with Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.07210)]
  <sub>PromptReps showed that an autoregressive language model can be used directly as a retriever by prompting it to generate dense and sparse representations of a query or passage. Extending this to multip…</sub>
- [2026/04] **TRIMS: Trajectory-Ranked Instruction Masked Supervision for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.00666)]
  <sub>Diffusion language models (DLMs) offer a promising path toward low-latency generation through parallel decoding, but their practical efficiency depends heavily on the decoding trajectory. In practice,…</sub>
- [2026/03] **Generalized Discrete Diffusion from Snapshots** *arXiv* [[paper](https://arxiv.org/abs/2603.21342)]
  <sub>We introduce Generalized Discrete Diffusion from Snapshots (GDDS), a unified framework for discrete diffusion modeling that supports arbitrary noising processes over large discrete state spaces. Our f…</sub>
- [2026/03] **Diffutron: A Masked Diffusion Language Model for Turkish Language** *arXiv* [[paper](https://arxiv.org/abs/2603.20466)]
  <sub>Masked Diffusion Language Models (MDLMs) have emerged as a compelling non-autoregressive alternative to standard large language models; however, their application to morphologically rich languages rem…</sub>
- [2026/03] **Learning Permutation Distributions via Reflected Diffusion on Ranks** *arXiv* [[paper](https://arxiv.org/abs/2603.17353)]
  <sub>The finite symmetric group S_n provides a natural domain for permutations, yet learning probability distributions on S_n is challenging due to its factorially growing size and discrete, non-Euclidean…</sub>
- [2026/03] **Self-Aware Markov Models for Discrete Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2603.16661)]
  <sub>Standard masked discrete diffusion models face limitations in reasoning tasks due to their inability to correct their own mistakes on the masking path. Since they rely on a fixed number of denoising s…</sub>
- [2026/03] **Generalized Discrete Diffusion with Self-Correction** *arXiv* [[paper](https://arxiv.org/abs/2603.02230)]
  <sub>Self-correction is an effective technique for maintaining parallel sampling in discrete diffusion models with minimal performance degradation. Prior work has explored self-correction at inference time…</sub>
- [2026/03] **D3LM: A Discrete DNA Diffusion Language Model for Bidirectional DNA Understanding and Generation** *arXiv* [[paper](https://arxiv.org/abs/2603.01780)]
  <sub>Early DNA foundation models adopted BERT-style training, achieving good performance on DNA understanding tasks but lacking generative capabilities. Recent autoregressive models enable DNA generation,…</sub>
- [2026/02] **Just on Time: Token-Level Early Stopping for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.11133)]
  <sub>Diffusion language models generate text through iterative refinement, a process that is often computationally inefficient because many tokens reach stability long before the final denoising step. We i…</sub>
- [2026/02] **Stop Training for the Worst: Progressive Unmasking Accelerates Masked Diffusion Training** *arXiv* [[paper](https://arxiv.org/abs/2602.10314)]
  <sub>Masked Diffusion Models (MDMs) have emerged as a promising approach for generative modeling in discrete spaces. By generating sequences in any order and allowing for parallel decoding, they enable fas…</sub>
- [2026/02] **Reversible Diffusion Decoding for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.00150)]
  <sub>Diffusion language models enable parallel token generation through block-wise decoding, but their irreversible commitments can lead to stagnation, where the reverse diffusion process fails to make fur…</sub>
- [2026/01] **Towards Latent Diffusion Suitable For Text** *arXiv* [[paper](https://arxiv.org/abs/2601.16220)]
  <sub>Language diffusion models aim to improve sampling speed and coherence over autoregressive LLMs. We introduce Neural Flow Diffusion Models for language generation, an extension of NFDM that enables the…</sub>
- [2025/12] **Fast-Decoding Diffusion Language Models via Progress-Aware Confidence Schedules** *arXiv* [[paper](https://arxiv.org/abs/2512.02892)]
  <sub>Diffusion large language models (dLLMs) offer a promising alternative to autoregressive models, but their practical utility is severely hampered by slow, iterative sampling. We present SchED, a traini…</sub>
- [2025/11] **Masks Can Be Distracting: On Context Comprehension in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2511.21338)]
  <sub>Masked Diffusion Language Models (MDLMs) have recently emerged as a promising alternative to Autoregressive Language Models (ARLMs), leveraging a denoising objective that, in principle, should enable…</sub>
- [2025/11] **Masked Diffusion Models are Secretly Learned-Order Autoregressive Models** *arXiv* [[paper](https://arxiv.org/abs/2511.19152)]
  <sub>Masked Diffusion Models (MDMs) have emerged as one of the most promising paradigms for generative modeling over discrete domains. It is known that MDMs effectively train to decode tokens in a random o…</sub>
- [2025/11] **Diffusion Language Models are Super Data Learners** *arXiv* [[paper](https://arxiv.org/abs/2511.03276)]
  <sub>Under strictly controlled pre-training settings, we observe a Crossover: when unique data is limited, diffusion language models (DLMs) consistently surpass autoregressive (AR) models by training for m…</sub>
- [2025/10] **Efficient Parallel Samplers for Recurrent-Depth Models and Their Connection to Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2510.14961)]
  <sub>Language models with recurrent depth, also referred to as universal or looped when considering transformers, are defined by the capacity to increase their computation through the repetition of layers.…</sub>
- [2025/10] **Next Semantic Scale Prediction via Hierarchical Diffusion Language Models** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2510.08632)]
  <sub>In this paper we introduce Hierarchical Diffusion Language Models (HDLM) -- a novel family of discrete diffusion models for language modeling. HDLM builds on a hierarchical vocabulary where low-level…</sub>
- [2025/09] **Discovering Mathematical Equations with Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2509.13136)]
  <sub>Discovering valid and meaningful mathematical equations from observed data plays a crucial role in scientific discovery. While this task, symbolic regression, remains challenging due to the vast searc…</sub>
- [2025/09] **Set Block Decoding is a Language Model Inference Accelerator** *arXiv* [[paper](https://arxiv.org/abs/2509.04185)]
  <sub>Autoregressive next token prediction language models offer powerful capabilities but face significant challenges in practical deployment due to the high computational and memory costs of inference, pa…</sub>
- [2025/08] **Whisfusion: Parallel ASR Decoding via a Diffusion Transformer** *arXiv* [[paper](https://arxiv.org/abs/2508.07048)]
  <sub>Fast Automatic Speech Recognition (ASR) is critical for latency-sensitive applications such as real-time captioning and meeting transcription. However, truly parallel ASR decoding remains challenging…</sub>
- [2025/07] **DiffNMR: Diffusion Models for Nuclear Magnetic Resonance Spectra Elucidation** *arXiv* [[paper](https://arxiv.org/abs/2507.08854)]
  <sub>Nuclear Magnetic Resonance (NMR) spectroscopy is a central characterization method for molecular structure elucidation, yet interpreting NMR spectra to deduce molecular structures remains challenging…</sub>
- [2025/07] **Discrete Diffusion Models for Language Generation** *arXiv* [[paper](https://arxiv.org/abs/2507.07050)]
  <sub>Diffusion models have emerged as a powerful class of generative models, achieving state-of-the-art results in continuous data domains such as image and video generation. Their core mechanism involves…</sub>
- [2025/05] **Diffusion vs. Autoregressive Language Models: A Text Embedding Perspective** *EMNLP 2025* [[paper](https://arxiv.org/abs/2505.15045)]
  <sub>Large language model (LLM)-based embedding models, benefiting from large scale pre-training and post-training, have begun to surpass BERT and T5-based models on general-purpose text embedding tasks su…</sub>
- [2025/04] **Target Concrete Score Matching: A Holistic Framework for Discrete Diffusion** *ICML 2025 poster* [[paper](https://arxiv.org/abs/2504.16431)]
  <sub>Discrete diffusion is a promising framework for modeling and generating discrete data. In this work, we present Target Concrete Score Matching (TCSM), a novel and versatile objective for training and…</sub>

## sampling-efficiency (58)

_Faster inference: fewer steps, parallel decoding, KV cache, distillation for speed._

- [2026/05] **DiLaDiff: Distilled Latent-Augmented Diffusion for Language Modeling** *arXiv* [[paper](https://arxiv.org/abs/2605.23605)]
  <sub>Diffusion language models intrinsically fail to capture correlations between decoded tokens, which leads to a harsh trade-off between sampling quality and throughput. To solve this issue, we propose D…</sub>
- [2026/05] **PulseCol: Periodically Refreshed Column-Sparse Attention for Accelerating Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.20813)]
  <sub>Inference in diffusion large language models (dLLMs) is computationally expensive, as full self-attention must be repeatedly executed at each step of the denoising process without KV cache. Recent spa…</sub>
- [2026/05] **Neural Estimation of Pairwise Mutual Information in Masked Discrete Sequence Models** *arXiv* [[paper](https://arxiv.org/abs/2605.20187)]
  <sub>Understanding dependencies between variables is critical for interpretability and efficient generation in masked diffusion models (MDMs), yet these models primarily expose marginal conditional distrib…</sub>
- [2026/05] **Forward-Learned Discrete Diffusion: Learning how to noise to denoise faster** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2605.18204)]
  <sub>Discrete diffusion models are a powerful class of generative models with strong performance across many domains. For efficiency, however, discrete diffusion typically parameterizes the generative (rev…</sub>
- [2026/05] **Understanding and Accelerating the Training of Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.13026)]
  <sub>Masked diffusion models (MDMs) have emerged as a promising alternative to autoregressive models (ARMs) for language modeling. However, MDMs are known to learn substantially more slowly than ARMs, whic…</sub>
- [2026/05] **Orthrus: Memory-Efficient Parallel Token Generation via Dual-View Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.12825)]
  <sub>We introduce Orthrus, a simple and efficient dual-architecture framework that unifies the exact generation fidelity of autoregressive Large Language Models (LLMs) with the high-speed parallel token ge…</sub>
- [2026/05] **Dystruct: Dynamically Structured Diffusion Language Model Decoding via Bayesian Inference** *arXiv* [[paper](https://arxiv.org/abs/2605.09820)]
  <sub>Diffusion language models (DLMs) have recently emerged as a promising alternative to autoregressive models, primarily due to their ability to enable parallel decoding. Despite this advantage, most exi…</sub>
- [2026/05] **DARE: Diffusion Language Model Activation Reuse for Efficient Inference** *arXiv* [[paper](https://arxiv.org/abs/2605.08134)]
  <sub>Diffusion Large Language Models (dLLMs) have emerged as a promising alternative to auto-regressive (AR) models, offering greater expressive capacity and potential for parallel generation and faster in…</sub>
- [2026/05] **Towards Closing the Autoregressive Gap in Language Modeling via Entropy-Gated Continuous Bitstream Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2605.07013)]
  <sub>Diffusion language models (DLMs) promise parallel, order-agnostic generation, but on standard benchmarks they have historically lagged behind autoregressive models in sample quality and diversity. Rec…</sub>
- [2026/05] **Consistent Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.00161)]
  <sub>Diffusion language models (DLMs) are an attractive alternative to autoregressive models because they promise sublinear-time, parallel generation, yet practical gains remain elusive as high-quality sam…</sub>
- [2026/04] **Measuring Temporal Linguistic Emergence in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.23235)]
  <sub>Diffusion language models expose an explicit denoising trajectory, making it possible to ask when different kinds of information become measurable during generation. We study three independent 32-step…</sub>
- [2026/04] **NI Sampling: Accelerating Discrete Diffusion Sampling by Token Order Optimization** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2604.18471)]
  <sub>Discrete diffusion language models (dLLMs) have recently emerged as a promising alternative to traditional autoregressive approaches, offering the flexibility to generate tokens in arbitrary orders an…</sub>
- [2026/04] **LoSA: Locality Aware Sparse Attention for Block-Wise Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.12056)]
  <sub>Block-wise diffusion language models (DLMs) generate multiple tokens in any order, offering a promising alternative to the autoregressive decoding pipeline. However, they still remain bottlenecked by…</sub>
- [2026/04] **Introspective Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.11035)]
  <sub>Diffusion language models promise parallel generation, yet still lag behind autoregressive (AR) models in quality. We stem this gap to a failure of introspective consistency: AR models agree with thei…</sub>
- [2026/04] **Attention-Based Sampler for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.08564)]
  <sub>Auto-regressive models (ARMs) have established a dominant paradigm in language modeling. However, their strictly sequential decoding paradigm imposes fundamental constraints on both inference efficien…</sub>
- [2026/04] **Dependency-Guided Parallel Decoding in Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.02560)]
  <sub>Discrete diffusion language models (dLLMs) accelerate text generation by unmasking multiple tokens in parallel. However, parallel decoding introduces a distributional mismatch: it approximates the joi…</sub>
- [2026/04] **OSCAR: Orchestrated Self-verification and Cross-path Refinement** *arXiv* [[paper](https://arxiv.org/abs/2604.01624)]
  <sub>Diffusion language models (DLMs) expose their denoising trajectories, offering a natural handle for inference-time control; accordingly, an ideal hallucination mitigation framework should intervene du…</sub>
- [2026/04] **Expert-Choice Routing Enables Adaptive Computation in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.01622)]
  <sub>Diffusion language models (DLMs) enable parallel, non-autoregressive text generation, yet existing DLM mixture-of-experts (MoE) models inherit token-choice (TC) routing from autoregressive systems, le…</sub>
- [2026/03] **S2D2: Fast Decoding for Diffusion LLMs via Training-Free Self-Speculation** *arXiv* [[paper](https://arxiv.org/abs/2603.25702)]
  <sub>Block-diffusion language models offer a promising path toward faster-than-autoregressive generation by combining block-wise autoregressive decoding with within-block parallel denoising. However, in th…</sub>
- [2026/03] **Beyond Masks: Efficient, Flexible Diffusion Language Models via Deletion-Insertion Processes** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2603.23507)]
  <sub>While Masked Diffusion Language Models (MDLMs) relying on token masking and unmasking have shown promise in language modeling, their computational efficiency and generation flexibility remain constrai…</sub>
- [2026/03] **Autoregressive vs. Masked Diffusion Language Models: A Controlled Comparison** *arXiv* [[paper](https://arxiv.org/abs/2603.22075)]
  <sub>We present a controlled empirical comparison between autoregressive (AR) and masked diffusion (MDLM) language models. Both models are trained on identical data (50M tokens from TinyStories), identical…</sub>
- [2026/03] **Beyond Single Tokens: Distilling Discrete Diffusion Models via Discrete MMD** *arXiv* [[paper](https://arxiv.org/abs/2603.20155)]
  <sub>It is currently difficult to distill discrete diffusion models. In contrast, continuous diffusion literature has many distillation approaches methods that can reduce sampling steps to a handful. Our m…</sub>
- [2026/03] **Are Expressive Encoders Necessary for Discrete Graph Generation?** *arXiv* [[paper](https://arxiv.org/abs/2603.08825)]
  <sub>Discrete graph generation has emerged as a powerful paradigm for modeling graph data, often relying on highly expressive neural backbones such as transformers or higher-order architectures. We revisit…</sub>
- [2026/03] **DyLLM: Efficient Diffusion LLM Inference via Saliency-based Token Selection and Partial Attention** *arXiv* [[paper](https://arxiv.org/abs/2603.08026)]
  <sub>Masked Diffusion Language Models (MDLMs) enable parallel token decoding, providing a promising alternative to the sequential nature of autoregressive generation. However, their iterative denoising pro…</sub>
- [2026/03] **Progressive Refinement Regulation for Accelerating Diffusion Language Model Decoding** *arXiv* [[paper](https://arxiv.org/abs/2603.04514)]
  <sub>Diffusion language models generate text through iterative denoising under a uniform refinement rule applied to all tokens. However, tokens stabilize at different rates in practice, leading to substant…</sub>
- [2026/02] **Rejection Mixing: Fast Semantic Propagation of Mask Tokens for Efficient DLLM Inference** *arXiv* [[paper](https://arxiv.org/abs/2602.22868)]
  <sub>Diffusion Large Language Models (DLLMs) promise fast non-autoregressive inference but suffer a severe quality-speed trade-off in parallel decoding. This stems from the ''combinatorial contradiction''…</sub>
- [2026/02] **dLLM: Simple Diffusion Language Modeling** *arXiv* [[paper](https://arxiv.org/abs/2602.22661)]
  <sub>Although diffusion language models (DLMs) are evolving quickly, many recent models converge on a set of shared components. These components, however, are distributed across ad-hoc research codebases o…</sub>
- [2026/02] **Adaptation to Intrinsic Dependence in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.20126)]
  <sub>Diffusion language models (DLMs) have recently emerged as a promising alternative to autoregressive (AR) approaches, enabling parallel token generation beyond a rigid left-to-right order. Despite grow…</sub>
- [2026/02] **Is Your Diffusion Sampler Actually Correct? A Sampler-Centric Evaluation of Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.19619)]
  <sub>Discrete diffusion language models (dLLMs) provide a fast and flexible alternative to autoregressive models (ARMs) via iterative denoising with parallel updates. However, their evaluation is challengi…</sub>
- [2026/02] **IDLM: Inverse-distilled Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.19066)]
  <sub>Diffusion Language Models (DLMs) have recently achieved strong results in text generation. However, their multi-step sampling leads to slow inference, limiting practical use. To address this, we exten…</sub>
- [2026/02] **Why Any-Order Autoregressive Models Need Two-Stream Attention: A Structural-Semantic Tradeoff** *arXiv* [[paper](https://arxiv.org/abs/2602.16092)]
  <sub>Any-order autoregressive models (AO-ARMs) offer a promising path toward efficient masked diffusion by enabling native key-value caching, but competitive performance has so far required two-stream atte…</sub>
- [2026/02] **DiffuRank: Effective Document Reranking with Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.12528)]
  <sub>Recent advances in large language models (LLMs) have inspired new paradigms for document reranking. While this paradigm better exploits the reasoning and contextual understanding capabilities of LLMs,…</sub>
- [2026/02] **TEAM: Temporal-Spatial Consistency Guided Expert Activation for MoE Diffusion Language Model Acceleration** *arXiv* [[paper](https://arxiv.org/abs/2602.08404)]
  <sub>Diffusion large language models (dLLMs) have recently gained significant attention due to their inherent support for parallel decoding. Building on this paradigm, Mixture-of-Experts (MoE) dLLMs with a…</sub>
- [2026/02] **Stop the Flip-Flop: Context-Preserving Verification for Fast Revocable Diffusion Decoding** *arXiv* [[paper](https://arxiv.org/abs/2602.06161)]
  <sub>Parallel diffusion decoding can accelerate diffusion language model inference by unmasking multiple tokens per step, but aggressive parallelism often harms quality. Revocable decoding mitigates this b…</sub>
- [2026/02] **Swordsman: Entropy-Driven Adaptive Block Partition for Efficient Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.04399)]
  <sub>Block-wise decoding effectively improves the inference speed and quality in diffusion language models (DLMs) by combining inter-block sequential denoising and intra-block parallel unmasking. However,…</sub>
- [2026/02] **SPA-Cache: Singular Proxies for Adaptive Caching in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.02544)]
  <sub>While Diffusion Language Models (DLMs) offer a flexible, arbitrary-order alternative to the autoregressive paradigm, their non-causal nature precludes standard KV caching, forcing costly hidden state…</sub>
- [2026/02] **Focus-dLLM: Accelerating Long-Context Diffusion LLM Inference via Confidence-Guided Context Focusing** *arXiv* [[paper](https://arxiv.org/abs/2602.02159)]
  <sub>Diffusion Large Language Models (dLLMs) deliver strong long-context processing capability in a non-autoregressive decoding paradigm. However, the considerable computational cost of bidirectional full…</sub>
- [2026/02] **Sentence Curve Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.01807)]
  <sub>Language models (LMs) are a central component of modern AI systems, and diffusion-based language models (DLMs) have recently emerged as a competitive alternative. Both paradigms rely on word embedding…</sub>
- [2026/02] **Balancing Understanding and Generation in Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.01362)]
  <sub>In discrete generative modeling, two dominant paradigms demonstrate divergent capabilities: Masked Diffusion Language Models (MDLM) excel at semantic understanding and zero-shot generalization, wherea…</sub>
- [2026/02] **Latent Shadows: The Gaussian-Discrete Duality in Masked Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2602.00792)]
  <sub>Masked discrete diffusion is a dominant paradigm for high-quality language modeling where tokens are iteratively corrupted to a mask state, yet its inference efficiency is bottlenecked by the lack of…</sub>
- [2026/01] **VidLaDA: Bidirectional Diffusion Large Language Models for Efficient Video Understanding** *arXiv* [[paper](https://arxiv.org/abs/2601.17868)]
  <sub>Current Video Large Language Models (Video LLMs) typically encode frames via a vision encoder and employ an autoregressive (AR) LLM for understanding and generation. However, this AR paradigm inevitab…</sub>
- [2026/01] **Auto-Regressive Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2601.16971)]
  <sub>Masked diffusion models (MDMs) have emerged as a promising approach for language modeling, yet they face a performance gap compared to autoregressive models (ARMs) and require more training iterations…</sub>
- [2026/01] **Beyond Hard Masks: Progressive Token Evolution for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.07351)]
  <sub>Diffusion Language Models (DLMs) offer a promising alternative for language modeling by enabling parallel decoding through iterative refinement. However, most DLMs rely on hard binary masking and disc…</sub>
- [2026/01] **DIP: Dynamic In-Context Planner For Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2601.03199)]
  <sub>Diffusion language models (DLMs) have shown strong potential for general natural language tasks with in-context examples. However, due to the bidirectional attention mechanism, DLMs incur substantial…</sub>
- [2025/12] **On the Role of Discreteness in Diffusion LLMs** *arXiv* [[paper](https://arxiv.org/abs/2512.22630)]
  <sub>Diffusion models offer appealing properties for language generation, such as parallel decoding and iterative refinement, but the discrete and highly structured nature of text challenges the direct app…</sub>
- [2025/12] **Distillation of Discrete Diffusion by Exact Conditional Distribution Matching** *arXiv* [[paper](https://arxiv.org/abs/2512.12889)]
  <sub>Discrete diffusion models (DDMs) are a powerful class of generative models for categorical data, but they typically require many function evaluations for a single sample, making inference expensive. E…</sub>
- [2025/12] **Decoding Large Language Diffusion Models with Foreseeing Movement** *arXiv* [[paper](https://arxiv.org/abs/2512.04135)]
  <sub>Large Language Diffusion Models (LLDMs) benefit from a flexible decoding mechanism that enables parallelized inference and controllable generations over autoregressive models. Yet such flexibility int…</sub>
- [2025/12] **Beyond Confidence: Adaptive and Coherent Decoding for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2512.02044)]
  <sub>Diffusion Language Models (DLMs) have recently achieved significant success due to their any-order generation capabilities. However, existing inference methods typically rely on local, immediate-step…</sub>
- [2025/10] **dInfer: An Efficient Inference Framework for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2510.08666)]
  <sub>Diffusion-based large language models (dLLMs) have emerged as a promising alternative to autoregressive (AR) LLMs, leveraging denoising-based generation to enable inherent parallelism. Even more and m…</sub>
- [2025/10] **DiffuSpec: Unlocking Diffusion Language Models for Speculative Decoding** *arXiv* [[paper](https://arxiv.org/abs/2510.02358)]
  <sub>As large language models (LLMs) scale up, accuracy improves, but the autoregressive (AR) nature of decoding increases latency since each token requires a serial forward pass. Speculative decoding addr…</sub>
- [2025/09] **SparseD: Sparse Attention for Diffusion Language Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2509.24014)]
  <sub>While diffusion language models (DLMs) offer a promising alternative to autoregressive models (ARs), existing open-source DLMs suffer from high inference latency. This bottleneck is mainly due to the…</sub>
- [2025/08] **DPad: Efficient Diffusion Language Models with Suffix Dropout** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2508.14148)]
  <sub>Diffusion-based Large Language Models (dLLMs) parallelize text generation by framing decoding as a denoising process, but suffer from high computational overhead since they predict all future suffix t…</sub>
- [2025/08] **Seed Diffusion: A Large-Scale Diffusion Language Model with High-Speed Inference** *arXiv* [[paper](https://arxiv.org/abs/2508.02193)]
  <sub>We present Seed Diffusion Preview, a large-scale language model based on discrete-state diffusion, offering remarkably fast inference speed. Thanks to non-sequential, parallel generation, discrete dif…</sub>
- [2025/07] **Guided Generation for Developable Antibodies** *arXiv* [[paper](https://arxiv.org/abs/2507.02670)]
  <sub>Therapeutic antibodies require not only high-affinity target engagement, but also favorable manufacturability, stability, and safety profiles for clinical effectiveness. These properties are collectiv…</sub>
- [2025/06] **DLM-One: Diffusion Language Models for One-Step Sequence Generation** *arXiv* [[paper](https://arxiv.org/abs/2506.00290)]
  <sub>This paper introduces DLM-One, a score-distillation-based framework for one-step sequence generation with continuous diffusion language models (DLMs). DLM-One eliminates the need for iterative refinem…</sub>
- [2025/05] **dKV-Cache: The Cache for Diffusion Language Models** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2505.15781)]
  <sub>Diffusion Language Models (DLMs) have been seen as a promising competitor for autoregressive language models. However, diffusion language models have long been constrained by slow inference. A core ch…</sub>
- [2025/05] **Learning Long-Context Diffusion Policies via Past-Token Prediction** *arXiv* [[paper](https://arxiv.org/abs/2505.09561)]
  <sub>Reasoning over long sequences of observations and actions is essential for many robotic tasks. Yet, learning effective long-context policies from demonstrations remains challenging. As context length…</sub>
- [2025/05] **DiffPattern-Flex: Efficient Layout Pattern Generation via Discrete Diffusion** *IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems 2025* [[paper](https://arxiv.org/abs/2505.04173)]
  <sub>Recent advancements in layout pattern generation have been dominated by deep generative models. However, relying solely on neural networks for legality guarantees raises concerns in many practical app…</sub>

## benchmarks-evaluation (2)

_New benchmarks or evaluation methodologies._

- [2026/05] **DiffScore: Text Evaluation Beyond Autoregressive Likelihood** *arXiv* [[paper](https://arxiv.org/abs/2605.11601)]
  <sub>Autoregressive language models are widely used for text evaluation, however, their left-to-right factorization introduces positional bias, i.e., early tokens are scored with only leftward context, con…</sub>
- [2025/09] **Masked Diffusion Language Models with Frequency-Informed Training** *Proceedings of the First BabyLM Workshop 2025* [[paper](https://arxiv.org/abs/2509.05056)]
  <sub>We present a masked diffusion language modeling framework for data-efficient training for the BabyLM 2025 Challenge. Our approach applies diffusion training objectives to language modeling under stric…</sub>

## other (59)

_Did not match any category — manual review needed._

- [2026/05] **The Attribution Contract: Feature Attribution for Generative Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.23080)]
  <sub>Feature attribution methods promise to identify which input features matter for a model output. In generative language models, however, it is often unclear what should count as a feature in the first…</sub>
- [2026/05] **MetaDNS: Enhancing Exploration in Discrete Neural Samplers via Well-Tempered Metadynamics** *arXiv* [[paper](https://arxiv.org/abs/2605.21722)]
  <sub>Sampling from discrete distributions with multiple modes and energy barriers is fundamental to machine learning and computational physics. Recent discrete neural samplers like MDNS suffer from mode co…</sub>
- [2026/05] **Drifting Objectives for Refining Discrete Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.19470)]
  <sub>Discrete diffusion language models (DDLMs) generate text by iteratively denoising categorical token sequences, while recent drifting methods for continuous generators suggest that part of this samplin…</sub>
- [2026/05] **AnchorDiff: Topology-Aware Masked Diffusion with Confidence-based Rewriting for Radiology Report Generation** *arXiv* [[paper](https://arxiv.org/abs/2605.17071)]
  <sub>Radiology report generation (RRG) aims to automatically produce clinically accurate textual reports from medical images. Existing methods predominantly rely on autoregressive (AR) language models, who…</sub>
- [2026/05] **AnchorRoute: Human Motion Synthesis with Interval-Routed Sparse Contro** *arXiv* [[paper](https://arxiv.org/abs/2605.14716)]
  <sub>Sparse anchors provide a compact interface for human motion authoring: users specify a few root positions, planar trajectory samples, or body-point targets, while the system synthesizes the full-body…</sub>
- [2026/05] **Where Should Diffusion Enter a Language Model? Geometry-Guided Hidden-State Replacement** *arXiv* [[paper](https://arxiv.org/abs/2605.14368)]
  <sub>Continuous diffusion language models lag behind autoregressive transformers, partly because diffusion is applied in spaces poorly suited to language denoising and token recovery. We propose DiHAL, a g…</sub>
- [2026/05] **The Efficiency Gap in Byte Modeling** *arXiv* [[paper](https://arxiv.org/abs/2605.12928)]
  <sub>Modern language models have historically relied on two dominant design choices: subword tokenization and autoregressive (AR) ordering. These design decisions bake in priors that dictate a model's lear…</sub>
- [2026/05] **Language Modeling with Hyperspherical Flows** *arXiv* [[paper](https://arxiv.org/abs/2605.11125)]
  <sub>Discrete Diffusion Language Models progressed rapidly as an alternative to autoregressive (AR) models, motivated by their parallel generation abilities. However, for tractability, discrete diffusion m…</sub>
- [2026/05] **Path-Dependent Denoising: A Non-Conservative Field Perspective on Order Collapse in Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2605.09303)]
  <sub>Diffusion language models (DLMs) offer a structural alternative to autoregressive generation: denoising can update tokens in arbitrary orders or in parallel rather than along a fixed left-to-right cha…</sub>
- [2026/04] **On the Quantization Robustness of Diffusion Language Models in Coding Benchmarks** *arXiv* [[paper](https://arxiv.org/abs/2604.20079)]
  <sub>Auto-regressive Large Language Models (LLMs) achieve strong performance on coding tasks, but incur high memory and inference costs. Diffusion-based language models (d-LLMs) offer bounded inference cos…</sub>
- [2026/04] **Interpolating Discrete Diffusion Models with Controllable Resampling** *arXiv* [[paper](https://arxiv.org/abs/2604.17310)]
  <sub>Discrete diffusion models form a powerful class of generative models across diverse domains, including text and graphs. However, existing approaches face fundamental limitations. Masked diffusion mode…</sub>
- [2026/04] **Diffusion Language Models for Speech Recognition** *arXiv* [[paper](https://arxiv.org/abs/2604.14001)]
  <sub>Diffusion language models have recently emerged as a leading alternative to standard language models, due to their ability for bidirectional attention and parallel text generation. In this work, we ex…</sub>
- [2026/04] **Learning Discrete Diffusion of Graphs via Free-Energy Gradient Flows** *arXiv* [[paper](https://arxiv.org/abs/2604.11311)]
  <sub>Diffusion-based models on continuous spaces have seen substantial recent progress through the mathematical framework of gradient flows, leveraging the Wasserstein-2 (${W}_2$) metric via the Jordan-Kin…</sub>
- [2026/04] **A Tale of Two Temperatures: Simple, Efficient, and Diverse Sampling from Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.09921)]
  <sub>Much work has been done on designing fast and accurate sampling for diffusion language models (dLLMs). However, these efforts have largely focused on the tradeoff between speed and quality of individu…</sub>
- [2026/04] **Rethinking Token Prediction: Tree-Structured Diffusion Language Model** *arXiv* [[paper](https://arxiv.org/abs/2604.03537)]
  <sub>Discrete diffusion language models have emerged as a competitive alternative to auto-regressive language models, but training them efficiently under limited parameter and memory budgets remains challe…</sub>
- [2026/04] **Generative Frontiers: Why Evaluation Matters for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.02718)]
  <sub>Diffusion language models have seen exciting recent progress, offering far more flexibility in generative trajectories than autoregressive models. This flexibility has motivated a growing body of rese…</sub>
- [2026/04] **Inverse Design of Optical Multilayer Thin Films using Robust Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2604.01106)]
  <sub>Inverse design of optical multilayer stacks seeks to infer layer materials, thicknesses, and ordering from a desired target spectrum. It is a long-standing challenge due to the large design space and…</sub>
- [2026/04] **OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.00688)]
  <sub>We present OmniVoice, a massively multilingual zero-shot text-to-speech (TTS) model that scales to over 600 languages. At its core is a novel diffusion language model-style discrete non-autoregressive…</sub>
- [2026/03] **STRIDE: When to Speak Meets Sequence Denoising for Streaming Video Understanding** *arXiv* [[paper](https://arxiv.org/abs/2603.27593)]
  <sub>Recent progress in video large language models (Video-LLMs) has enabled strong offline reasoning over long and complex videos. However, real-world deployments increasingly require streaming perception…</sub>
- [2026/03] **Lingshu-Cell: A generative cellular world model for transcriptome modeling toward virtual cells** *arXiv* [[paper](https://arxiv.org/abs/2603.25240)]
  <sub>Modeling cellular states and predicting their responses to perturbations are central challenges in computational biology and the development of virtual cells. Existing foundation models for single-cel…</sub>
- [2026/03] **Generating from Discrete Distributions Using Diffusions: Insights from Random Constraint Satisfaction Problems** *arXiv* [[paper](https://arxiv.org/abs/2603.20589)]
  <sub>Generating data from discrete distributions is important for a number of application domains including text, tabular data, and genomic data. Several groups have recently used random $k$-satisfiability…</sub>
- [2026/03] **D5P4: Partition Determinantal Point Process for Diversity in Parallel Discrete Diffusion Decoding** *arXiv* [[paper](https://arxiv.org/abs/2603.19146)]
  <sub>Discrete diffusion models are promising alternatives to autoregressive approaches for text generation, yet their decoding methods remain under-studied. Standard decoding methods for autoregressive mod…</sub>
- [2026/03] **Controllable Accent Normalization via Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2603.14275)]
  <sub>Existing accent normalization methods do not typically offer control over accent strength, yet many applications-such as language learning and dubbing-require tunable accent retention. We propose DLM-…</sub>
- [2026/03] **CoDAR: Continuous Diffusion Language Models are More Powerful Than You Think** *arXiv* [[paper](https://arxiv.org/abs/2603.02547)]
  <sub>We study why continuous diffusion language models (DLMs) have lagged behind discrete diffusion approaches despite their appealing continuous generative dynamics. Under a controlled token--recovery stu…</sub>
- [2026/03] **DUEL: Exact Likelihood for Masked Diffusion via Deterministic Unmasking** *arXiv* [[paper](https://arxiv.org/abs/2603.01367)]
  <sub>Masked diffusion models (MDMs) generate text by iteratively selecting positions to unmask and then predicting tokens at those positions. Yet MDMs lack proper likelihood evaluation: the evidence lower…</sub>
- [2026/02] **Sharp Convergence Rates for Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2602.22505)]
  <sub>Discrete diffusion models have achieved strong empirical performance in text and other symbolic domains, with masked (absorbing-rate) variants emerging as competitive alternatives to autoregressive mo…</sub>
- [2026/02] **DICArt: Advancing Category-level Articulated Object Pose Estimation in Discrete State-Spaces** *arXiv* [[paper](https://arxiv.org/abs/2602.19565)]
  <sub>Articulated object pose estimation is a core task in embodied AI. Existing methods typically regress poses in a continuous space, but often struggle with 1) navigating a large, complex search space an…</sub>
- [2026/02] **Prompt Optimization Via Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.18449)]
  <sub>We propose a diffusion-based framework for prompt optimization that leverages Diffusion Language Models (DLMs) to iteratively refine system prompts through masked denoising. By conditioning on interac…</sub>
- [2026/02] **Sink-Aware Pruning for Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.17664)]
  <sub>Diffusion Language Models (DLMs) incur high inference cost due to iterative denoising, motivating efficient pruning. Existing pruning heuristics largely inherited from autoregressive (AR) LLMs, typica…</sub>
- [2026/02] **The Energy of Falsehood: Detecting Hallucinations via Diffusion Model Likelihoods** *Proceedings of the Ninth Fact Extraction and VERification Workshop (FEVER) 2026* [[paper](https://arxiv.org/abs/2602.11364)]
  <sub>Large Language Models (LLMs) frequently hallucinate plausible but incorrect assertions, a vulnerability often missed by uncertainty metrics when models are confidently wrong. We propose DiffuTruth, an…</sub>
- [2026/02] **TDGNet: Hallucination Detection in Diffusion Language Models via Temporal Dynamic Graphs** *arXiv* [[paper](https://arxiv.org/abs/2602.08048)]
  <sub>Diffusion language models (D-LLMs) offer parallel denoising and bidirectional context, but hallucination detection for D-LLMs remains underexplored. Prior detectors developed for auto-regressive LLMs…</sub>
- [2026/02] **Discrete diffusion samplers and bridges: Off-policy algorithms and applications in latent spaces** *arXiv* [[paper](https://arxiv.org/abs/2602.05961)]
  <sub>Sampling from a distribution $p(x) \propto e^{-\mathcal{E}(x)}$ known up to a normalising constant is an important and challenging problem in statistics. Recent years have seen the rise of a new famil…</sub>
- [2026/02] **ScDiVa: Masked Discrete Diffusion for Joint Modeling of Single-Cell Identity and Expression** *arXiv* [[paper](https://arxiv.org/abs/2602.03477)]
  <sub>Single-cell RNA-seq profiles are high-dimensional, sparse, and unordered, causing autoregressive generation to impose an artificial ordering bias and suffer from error accumulation. To address this, w…</sub>
- [2026/02] **Self-Rewarding Sequential Monte Carlo for Masked Diffusion Language Models** *arXiv* [[paper](https://arxiv.org/abs/2602.01849)]
  <sub>This work presents self-rewarding sequential Monte Carlo (SMC), an inference-time scaling algorithm enabling effective sampling of masked diffusion language models (MDLMs). Our algorithm stems from th…</sub>
- [2026/01] **Diffusion Large Language Models for Black-Box Optimization** *arXiv* [[paper](https://arxiv.org/abs/2601.14446)]
  <sub>Offline black-box optimization (BBO) aims to find optimal designs based solely on an offline dataset of designs and their labels. Such scenarios frequently arise in domains like DNA sequence design an…</sub>
- [2026/01] **GCG Attack On A Diffusion LLM** *arXiv* [[paper](https://arxiv.org/abs/2601.14266)]
  <sub>While most LLMs are autoregressive, diffusion-based LLMs have recently emerged as an alternative method for generation. Greedy Coordinate Gradient (GCG) attacks have proven effective against autoregre…</sub>
- [2026/01] **Revealing the Attention Floating Mechanism in Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2601.07894)]
  <sub>Masked diffusion models (MDMs), which leverage bidirectional attention and a denoising process, are narrowing the performance gap with autoregressive models (ARMs). However, their internal attention m…</sub>
- [2025/12] **Guided Discrete Diffusion for Constraint Satisfaction Problems** *arXiv* [[paper](https://arxiv.org/abs/2512.14765)]
  <sub>We propose discrete diffusion guidance for constraint satisfaction problems (CSPs) and demonstrate its ability to solve Sudoku puzzles without supervision.…</sub>
- [2025/12] **Foundations of Diffusion Models in General State Spaces: A Self-Contained Introduction** *arXiv* [[paper](https://arxiv.org/abs/2512.05092)]
  <sub>Although diffusion models now occupy a central place in generative modeling, introductory treatments commonly assume Euclidean data and seldom clarify their connection to discrete-state analogues. Thi…</sub>
- [2025/11] **Bringing Stability to Diffusion: Decomposing and Reducing Variance of Training Masked Diffusion Models** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2511.18159)]
  <sub>Masked diffusion models (MDMs) are a promising alternative to autoregressive models (ARMs), but they suffer from inherently much higher training variance. High variance leads to noisier gradient estim…</sub>
- [2025/11] **MissHDD: Hybrid Deterministic Diffusion for Hetrogeneous Incomplete Data Imputation** *arXiv* [[paper](https://arxiv.org/abs/2511.14543)]
  <sub>Incomplete data are common in real-world tabular applications, where numerical, categorical, and discrete attributes coexist within a single dataset. This heterogeneous structure presents significant…</sub>
- [2025/11] **A Diffusion Model to Shrink Proteins While Maintaining Their Function** *ICLR 2026 Poster* [[paper](https://arxiv.org/abs/2511.07390)]
  <sub>Many proteins useful in modern medicine or bioengineering are challenging to make in the lab, fuse with other proteins in cells, or deliver to tissues in the body, because their sequences are too long…</sub>
- [2025/10] **Don't Let It Fade: Preserving Edits in Diffusion Language Models via Token Timestep Allocation** *NeurIPS 2025 poster* [[paper](https://arxiv.org/abs/2510.26200)]
  <sub>While diffusion language models (DLMs) enable fine-grained refinement, their practical controllability remains fragile. We identify and formally characterize a central failure mode called update forge…</sub>
- [2025/10] **Variational Masked Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2510.23606)]
  <sub>Masked diffusion models have recently emerged as a flexible framework for discrete generative modeling. However, a key limitation of standard masked diffusion is its inability to effectively capture d…</sub>
- [2025/10] **ProGress: Structured Music Generation via Graph Diffusion and Hierarchical Music Analysis** *arXiv* [[paper](https://arxiv.org/abs/2510.10249)]
  <sub>Artificial Intelligence (AI) for music generation is undergoing rapid developments, with recent symbolic models leveraging sophisticated deep learning and diffusion model algorithms. One drawback with…</sub>
- [2025/10] **What Makes Diffusion Language Models Super Data Learners?** *arXiv* [[paper](https://arxiv.org/abs/2510.04071)]
  <sub>Recent studies have shown that diffusion language models achieve remarkable data efficiency under limited-data constraints, yet the underlying mechanisms remain unclear. In this work, we perform exten…</sub>
- [2025/09] **Double Descent as a Lens for Sample Efficiency in Autoregressive vs. Discrete Diffusion Models** *arXiv* [[paper](https://arxiv.org/abs/2509.24974)]
  <sub>Data scarcity drives the need for more sample-efficient large language models. In this work, we use the double descent phenomenon to holistically compare the sample efficiency of discrete diffusion an…</sub>
- [2025/09] **Scale-Wise VAR is Secretly Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2509.22636)]
  <sub>Autoregressive (AR) transformers have emerged as a powerful paradigm for visual generation, largely due to their scalability, computational efficiency and unified architecture with language and vision…</sub>
- [2025/09] **Parallel Thinking, Sequential Answering: Bridging NAR and AR for Efficient Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2509.20744)]
  <sub>We study reasoning tasks through a framework that integrates auto-regressive (AR) and non-autoregressive (NAR) language models. AR models, which generate text sequentially, excel at producing coherent…</sub>
- [2025/07] **Pyramid Hierarchical Masked Diffusion Model for Imaging Synthesis** *IEEE International Joint Conference on Neural Network 2025* [[paper](https://arxiv.org/abs/2507.16579)]
  <sub>Medical image synthesis plays a crucial role in clinical workflows, addressing the common issue of missing imaging modalities due to factors such as extended scan times, scan corruption, artifacts, pa…</sub>
- [2025/07] **Perfect diffusion is $\mathsf{TC}^0$ -- Bad diffusion is Turing-complete** *arXiv* [[paper](https://arxiv.org/abs/2507.12469)]
  <sub>This paper explores the computational complexity of diffusion-based language modeling. We prove a dichotomy based on the quality of the score-matching network in a diffusion model. In one direction, a…</sub>
- [2025/07] **Predicting and generating antibiotics against future pathogens with ApexOracle** *arXiv* [[paper](https://arxiv.org/abs/2507.07862)]
  <sub>Antimicrobial resistance (AMR) is escalating and outpacing current antibiotic development. Thus, discovering antibiotics effective against emerging pathogens is becoming increasingly critical. However…</sub>
- [2025/07] **Your Absorbing Discrete Diffusion Secretly Models the Bayesian Posterior** *arXiv* [[paper](https://arxiv.org/abs/2507.07586)]
  <sub>Discrete diffusion language models learn to reconstruct text from randomly masked inputs, yet under mild assumptions their denoiser already implements the exact Bayesian posterior over the original to…</sub>
- [2025/06] **Any-Order GPT as Masked Diffusion Model: Decoupling Formulation and Architecture** *arXiv* [[paper](https://arxiv.org/abs/2506.19935)]
  <sub>Large language models (LLMs) predominantly use autoregressive (AR) approaches, but masked diffusion models (MDMs) are emerging as viable alternatives. A key challenge in comparing AR and MDM paradigms…</sub>
- [2025/04] **DDPS: Discrete Diffusion Posterior Sampling for Paths in Layered Graphs** *arXiv* [[paper](https://arxiv.org/abs/2504.20754)]
  <sub>Diffusion models form an important class of generative models today, accounting for much of the state of the art in cutting edge AI research. While numerous extensions beyond image and video generatio…</sub>
- [2025/04] **Fashion-RAG: Multimodal Fashion Image Editing via Retrieval-Augmented Generation** *IEEE International Joint Conference on Neural Network 2025* [[paper](https://arxiv.org/abs/2504.14011)]
  <sub>In recent years, the fashion industry has increasingly adopted AI technologies to enhance customer experience, driven by the proliferation of e-commerce platforms and virtual applications. Among the v…</sub>
- [2025/03] **Unified Multimodal Discrete Diffusion** *arXiv* [[paper](https://arxiv.org/abs/2503.20853)]
  <sub>Multimodal generative models that can understand and generate across multiple modalities are dominated by autoregressive (AR) approaches, which process tokens sequentially from left to right, or top t…</sub>
- [2025/02] **DiffListener: Discrete Diffusion Model for Listener Generation** *IEEE International Conference on Acoustics, Speech, and Signal Processing 2025* [[paper](https://arxiv.org/abs/2502.06822)]
  <sub>The listener head generation (LHG) task aims to generate natural nonverbal listener responses based on the speaker's multimodal cues. While prior work either rely on limited modalities (e.g. audio and…</sub>
- [2025/01] **D3RM: A Discrete Denoising Diffusion Refinement Model for Piano Transcription** *IEEE International Conference on Acoustics, Speech, and Signal Processing 2025* [[paper](https://arxiv.org/abs/2501.05068)]
  <sub>Diffusion models have been widely used in the generative domain due to their convincing performance in modeling complex data distributions. Moreover, they have shown competitive results on discriminat…</sub>
