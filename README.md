# DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval

[![YouTube Demo](https://img.shields.io/badge/YouTube-Demo-red?logo=youtube)](https://www.youtube.com/watch?v=1aLHfbPiyJc)
[![IEEE Paper](https://img.shields.io/badge/IEEE-Paper-blue?logo=ieee)](https://ieeexplore.ieee.org/document/10418885)

**DualShape** is a sketch-based 3D modeling system that allows users to create detailed models by combining part generation and part retrieval. It enables intuitive and efficient 3D design even for users without modeling experience.

---

## 🔍 Overview

Traditional sketch-based 3D modeling is often limited by the ambiguity and sparsity of user input. **DualShape** addresses this with a four-stage hybrid pipeline:

1. **Part Retrieval** – Based on sketch similarity using BoF + GALIF features (e.g., tire parts)
2. **Part Generation** – Using SDF-based deep learning for generating complex components (e.g., car shells)
3. **Part Assembly** – Geometric rules for alignment, proportion, and overlap
4. **Model Refinement** – Manual editing of part position and scale for final adjustment

---

## 🧠 Framework Overview

![DualShape Framework](./assets/dualshape_framework.png)

> *Note: Replace the image path above with the actual location of your framework diagram (e.g., `assets/framework.png`).*

---

## 🎥 Demo Video

[![Watch Demo on YouTube](https://img.youtube.com/vi/1aLHfbPiyJc/0.jpg)](https://www.youtube.com/watch?v=1aLHfbPiyJc)

---

## ✨ Key Features

- ✏️ Real-time sketching interface with shadow guidance
- 🔧 Hybrid part-based modeling: generation + retrieval
- 🧩 Intuitive assembly and scaling tools
- 🌐 Extensible to other categories (cars, chairs, tables...)

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

## 📐 Results & Evaluation

| Metric               | DualShape | MeshSDF | Sketch2Mesh |
|----------------------|-----------|---------|-------------|
| Chamfer Distance ↓   | **2.53e-3** | 4.28e-3 | 3.09e-3     |
| Normal Consistency ↑ | 89.21%    | 90.68%  | 90.75%      |

- DualShape preserves more **detail in fine components** like tires  
- Ensures **clear structural alignment** between parts  
- Achieves better overall user satisfaction in usability tests

---

## 📁 Dataset Summary

- 🧱 Part dataset: 1000 labeled car part models (500 shells + 500 tires)
- 🖼 Sketch dataset: 18,000 shell contours + 51,000 tire contours
- 🛠 Contour extraction using Canny & OpenSSE

---

## 🧑‍💻 Authors

* **Xusheng Du** – [JAIST](https://www.jaist.ac.jp/)
* **Tianyu Zhang** – [JAIST](https://www.jaist.ac.jp/)
* **Haoran Xie** – Associate Professor, [JAIST](https://www.jaist.ac.jp/)

---

## 📄 Citation

If you use this work, please cite:

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



