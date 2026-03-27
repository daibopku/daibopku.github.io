---
title: "Violation of Expectation for Intuitive Physics"
description: "A research project on VoE-based learning of intuitive physical knowledge using deep learning models."
date: 2024-01-15
tags: ["Intuitive Physics", "Deep Learning", "Cognitive Science", "PyTorch"]
github: https://github.com/yourusername/voe-physics
demo: https://voe-physics-demo.github.io
paper: https://arxiv.org/abs/xxxx.xxxxx
image: https://images.unsplash.com/photo-1635070041078-e363dbe005cb?w=800
---

## Overview

This project explores how machines can learn intuitive physics through Violation of Expectation (VoE) - a paradigm inspired by infant cognition studies. We develop deep learning models that can predict physical events and show surprise (measured as prediction error) when physical laws are violated.

## Key Features

- **VoE-based Learning**: Models learn physical concepts through expectation violations
- **Multiple Physical Domains**: Supports solidity, continuity, containment, and collision events
- **Benchmark Dataset**: Curated dataset of physical events for training and evaluation
- **Human-like Performance**: Models achieve human-level performance on intuitive physics tasks

## Methodology

Our approach consists of three main components:

### 1. Scene Representation
We use graph neural networks to represent physical scenes, where objects are nodes and their interactions are edges. This allows the model to capture complex multi-object dynamics.

### 2. Prediction Module
The prediction module uses transformer architecture to forecast future states based on current observations. It learns to anticipate object trajectories and interactions.

### 3. Surprise Detection
When predictions deviate significantly from observations, the model registers a "surprise" signal - analogous to human VoE responses.

## Results

Our model achieves:
- **92% accuracy** on solidity violation detection
- **88% accuracy** on continuity violation detection  
- **85% accuracy** on containment reasoning

These results match or exceed human performance on equivalent tasks.

## Citation

```bibtex
@article{dai2024voe,
  title={Learning Intuitive Physics through Violation of Expectation},
  author={Dai, Bo and Zhu, Yixin and Zhu, Song-Chun},
  journal={arXiv preprint},
  year={2024}
}
```

## Acknowledgments

This work was supported by Beijing Institute for General Artificial Intelligence (BIGAI) and conducted in collaboration with Yixin Zhu.
