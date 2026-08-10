---
layout: post
date: 2026-08-10 12:00:00-0500
inline: true
related_posts: false
---

Our updated **ROM** paper is now on [arXiv](https://arxiv.org/abs/2603.22016). We frame overthinking in large reasoning models as a latent productive-to-redundant transition that is directly decodable from hidden states around first-correct-solution (FCS) boundaries. **ROM** turns this signal into control: a lightweight streaming detector (~0.1% of backbone parameters) monitors a *frozen* LRM and intervenes at well-formed reasoning boundaries — no answer extraction, no probe decoding, no backbone updates. Our **Counterfactual Self-Correction (CSC)** augmentation preserves pre-FCS self-correction. Across five backbones, five benchmarks, and ten baselines under a shared protocol, ROM attains the highest accuracy in 19 of 25 settings, cuts response length 28–77% (mean 45%), and is the only method on the accuracy–length Pareto front in every setting; the same MATH500-trained head transfers zero-shot and cuts wall-clock latency by 46.5%. Check out our [project page](https://xinyan-wang-stat.github.io/ROM-LRM/), [code](https://github.com/SaFo-Lab/ROM), and [dataset](https://huggingface.co/datasets/xinyan-wang/ROM).
