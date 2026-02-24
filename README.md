# 🔍 SDE-DET

**SDE-DET** — A Precision Network for Shatian Pomelo Detection in Complex Orchard Environments

👉 TL;DR: **SDE-DET** provides **training, validation, heatmap visualization, and Docker** — supporting **YOLO, DETR, R-CNN** and more in one unified repo.

<p align="center">
  <a href="https://github.com/yihaohu0118/SDE-DET">
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="40" alt="GitHub"/>
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://doi.org/10.1016/j.atech.2026.101915">
    <img src="https://img.shields.io/badge/Paper-DOI-blue?style=flat-square" width="120" alt="Paper"/>
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://huggingface.co/">
    <img src="https://huggingface.co/front/assets/huggingface_logo-noborder.svg" width="40" alt="Hugging Face"/>
  </a>
</p>

<p align="center">
  <b>💻 Code</b> &nbsp; | &nbsp; <b>📖 Paper</b> &nbsp; | &nbsp; <b>🤗 Weights</b>
</p>

---

## 📄 Paper

📄 **Paper:** [https://doi.org/10.1016/j.atech.2026.101915](https://doi.org/10.1016/j.atech.2026.101915)

> The source code will be published when the paper is accepted. Please refer to subsequent updates.

---

## ✨ Highlights

- 🏗️ **Multi-backbone support** — YOLOv8/9/10, Faster R-CNN, DETR, CenterNet, RTMDet, and more  
- 🏋️ **Full pipeline** — training, validation, heatmap visualization  
- 🐳 **Docker support** — reproducible environment  
- 📦 **Pre-trained weights** — `best.pt` included; larger checkpoints on Hugging Face  
- 📊 **Ablation experiments** — DA and StarNet+DA configurations  

---

## 🔎 Supported Backbones

| Backbone | Type | Description |
|----------|------|-------------|
| YOLOv8n / YOLOv8s | One-stage | Lightweight real-time detectors |
| YOLOv10n / YOLOv10s | One-stage | Efficient YOLO variants |
| YOLOv9-C | One-stage | High-performance YOLO |
| Faster R-CNN R50 | Two-stage | Classic two-stage detector |
| Cascade R-CNN R101 | Two-stage | Multi-stage refinement |
| CenterNet | Anchor-free | Keypoint-based detection |
| RT-DETR | DETR-family | Real-time transformer |
| DDQ-DETR R50 | DETR-family | Dense query DETR |
| DINO 4-scale R50 | DETR-family | Improved DETR |
| RTMDet-M | One-stage | Real-time multi-task |

---

## 📁 Project Structure

```
SDE-DET/
├── SDE-DET/               # Main source code
├── docker/                # Docker configuration
├── example_image/         # Example images for demo
├── examples/              # Example scripts
├── heatmap.py             # Heatmap visualization
├── train1.py              # Training script
├── val.py                 # Validation script
├── best.pt                # Pre-trained model weights
├── yolov8n/   yolov8s/    # YOLO backbones
├── yolov9-c/  yolov10n/   yolov10s/
├── faster rcnn r50/       cascade-rcnn-r101/
├── centernet/  rt-detr/   rtmdet-m/
├── ddq-detr-r50/          dino-4scale-r50/
├── 消融实验（DA）/         # Ablation: Data Augmentation
├── 消融实验（starnet+DA）/  # Ablation: StarNet + DA
└── 热力图/                # Heatmap outputs
```

---

## ⚙️ Quickstart

### Training

```bash
python train1.py  # with your dataset config
```

### Validation

```bash
python val.py
```

### Heatmap Visualization

```bash
python heatmap.py
```

### Docker

```bash
# Use the configuration in docker/ for reproducible environments
```

---

## 📦 Resources

| Resource | Location |
|----------|----------|
| **Example images** | `example_image/` |
| **Model weights** | `best.pt` (in repo); larger checkpoints on [Hugging Face](https://huggingface.co/) — links to be added |

> Part of the model weights are too large for this repository and will be hosted on Hugging Face.

---

## 📚 Citation

If you use **SDE-DET** in your research, please cite:

```bibtex
@article{sdedet2026,
  title     = {SDE-DET},
  author    = {Yihao Hu and collaborators},
  year      = {2026},
  journal   = {Computers and Electronics in Agriculture},
  doi       = {10.1016/j.atech.2026.101915},
  url       = {https://github.com/yihaohu0118/SDE-DET}
}
```
