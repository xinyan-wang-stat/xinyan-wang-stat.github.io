---
layout: about
title: about
permalink: /
subtitle: xwang2587@wisc.edu.

profile:
  align: right
  image: graduation_square.png
  image_circular: false # crops the image to make circular
  address: >
    <p>5615 Morgridge Hall, 1205 University Avenue, Madison, WI 53706</p>

news: true
latest_posts: false
selected_papers: true
social: true

service:
  - Reviewer of ACL' 26, ECCV' 26, EMNLP' 26, NeurIPS' 26.
---

I am **Xinyan Wang**, a third year PhD student in Statistics at the University of Wisconsin–Madison, advised by [Professor Jun Shao](https://pages.stat.wisc.edu/~shao/) and working with [Professor Chaowei Xiao](https://xiaocw11.github.io/) at Johns Hopkins University. I received my BS in Statistics from East China Normal University in 2022 and MS in Statistics from UW–Madison in 2023. I am also pursuing a MS in Computer Science at UW–Madison.

I work on large reasoning models (LRMs). My goal is to make reasoning models efficient and safe enough to deploy in practice, using reinforcement learning and representation analysis. My current topics of interest include:

- **Efficient Reasoning**: Reducing redundant computation in large reasoning models at inference time — e.g., [ROM](https://arxiv.org/abs/2603.22016), a model-agnostic streaming detector-and-intervention framework that curbs overthinking in frozen LRMs in real time at no accuracy cost.
- **Safety of Reasoning Models**: Understanding and red-teaming the vulnerabilities that long reasoning traces introduce — e.g., [ReasoningBomb](https://arxiv.org/abs/2602.00154) (CCS 2026), a reinforcement-learning-based inference-time denial-of-service attack that traps LRMs into pathologically long reasoning.
- **Reasoning Distillation**: Identifying which teacher signals are reliable when distilling reasoning into models and weighting supervision accordingly — e.g., [PW-OPSD](https://arxiv.org/abs/2605.21606), which shows teacher-token reliability in on-policy self-distillation is position-structured and up-weights reliable later tokens at no extra teacher cost.
