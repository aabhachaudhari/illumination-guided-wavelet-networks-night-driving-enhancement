# Unsupervised Illumination-Guided Wavelet Networks for Night-Driving Image Enhancement

This repository contains the **proposed research work** for developing an **Unsupervised Illumination-Guided Wavelet Network (IGWNet)** to enhance night-driving images.  
**Note:** The implementation is currently in the **proposal and design phase**, and the full model training and code execution are **not yet completed**. This repository currently documents the methodology, architecture, planned pipeline, literature foundation, and dataset usage, which will guide future implementation.

Night-time driving images often suffer from low illumination, reduced contrast, and high noise, posing challenges for autonomous and driver-assistance vision systems. The proposed model aims to improve visibility and preserve structural details **without requiring paired low-light/high-light training images**, achieving natural and artifact-free enhancement.

---

## 🎯 **Objective**
- Design a wavelet and illumination-guided enhancement network for night-driving images.
- Preserve textures, edges, and scene structure while improving brightness.
- Develop an **unsupervised learning strategy** that does not rely on ground-truth enhanced images.

---

## 🧠 **Proposed Method**
| Component | Role |
|----------|------|
| **Wavelet Transform Module** | Separates image into frequency components for targeted enhancement |
| **Illumination Guidance Module** | Learns exposure and lighting correction |
| **Texture Refinement Block** | Restores high-frequency road and object structures |
| **Unsupervised Reconstruction Losses** | Supports training without paired enhancement data |

> *Implementation of the modules is ongoing and planned to be completed in upcoming development iterations.*

---

## 🏗️ **Current Repository Status**
| Stage | Status |
|-------|--------|
| Literature Review | ✅ Completed |
| Model Architecture Design | ✅ Defined |
| Dataset Selection | ✅ Identified (ExDark, BDD100K Night subset, LoLi-Phone) |
| Training Code | 🚧 **In Progress** |
| Testing and Evaluation | ❌ Not Started |
| Final Model & Results | ❌ Pending Implementation |

---

## 📦 Planned Dependencies (for implementation)
- Python 3.8+
- PyTorch / TensorFlow
- OpenCV
- NumPy
- Matplotlib

---

## 📝 **Future Work**
- Implement wavelet decomposition layer for feature extraction.
- Train model on selected night-driving datasets.
- Evaluate performance using **PSNR**, **SSIM**, and **NIQE**.
- Compare results with existing low-light enhancement methods.

---

## 🧭 **Applications (Post-Completion)**
- Autonomous vehicle vision enhancement
- ADAS (Advanced Driver Assistance Systems)
- Night surveillance and road safety systems

---

## 📜 License
This project is intended **for academic and research purposes only**.

