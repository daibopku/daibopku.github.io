---
title: "PhyRecon: Physically Plausible Neural Scene Reconstruction"
authors: "Junfeng Ni, Yixin Chen, Bohan Jing, Nan Jiang, Bin Wang, <u>Bo Dai</u>, Puhao Li, Yixin Zhu, Song-Chun Zhu, Siyuan Huang"
venue: "NeurIPS 2024"
date: 2024-04-25

# Links
pdf: https://arxiv.org/pdf/2404.16666.pdf
arxiv: https://arxiv.org/abs/2404.16666
code: 
dataset: 
project: https://phyrecon.github.io/
video: 
poster: 
slides: 
doi: 

# Teaser image (第一张图 Fig.1)
teaser: /publications/files/phyrecon_teaser.png

# 首页列表显示的缩略图
thumbnail: /publications/files/phyrecon_teaser.png

# BibTeX citation
bibtex: |
  @inproceedings{ni2024phyrecon,
    title={PhyRecon: Physically Plausible Neural Scene Reconstruction},
    author={Ni, Junfeng and Chen, Yixin and Jing, Bohan and Jiang, Nan and Wang, Bin and Dai, Bo and Li, Puhao and Zhu, Yixin and Zhu, Song-Chun and Huang, Siyuan},
    booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
    year={2024}
  }
---

## Abstract

We address the issue of physical implausibility in multi-view neural reconstruction. While implicit representations have gained popularity in multi-view 3D reconstruction, previous work struggles to yield physically plausible results, limiting their utility in domains requiring rigorous physical accuracy.

This lack of plausibility stems from the absence of physics modeling in existing methods and their inability to recover intricate geometrical structures. In this paper, we introduce **PHYRECON**, the first approach to leverage both differentiable rendering and differentiable physics simulation to learn implicit surface representations.

PHYRECON features a novel differentiable particle-based physical simulator built on neural implicit representations. Central to this design is an efficient transformation between SDF-based implicit representations and explicit surface points via our proposed **Surface Points Marching Cubes (SP-MC)**, enabling differentiable learning with both rendering and physical losses.

Additionally, PHYRECON models both rendering and physical uncertainty to identify and compensate for inconsistent and inaccurate monocular geometric priors. The physical uncertainty further facilitates physics-guided pixel sampling to enhance the learning of slender structures.

By integrating these techniques, our model supports differentiable joint modeling of appearance, geometry, and physics. Extensive experiments demonstrate that PHYRECON significantly improves the reconstruction quality. Our results also exhibit superior physical stability in physical simulators, with at least a **40% improvement** across all datasets, paving the way for future physics-based applications.

## Citation

```bibtex
@inproceedings{ni2024phyrecon,
  title={PhyRecon: Physically Plausible Neural Scene Reconstruction},
  author={Ni, Junfeng and Chen, Yixin and Jing, Bohan and Jiang, Nan and Wang, Bin and Dai, Bo and Li, Puhao and Zhu, Yixin and Zhu, Song-Chun and Huang, Siyuan},
  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
  year={2024}
}
```
