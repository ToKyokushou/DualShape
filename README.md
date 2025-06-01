DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval

DualShape is a novel sketch-based 3D modeling system that enables users to create detailed 3D models by combining deep learning-based part generation with part retrieval from a curated database. This hybrid framework allows both novices and professionals to intuitively design 3D models from free-hand sketches.

🔍 Overview
Creating 3D shapes from sketches is traditionally challenging due to the sparsity and ambiguity of sketch input. DualShape addresses this challenge by introducing a four-stage hybrid pipeline:

Part Retrieval – Uses sketch-based visual feature matching (via OpenSSE and BoF-GALIF) to retrieve precise components (e.g., tires).

Part Generation – Utilizes deep implicit fields (SDFs) to generate complex components (e.g., car shells) from sketches.

Part Assembly – Automatically assembles retrieved/generated parts using geometric rules (alignment, scale, overlap).

Model Refinement – Allows manual fine-tuning of parts' position and scale via an interactive UI.

✨ Features
🖊️ Free-hand sketch interface with shadow-guidance from retrieved 3D models.

🧩 Hybrid modeling: combines retrieval (for detailed, repeated parts) and generation (for diverse composite parts).

⚙️ User-friendly assembly and editing tools for spatial alignment and scaling.

👤 No professional modeling skills required – beginner-friendly workflow.

📽 Demo Video
Watch the system in action on YouTube:
👉 https://www.youtube.com/watch?v=1aLHfbPiyJc

🧪 Evaluation
📊 Outperforms state-of-the-art methods like MeshSDF and Sketch2Mesh in both detail preservation and part connectivity.

✅ User study with 16 participants shows high satisfaction in usability and results quality.

📐 Metrics:

Chamfer Distance (↓): 2.53 × 10⁻³

Normal Consistency (↑): 89.21%

📁 Dataset & Architecture
💾 Part Dataset: 1000 instances (500 car shells + 500 tires) from ShapePFCN.

🖼 Sketch Dataset: 18,000 car shell contours + 51,000 tire contours.

🧠 Network: ResNet-based encoder + SDF decoder for generation; BoF+GALIF for retrieval.

🖥 System Components
🎨 Real-time browser-based sketching interface

🧠 Retrieval engine using OpenSSE

🔧 Assembly engine with geometric alignment

🪚 Manual refinement tools

📌 Applications
🚗 Car design

🪑 Chair modeling

🧩 Easily extensible to new categories: tables, vases, aircraft, etc.

📄 Citation
If you find this project useful in your research, please cite:

bibtex
复制
编辑
@article{du2024dualshape,
  title={DualShape: Sketch-Based 3D Shape Design With Part Generation and Retrieval},
  author={Du, Xusheng and Zhang, Tianyu and Xie, Haoran},
  journal={IEEE Access},
  volume={12},
  pages={18888--18900},
  year={2024},
  publisher={IEEE}
}
🧑‍💻 Authors
Xusheng Du – JAIST

Tianyu Zhang – JAIST

Haoran Xie – Associate Professor, JAIST

