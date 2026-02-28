## Lightweight segmentation of rock-mass cracks based on anisotropic feature modeling for geological hazard monitoring
## Abstract
Automated segmentation of rock-mass cracks is a prerequisite for effective geological hazard assessment; however, accurate segmentation remains a persistent challenge due to the slender geometry, anisotropic nature, and weakly textured appearance of cracks in complex field environments. To overcome these limitations, we propose GDAFNet, a lightweight Geometry and Direction Awareness Fusion Network designed to enhance the discrimination of fine crack structures. The architecture integrates diagonal aggregation convolution with multi-directional perception modules to capture intricate spatial features, while a hierarchical cross-attention decoder is introduced to refine topological crack continuity. Extensive empirical validation on the CrackSeg9k dataset and our proposed GHCrack dataset demonstrates the superiority of this approach. GDAFNet achieves a Mean Intersection over Union (mIoU) of 82.64\% on CrackSeg9k—establishing a new state-of-the-art (SOTA)—and 82.38\% on GHCrack. These results surpass robust CNN and Transformer baselines by 0.8\% and 0.64\%, respectively, and surpassing efficient models by up to 3.48\% and 5.71\%. Notably, GDAFNet achieves this performance with only 0.59 million parameters—a reduction of over 95\% compared to classical networks—thereby offering a highly efficient solution for real-time monitoring.

## Model Architecture
![model overview](fig/overview.png)

## 📁 Project Structure

```plaintext
.
├── 📂 data/                 # Experiment data
│   └── data.jpg       
├── 📂 fig/                    # Model structure diagram
│   └── overview.png       
├── 📂 model/                  # Model architecture definition directory
│   └── our_model.py           # Core model implementation from the paper
└── 📜 README.md               # This file
