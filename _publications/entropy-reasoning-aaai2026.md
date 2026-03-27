---
title: "Reasoning with Exploration: An Entropy Perspective"
authors: "Daixuan Cheng, Shaohan Huang, Xuekai Zhu, <u>Bo Dai</u>, Wayne Xin Zhao, Zhenliang Zhang, Furu Wei"
venue: "AAAI 2026"
date: 2025-06-18

# Links
pdf: https://arxiv.org/pdf/2506.14758.pdf
arxiv: https://arxiv.org/abs/2506.14758
code: 
dataset: 
project: 
video: 
poster: 
slides: 
doi: 

# Teaser image (第一张图 Fig.1)
teaser: /publications/files/entropy_reasoning_fig1.png

# 首页列表显示的缩略图
thumbnail: /publications/files/entropy_reasoning_fig1.png

# BibTeX citation
bibtex: |
  @inproceedings{cheng2026reasoning,
    title={Reasoning with Exploration: An Entropy Perspective},
    author={Cheng, Daixuan and Huang, Shaohan and Zhu, Xuekai and Dai, Bo and Zhao, Wayne Xin and Zhang, Zhenliang and Wei, Furu},
    booktitle={AAAI Conference on Artificial Intelligence},
    year={2026}
  }
---

## Abstract

Balancing exploration and exploitation is a central goal in reinforcement learning (RL). Despite recent advances in enhancing large language model (LLM) reasoning, most methods lean toward exploitation, and increasingly encounter performance plateaus. In this work, we revisit entropy -- a signal of exploration in RL -- and examine its relationship to exploratory reasoning in LLMs.

Through empirical analysis, we uncover positive correlations between high-entropy regions and three types of exploratory reasoning actions:

1. **Pivotal tokens** that determine or connect logical steps
2. **Reflective actions** such as self-verification and correction
3. **Rare behaviors** under-explored by the base LLMs

Motivated by this, we introduce a minimal modification to standard RL with only one line of code: augmenting the advantage function with an entropy-based term. Unlike traditional maximum-entropy methods which encourage exploration by promoting uncertainty, we encourage exploration by promoting longer and deeper reasoning chains.

Notably, our method achieves significant gains on the Pass@K metric -- an upper-bound estimator of LLM reasoning capabilities -- even when evaluated with extremely large K values, pushing the boundaries of LLM reasoning.

## Citation

```bibtex
@inproceedings{cheng2026reasoning,
  title={Reasoning with Exploration: An Entropy Perspective},
  author={Cheng, Daixuan and Huang, Shaohan and Zhu, Xuekai and Dai, Bo and Zhao, Wayne Xin and Zhang, Zhenliang and Wei, Furu},
  booktitle={AAAI Conference on Artificial Intelligence},
  year={2026}
}
```
