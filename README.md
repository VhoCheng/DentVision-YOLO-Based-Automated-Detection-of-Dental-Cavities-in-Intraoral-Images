# DentVision
## YOLO-Based Automated Detection of Dental Cavities in Intraoral Images

DentVision is a deep learning framework for **automated detection of dental cavities in intraoral images** using YOLO-based object detection models.

This project explores the application of modern object detection algorithms for **computer-aided dental diagnosis**, providing a comparative evaluation of multiple YOLO architectures.

---

# Project Overview

Dental caries remain one of the most prevalent oral diseases worldwide. Early detection is essential for effective treatment and prevention. However, manual diagnosis from intraoral images is time-consuming and highly dependent on clinical expertise.

DentVision aims to develop an **AI-assisted cavity detection system** that can automatically identify suspicious caries regions from dental photographs.

---

# Model Architecture

This project evaluates three YOLO-based object detection models:

| Model | Type |
|------|------|
| YOLOv5s | Baseline detector |
| YOLOv8n | Lightweight improved detector |
| YOLOv8s | Enhanced detection performance |

All models were trained with identical dataset splits and experimental settings.

---

# Dataset

The dataset contains **intraoral dental images** annotated with bounding boxes.

Classes:

- cavity
- normal

Dataset configuration:

```yaml
train: train/images
val: valid/images
test: test/images

nc: 2
names: ['cavity','normal']
