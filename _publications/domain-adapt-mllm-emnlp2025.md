---
title: "On Domain-Adaptive Post-Training for Multimodal Large Language Models"
authors: "Daixuan Cheng, Shaohan Huang, Ziyu Zhu, Xintong Zhang, Wayne Xin Zhao, Zhongzhi Luan, <u>Bo Dai</u>, Zhenliang Zhang"
venue: "EMNLP 2025 Findings"
date: 2024-11-29

# Links
pdf: https://arxiv.org/pdf/2411.19930.pdf
arxiv: https://arxiv.org/abs/2411.19930
code: 
dataset: 
project: https://huggingface.co/AdaptLLM/Adapt-MLLM-to-Domains
video: 
poster: 
slides: 
doi: 

# Teaser image (第一张图 Fig.1)
teaser: /publications/files/domain_adapt_mllm_fig1.png

# 首页列表显示的缩略图
thumbnail: /publications/files/domain_adapt_mllm_fig1.png

# BibTeX citation
bibtex: |
  @inproceedings{cheng2024domain,
    title={On Domain-Adaptive Post-Training for Multimodal Large Language Models},
    author={Cheng, Daixuan and Huang, Shaohan and Zhu, Ziyu and Zhang, Xintong and Zhao, Wayne Xin and Luan, Zhongzhi and Dai, Bo and Zhang, Zhenliang},
    booktitle={EMNLP 2025 Findings},
    year={2025}
  }
---

## Abstract

Adapting general multimodal large language models (MLLMs) to specific domains, such as scientific and industrial fields, is highly significant in promoting their practical applications. This paper systematically investigates domain adaptation of MLLMs via post-training, focusing on data synthesis, training pipeline, and task evaluation.

**(1) Data Synthesis**: Using only open-source models, we develop a generate-then-filter pipeline that curates diverse visual instruction tasks based on domain-specific image-caption pairs. The resulting data surpass the data synthesized by manual rules or strong closed-source models in enhancing domain-specific performance.

**(2) Training Pipeline**: Unlike general MLLMs that typically adopt a two-stage training paradigm, we find that a single-stage approach is more effective for domain adaptation.

**(3) Task Evaluation**: We conduct extensive experiments in high-impact domains such as biomedicine, food, and remote sensing, by post-training a variety of MLLMs and then evaluating MLLM performance on various domain-specific tasks.

Finally, we fully open-source our models, code, and data to encourage future research in this area.

## Citation

```bibtex
@inproceedings{cheng2024domain,
  title={On Domain-Adaptive Post-Training for Multimodal Large Language Models},
  author={Cheng, Daixuan and Huang, Shaohan and Zhu, Ziyu and Zhang, Xintong and Zhao, Wayne Xin and Luan, Zhongzhi and Dai, Bo and Zhang, Zhenliang},
  booktitle={EMNLP 2025 Findings},
  year={2025}
}
```
