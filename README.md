# 🧠 Brain Tumor Classification Using YOLOv8n with Attention Layers
## 🚀 Overview

This project focuses on improving automated brain tumor detection and classification from MRI scans using the YOLOv8 Nano (YOLOv8n) object detection model enhanced with advanced attention mechanisms. Lightweight models like YOLOv8n offer fast inference but often suffer from feature degradation when handling complex medical images. To address this limitation, attention modules are integrated into the YOLOv8n backbone to enhance feature representation while maintaining real-time performance.

The project evaluates the effectiveness of Space–Time Mixing Attention (STMix), Polarized Self-Attention (PSA), and Dual Multi-Scale Attention Network (DMSANet) for detecting and classifying brain tumors.

## 🎯 Objectives

-**Detect & Classify**: Multi-class detection of Glioma, Meningioma, and Pituitary tumors from MRI images.

  -**Enhance Feature Extraction**: Improve spatial, channel, and multi-scale feature learning using attention mechanisms.

  -**Compare Performance**: Analyze detection accuracy and efficiency of different attention strategies integrated into YOLOv8n.

### 🏗️ Methodology

The YOLOv8n model was modified by injecting attention modules after the SPPF layer in the backbone. Each attention mechanism focuses on improving different aspects of feature learning:



1. **Space–Time Mixing Attention (STMix)**

-Focus: Preserving spatial context while enhancing feature interactions.

 -Benefit: Improved detection of tumors with irregular shapes and fine boundaries.

2.**Polarized Self-Attention (PSA)**

  -Focus: Separating spatial and channel attention paths for efficient feature refinement.

  -Benefit: Enhanced feature selectivity with minimal computational overhead.

3.**Dual Multi-Scale Attention Network (DMSANet)**

-Focus: Capturing both global context and local details using multi-scale attention.

  -Benefit: Robust detection across tumors of varying sizes and appearances.

### Dataset

-**Source**: Medical Image Dataset for Brain Tumor Detection (Kaggle / Figshare)

**Modalities**: MRI scans

**Preprocessing**:

-Resized to 640 × 640

-Normalized

-Split into Train / Validation / Test

### Classes

0 – Glioma

1 – Meningioma

2 – Pituitary

###  Experimental Setup

**Framework**: PyTorch + Ultralytics YOLOv8

**Hardware**: Google Colab (Tesla T4 GPU)

**Training Parameters:**

-Epochs: 50

-Batch Size: 16

-Image Size: 640

**Evaluation Metrics:**

-Precision

-Recall

-mAP@50

-mAP@50–95

### 📈 Results Summary

All attention-enhanced models outperformed the baseline YOLOv8n.

STMix improved spatial feature retention and tumor boundary detection.

PSA achieved efficient performance with balanced precision and recall.

DMSANet delivered the best multi-scale representation, especially for pituitary tumors.

These results demonstrate that integrating attention mechanisms significantly improves detection accuracy without sacrificing real-time inference speed.

### 🚀 Installation & Usage
**Prerequisites**

Python 3.8+

PyTorch

Ultralytics

### Setup
      Clone the repository:
       bash
       git clone https://github.com/Ruchirach/Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers.git
      cd Brain-Tumor-Classification-Using-YOLOv8n-Model-With-Attention-Layers
      pip install ultralytics
