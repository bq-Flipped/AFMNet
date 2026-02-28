## Lightweight segmentation of rock-mass cracks based on anisotropic feature modeling for geological hazard monitoring
## Abstract
Accurate segmentation of rock-mass cracks is essential for geological hazard investigation, yet remains challenging due to the slender morphology, strong anisotropy, and discontinuous distribution of cracks in complex field environments. To address these challenges, we propose a lightweight anisotropic feature modeling network for rock-mass crack segmentation, termed AFMNet. The proposed network enhances orientation-dependent crack representations through an anisotropic feature aggregation module and a multi-orientation perception module in the encoder to effectively capture directional and geometric characteristics of slender cracks. In the decoder, cross-scale attention and axis-gated attention are employed to progressively fuse multi-level features and reinforce structural continuity during feature reconstruction. Furthermore, a dual-task complementary output head is introduced to jointly optimize crack region segmentation and edge detail prediction, enabling boundary information to guide the final segmentation results.  Experimental results on the CrackSeg9k dataset and a self-constructed geological hazard crack dataset (GHCrack) show that AFMNet achieves mIoU scores of 82.64% and 82.38%, respectively, while maintaining a compact model size of only 0.59 million parameters, demonstrating a favorable balance between segmentation accuracy and computational efficiency.

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
