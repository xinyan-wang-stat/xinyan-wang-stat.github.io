---
layout: post
date: 2026-05-09 12:00:00-0500
inline: true
related_posts: false
---

**ROM** is on [arXiv](https://arxiv.org/abs/2603.22016). We frame overthinking in large reasoning models as a latent productive-to-redundant transition that surfaces in hidden states around first-correct-solution (FCS) boundaries, and propose **ROM**, a model-agnostic streaming framework that monitors a *frozen* LRM with a lightweight hidden-state detector and intervenes at well-formed reasoning boundaries. Our **Counterfactual Self-Correction (CSC)** augmentation preserves useful pre-FCS self-correction while labeling only post-FCS continuation as redundant. On Qwen3-8B and DeepSeek-R1-Distill-Qwen-32B across MATH500, GSM8K, AIME25, and MMLU-Pro, ROM improves the accuracy–length tradeoff (e.g., Qwen3-8B: 4262 → 3107 tokens with slightly higher accuracy), stacks with L1 for another ~21% token reduction at zero accuracy loss, and cuts wall-clock latency by 46.5%. Check out our [project page](https://xinyan-wang-stat.github.io/ROM-LRM/), [code](https://github.com/SaFo-Lab/ROM), and [dataset](https://huggingface.co/datasets/xinyan-wang/ROM).
