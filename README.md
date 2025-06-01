````markdown
# DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval

[![YouTube Demo](https://img.shields.io/badge/YouTube-Demo-red?logo=youtube)](https://www.youtube.com/watch?v=1aLHfbPiyJc)
[![IEEE Paper](https://img.shields.io/badge/IEEE-Paper-blue?logo=ieee)](https://ieeexplore.ieee.org/document/10418885)

**DualShape** is a novel sketch-based 3D modeling system that enables users to create detailed 3D models by combining deep learning-based part generation with part retrieval from a curated database. This hybrid framework allows both novices and professionals to intuitively design 3D models from free-hand sketches.

---

## 🔍 Overview

Creating 3D shapes from sketches is traditionally challenging due to the sparsity and ambiguity of sketch input. DualShape addresses this challenge by introducing a four-stage hybrid pipeline:

1. **Part Retrieval** – Sketch-based visual feature matching (OpenSSE + BoF-GALIF) for repeated detailed parts (e.g., tires).
2. **Part Generation** – Deep implicit field (SDF) generation for diverse composite parts (e.g., car shells).
3. **Part Assembly** – Auto assembly based on geometric alignment, scale, and overlap rules.
4. **Model Refinement** – Interactive tools for manual position/scale adjustment in the UI.

---

## 🎥 Demo Video

Click below to see the system in action:

[![Watch on YouTube](https://img.youtube.com/vi/1aLHfbPiyJc/0.jpg)](https://www.youtube.com/watch?v=1aLHfbPiyJc)

---

## 🧠 Framework Overview

![DualShape Framework](./figures/dualshape_framework.png)  
*Figure: DualShape hybrid generation pipeline with part retrieval, generation, and assembly.*

> 请将上面图片路径 `./figures/dualshape_framework.png` 替换为你 repo 中对应的图片文件路径（可为 `assets/framework.png` 等）。

---

## ✨ Features

- 🖊️ **Free-hand sketch interface** with real-time shadow guidance
- 🧩 **Hybrid modeling**: retrieval for fine-grained parts, generation for complex parts
- ⚙️ **Auto & manual part assembly**
- 👤 **No 3D modeling skills required**

---

## 🧪 Performance

| Metric         | DualShape | MeshSDF | Sketch2Mesh |
|----------------|-----------|---------|-------------|
| Chamfer Dist. ↓| **2.53e-3** | 4.28e-3 | 3.09e-3     |
| Normal Cons. ↑ | 89.21%    | 90.68%  | 90.75%      |

- ✅ High-detail reconstruction of tires and shell parts
- ✅ Clear structural alignment between assembled components

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

## 📁 Dataset Summary

- 🔧 3D part dataset (1000 models): car shells + tires
- ✏️ Contour dataset: 18,000 car shell sketches, 51,000 tire contours
- 📦 Supports extensible categories: chairs, tables, etc.

---

## 📄 Citation

If you find this project helpful, please cite:

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
````

📖 Official IEEE link: [https://ieeexplore.ieee.org/document/10418885](https://ieeexplore.ieee.org/document/10418885)

---

## 👨‍💻 Authors

* **Xusheng Du** – Japan Advanced Institute of Science and Technology (JAIST)
* **Tianyu Zhang** – JAIST
* **Haoran Xie** – Associate Professor, JAIST


