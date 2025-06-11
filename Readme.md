# HPDC-Net 🌿🔬

**Hybrid Plant Disease Classification Network (HPDC-Net)**  
A lightweight and high-accuracy CNN model designed for real-time plant leaf disease classification.

---

## 📌 Overview

Plant diseases pose a serious threat to global agriculture, affecting yield, quality, and food security. HPDC-Net is a compact and efficient deep learning model tailored for early-stage plant disease classification in resource-constrained environments, such as mobile or edge devices.

The network introduces a hybrid design using three novel modules:
- 🌱 **DSCB**: Depth-wise Separable Convolution Block  
- 🌊 **DAPB**: Dual-Path Adaptive Pooling Block  
- 🎯 **CARB**: Channel-Wise Attention Refinement Block  

Together, these components allow HPDC-Net to extract robust features with minimal computational cost.

---

## ⚙️ Key Features

- ✅ Lightweight (as low as **0.17M** parameters)
- 🚀 Fast Inference (up to **408 FPS** on GPU, **19 FPS** on CPU)
- 🎯 Accuracy > **99%** across multiple datasets (potato & tomato leaves)
- 🧩 Modular design with custom CNN blocks
- 💻 Suitable for **edge deployment** and **mobile applications**

---

## 🧠 Architecture Summary

The model consists of three stages:
1. **DSCB**: Efficient feature extraction using depth-wise separable convolutions.
2. **DAPB**: Enhances spatial and global context via dual-path pooling.
3. **CARB**: Refines important channels using attention mechanisms.

Each block is lightweight yet powerful, enabling end-to-end classification with high precision and low latency.

---

## 📊 Performance Summary

| Dataset         | Classes | Accuracy | Params | GFLOPs | FPS (CPU) | FPS (GPU) |
|----------------|---------|----------|--------|--------|-----------|-----------|
| Potato Leaf    | 03      | 99.7%    | 0.17M  | 0.06   | 19.82     | 408.25    |
| Tomato Leaf    | 10      | 99.1%    | 0.52M  | 0.06   | 19.82     | 408.25    |
| Mixed Leaves   | 13      | 99.3%    | 0.52M  | 0.06   | 19.82     | 408.25    |

---

## 🗂️ Repository Structure

```bash
HPDC-Net/
├── HPDC-Net.ipynb
└── README.md           # Project overview

