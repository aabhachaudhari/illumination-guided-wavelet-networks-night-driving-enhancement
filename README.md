# Unsupervised Illumination-Guided Wavelet Networks for Night-Driving Image Enhancement

Night-time driving scenes often suffer from low illumination, reduced visibility, noise interference, and weak contrast—significantly challenging perception systems in autonomous and assisted driving technologies. This project implements an **Unsupervised Illumination-Guided Wavelet Network (IGWNet)** designed to enhance night-driving images without requiring paired low/high-light training data.

The model leverages **wavelet-domain decomposition** and **illumination guidance priors** to restore structural details, amplify visibility, and suppress color distortion—all while maintaining natural brightness distribution.

---

## 🎯 **Key Objectives**
- Enhance visibility in low-light and night-time driving images.
- Improve lane markings, vehicle edges, pedestrian visibility & road contours.
- Avoid overexposure and maintain natural illumination balance.
- Train enhancement model **without paired ground-truth** high-light images.

---

## 🧠 **Core Concept**
The proposed network integrates:
| Component | Purpose |
|----------|---------|
| **Wavelet Decomposition** | Separates texture and illumination components. |
| **Illumination Guidance Module** | Learns exposure correction maps adaptively. |
| **Unsupervised Loss Strategy** | Removes need for labeled enhancement pairs. |

The network enhances contrast and illumination while preserving high-frequency structural details critical for driving environments.

---

## 🏗️ **Model Architecture Overview**
- Wavelet transform layer to decompose image → (LL, LH, HL, HH)
- Illumination estimation sub-network to guide exposure correction
- Texture refinement branch to restore edges and contours
- Multi-scale reconstruction decoder for final enhanced output

---

## 🧪 **Dataset**
This work can be trained and tested on publicly available night-driving datasets such as:
- **LoLi-Phone Night Driving Dataset**
- **ExDark**
- **BDD100K (Night subset)**

(Include dataset links in repository if allowed.)

---

## 📦 **Dependencies**
- Python 3.8+
- PyTorch / TensorFlow (state developer decides)
- OpenCV
- NumPy
- Matplotlib
