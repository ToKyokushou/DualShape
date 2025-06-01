
---

# DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval

[![YouTube Demo](https://img.shields.io/badge/YouTube-Demo-red?logo=youtube)](https://www.youtube.com/watch?v=1aLHfbPiyJc)

**DualShape** is a novel sketch-based 3D modeling system that enables users to create detailed 3D models by combining deep learning-based part generation with part retrieval from a curated database. This hybrid framework allows both novices and professionals to intuitively design 3D models from free-hand sketches.

---

## 🔍 Overview

Creating 3D shapes from sketches is traditionally challenging due to the sparsity and ambiguity of sketch input. DualShape addresses this challenge by introducing a four-stage hybrid pipeline:

1. **Part Retrieval** – Uses sketch-based visual feature matching (via OpenSSE and BoF-GALIF) to retrieve precise components (e.g., tires).
2. **Part Generation** – Utilizes deep implicit fields (SDFs) to generate complex components (e.g., car shells) from sketches.
3. **Part Assembly** – Automatically assembles retrieved/generated parts using geometric rules (alignment, scale, overlap).
4. **Model Refinement** – Allows manual fine-tuning of parts' position and scale via an interactive UI.

---

## ✨ Features

* 🖊️ **Free-hand sketch interface** with shadow-guidance from retrieved 3D models.
* 🧩 **Hybrid modeling**: combines retrieval (for detailed, repeated parts) and generation (for diverse composite parts).
* ⚙️ **User-friendly assembly** and editing tools for spatial alignment and scaling.
* 👤 **No professional modeling skills required** – beginner-friendly workflow.

---

## 📽 Demo Video

Watch the system in action on YouTube:
👉 [https://www.youtube.com/watch?v=1aLHfbPiyJc](https://www.youtube.com/watch?v=1aLHfbPiyJc)

---

## 🧪 Evaluation

* 📊 Outperforms state-of-the-art methods like MeshSDF and Sketch2Mesh in both detail preservation and part connectivity.
* ✅ User study with 16 participants shows high satisfaction in usability and results quality.
* 📐 Metrics:

  * Chamfer Distance (↓): **2.53 × 10⁻³**
  * Normal Consistency (↑): **89.21%**

---

## 📁 Dataset & Architecture

* 💾 **Part Dataset**: 1000 instances (500 car shells + 500 tires) from ShapePFCN.
* 🖼 **Sketch Dataset**: 18,000 car shell contours + 51,000 tire contours.
* 🧠 **Network**: ResNet-based encoder + SDF decoder for generation; BoF+GALIF for retrieval.

---

## 🖥 System Components

* 🎨 Real-time browser-based sketching interface
* 🧠 Retrieval engine using OpenSSE
* 🔧 Assembly engine with geometric alignment
* 🪚 Manual refinement tools

---

## 📌 Applications

* 🚗 **Car design**
* 🪑 **Chair modeling**
* 🧩 Easily extensible to new categories: tables, vases, aircraft, etc.

---

## 📄 Citation

If you find this project useful in your research, please cite:

```bibtex
@article{du2024dualshape,
  title={DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval},
  author={Du, Xusheng and Zhang, Tianyu and Xie, Haoran},
  journal={IEEE Access},
  volume={12},
  pages={18888--18900},
  year={2024},
  publisher={IEEE}
}
```

---

## 🧑‍💻 Authors

* **Xusheng Du** – [JAIST](https://www.jaist.ac.jp/)
* **Tianyu Zhang** – [JAIST](https://www.jaist.ac.jp/)
* **Haoran Xie** – Associate Professor, [JAIST](https://www.jaist.ac.jp/)

---
