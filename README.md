# SDE-DET

The source code for SDE-DET will be published when this paper is accepted. Please refer to subsequent updates.

## Paper

📄 **Paper:** [https://doi.org/10.1016/j.atech.2026.101915](https://doi.org/10.1016/j.atech.2026.101915)

## Project Overview

SDE-DET is an object detection framework that supports multiple detection backbones. The project provides training, validation, and visualization tools for detection tasks.

## Project Structure

```
SDE-DET/
├── SDE-DET/              # Main source code
├── docker/               # Docker configuration
├── example_image/        # Example images for demo
├── examples/             # Example scripts
├── heatmap.py            # Heatmap visualization
├── train1.py             # Training script
├── val.py                # Validation script
├── best.pt               # Pre-trained model weights
├── cascade-rcnn-r101/    # Cascade R-CNN ResNet-101 backbone
├── centernet/            # CenterNet
├── ddq-detr-r50/         # DDQ-DETR ResNet-50
├── dino-4scale-r50/      # DINO 4-scale ResNet-50
├── faster rcnn r50/      # Faster R-CNN ResNet-50
├── rt-detr/              # RT-DETR
├── rtmdet-m/             # RTMDet-M
├── yolov8n/              # YOLOv8 nano
├── yolov8s/              # YOLOv8 small
├── yolov10n/             # YOLOv10 nano
├── yolov10s/             # YOLOv10 small
├── yolov9-c/             # YOLOv9-C
├── 消融实验（DA）/        # Ablation: Data Augmentation
├── 消融实验（starnet+DA）/ # Ablation: StarNet + DA
└── 热力图/               # Heatmap outputs
```

## Supported Backbones

| Model | Description |
|-------|-------------|
| YOLOv8 / YOLOv10 | Lightweight real-time detectors |
| YOLOv9-C | High-performance YOLO variant |
| Faster R-CNN | Two-stage detector |
| Cascade R-CNN | Multi-stage refinement |
| CenterNet | Anchor-free detector |
| RT-DETR / DDQ-DETR / DINO | DETR-family transformers |
| RTMDet | Real-time multi-task detector |

## Usage

- **Training:** Run `train1.py` with your dataset configuration
- **Validation:** Run `val.py` for model evaluation
- **Heatmap:** Run `heatmap.py` for attention/activation visualization
- **Docker:** Use the configuration in `docker/` for reproducible environments

## Resources

- **Example images:** Available in `example_image/`
- **Model weights:** Part of the model weights are too large for this repository and will be hosted on [Hugging Face](https://huggingface.co/). Links will be added when available.
