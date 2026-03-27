---
title: "X-VoE: Measuring eXplanatory Violation of Expectation in Physical Events"
authors: "Bo Dai, Linge Wang, Baoxiong Jia, Song-Chun Zhu, Chi Zhang, Yixin Zhu"
venue: "ICCV 2023"
date: 2023-08-01

# Links
pdf: https://arxiv.org/pdf/2308.10441
arxiv: https://arxiv.org/abs/2308.10441
code: https://github.com/daibopku/X-VoE
dataset: https://huggingface.co/datasets/RuriSama/X-VoE/tree/main
project: https://sites.google.com/view/x-voe
video: https://vimeo.com/855745233
poster: 
slides: 
doi: 

# Teaser image/PDF (论文概念图/第一张图)
# 支持图片格式 (png, jpg, gif) 或 PDF
teaser: files/xvoe_explain.pdf

# 首页列表显示的缩略图（建议 200-300px 宽度）
thumbnail: files/xvoe_explain.pdf

# BibTeX citation
bibtex: |
  @inproceedings{dai2023xvoe,
    title={X-VoE: Measuring eXplanatory Violation of Expectation in Physical Events},
    author={Dai, Bo and Wang, Linge and Jia, Baoxiong and Zhu, Song-Chun and Zhang, Chi and Zhu, Yixin},
    booktitle={ICCV},
    year={2023}
  }
---

## Abstract

Intuitive physics is pivotal for human understanding of the physical world, enabling prediction and interpretation of events even in infancy. Nonetheless, replicating this level of intuitive physics in artificial intelligence (AI) remains a formidable challenge. This study introduces **X-VoE**, a comprehensive benchmark dataset, to assess AI agents’ grasp of intuitive physics. Built on the developmental psychology-rooted **Violation of Expectation (VoE)**  paradigm, X-VoE establishes a higher bar for the explanatory capacities of intuitive physics models. Each VoE scenario within X-VoE encompasses three distinct settings, probing models’ comprehension of events and their underlying explanations. Beyond model evaluation, we present an explanation-based learning system that captures physics dynamics and infers occluded object states solely from visual sequences, without explicit occlusion labels. Experimental outcomes highlight our model’s alignment with human commonsense when tested against X-VoE. A remarkable feature is our model’s ability to visually expound VoE events by reconstructing concealed scenes. Concluding, we discuss the findings’ implications and outline future research directions. Through X-VoE, we catalyze the advancement of AI endowed with human-like intuitive physics capabilities

## Method

Beyond model evaluation, we present an **explanation-based learning system** that captures physics dynamics and infers occluded object states solely from visual sequences, without explicit occlusion labels.

## Results

Experimental outcomes highlight our model's alignment with human commonsense when tested against X-VoE. A remarkable feature is our model's ability to **visually expound VoE events by reconstructing concealed scenes**.

## Citation

If you find this work useful, please consider citing:

```bibtex
@inproceedings{dai2023xvoe,
  title={X-VoE: Measuring eXplanatory Violation of Expectation in Physical Events},
  author={Dai, Bo and Wang, Linge and Jia, Baoxiong and Zhu, Song-Chun and Zhang, Chi and Zhu, Yixin},
  booktitle={ICCV},
  year={2023}
}
```
