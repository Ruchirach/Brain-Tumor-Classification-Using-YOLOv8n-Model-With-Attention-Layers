# Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers

## 🚀 Overview

This project aims to enhance the detection of brain tumors from MRI scans using the YOLOv8n architecture, integrated with advanced attention mechanisms. The attention mechanisms implemented in this project include Enhanced Spatial Attention (ESA), Frequency Channel Attention (FCANet), Iterative Attentional Union (IAU), and ResNeSt (Split-Attention). These mechanisms help improve feature extraction without significantly increasing inference time.

## 🎯 Objectives

- **Detect & Classify**: Multi-class detection of Glioma, Meningioma, and Pituitary tumors.
- **Enhance**: Improve the baseline YOLOv8n architecture using custom attention modules.
- **Compare**: Analyze the performance trade-offs between Spatial, Channel, and Frequency-domain attention strategies.

## 🏗️ Methodologies Implemented

We enhanced the YOLOv8n (Nano) model by integrating the following attention mechanisms:

1. **ESA (Enhanced Spatial Attention)**:
    - Focus: Preserving local spatial context using stride-based scaling.
    - Benefit: Improved boundary detection for small or irregular tumors.
  
2. **FCANet (Frequency Channel Attention)**:
    - Focus: Leveraging the frequency domain (Discrete Cosine Transform) for channel weighting.
    - Benefit: Better texture analysis and energy-based feature selection.
  
3. **IAU (Iterative Attentional Union)**:
    - Focus: Iteratively fusing spatial and channel information.
    - Benefit: Holistic feature refinement and robust feature representation.
  
4. **ResNeSt (Split-Attention)**:
    - Focus: Capturing cross-channel relationships using cardinal groups.
    - Benefit: Multi-path representation power similar to larger networks.

## 📊 Dataset

- **Source**: Medical Image Dataset for Brain Tumor Detection (Figshare/Kaggle).
- **Preprocessing**: Images resized to 640x640, normalized, and split into Train/Val/Test sets.

### Classes:
- 0: Glioma
- 1: Meningioma
- 2: Pituitary

## 🚀 Installation & Usage

### Prerequisites
- Python 3.8+
- PyTorch
- Ultralytics

### Setup

Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers.git
cd Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers
