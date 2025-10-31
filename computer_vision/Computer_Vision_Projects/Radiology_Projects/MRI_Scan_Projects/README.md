# 🧠 MRI Scan Projects  
**Medical AI Data Annotation – Radiology Division**

This directory contains all **MRI-based medical imaging projects** under the *Medical-AI-Data-Annotation* repository.  
Each project focuses on **segmentation, detection, and classification** of brain abnormalities to advance AI-based radiology research and education.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Imaging Modality** | MRI (Magnetic Resonance Imaging) |
| **Focus Area** | Brain imaging and tumor detection |
| **Annotation Types** | Segmentation masks, bounding boxes, metadata descriptors |
| **Annotation Tools** | [CVAT](https://cvat.org/), ITK-SNAP, 3D Slicer |
| **Export Formats** | CVAT XML, PNG Masks, COCO, YOLO (planned) |
| **Applications** | Medical AI model training, segmentation benchmarking, and clinical data education |

The datasets here are curated and structured for **multi-format interoperability** and are ready for training, benchmarking, and deployment across major AI frameworks.

---

## 📁 Folder Structure

MRI_Scan_Projects/
├── 50_mri_brain_tumor_annotation_project/ # Brain tumor segmentation dataset (50 scans)
│ ├── annotated_data/
│ ├── metadata/
│ ├── raw_data/
│ ├── screenshots/
│ └── README.md
│
└── README.md # Current documentation file (you are here)

---

## 🧩 Current Project

### [`50_mri_brain_tumor_annotation_project`](./50_mri_brain_tumor_annotation_project)
A curated dataset of **50 MRI brain scans**, annotated for **tumor segmentation** using CVAT.  
Annotations are exported as pixel-level segmentation masks (CLASS-wise and OBJECT-wise), along with CVAT XML files and visual documentation.

**Highlights:**
- Manual annotations using polygon and brush tools in CVAT  
- Structured for both **semantic** and **instance segmentation**  
- Integration-ready for U-Net, MONAI, and nnU-Net frameworks  
- Includes QA-reviewed mask exports and documentation reports  

---

## 🔬 Planned Additions

| Project | Description | Status |
|----------|-------------|--------|
| `50_mri_brain_tumor_annotation_project` | Brain tumor segmentation dataset | ✅ Completed |
| `100_mri_multilabel_project` | Multi-region segmentation (tumor, edema, ventricles, skull) | 🧩 In Progress |
| `mri_detection_project` | Bounding-box based MRI anomaly detection dataset | 🧩 Planned |

---

## 🧠 Applications

- Brain tumor detection, segmentation, and region analysis  
- Deep learning model training and benchmarking  
- Dataset format conversion studies  
- Radiology AI workflow demonstrations  
- Multi-modality AI education across MRI, CT, and X-Ray  

---

## 🧰 Recommended Tools

| Task | Suggested Tools |
|------|------------------|
| Annotation | CVAT, ITK-SNAP, 3D Slicer |
| Visualization | MONAI Viewer, SimpleITK, matplotlib |
| Model Training | MONAI, U-Net, nnU-Net, Detectron2 |
| Conversion | CVAT Exporter, Roboflow |
| Evaluation | Dice, IoU, Hausdorff Distance |

---

## 🧩 Integration with Other Modalities

This folder is part of the **Radiology Projects** suite, which also includes:  
- 🩻 [`X-RAY_Projects`](../X-RAY_Projects/) – Detection datasets for chest pathologies  
- 💀 [`CT_Scan_Projects`](../CT_Scan_Projects/) – CT-based tumor segmentation and detection datasets  

Together, these modalities enable **multimodal medical AI development** across 2D and 3D imaging domains.

---

## 📜 License & Citation

All MRI datasets are released for **research and educational use** only.  
Users must comply with ethical, privacy, and institutional medical data handling policies.

> **Citation (Suggested):**  
> Dr. Pradeep AI, *Medical-AI-Data-Annotation: MRI Scan Projects Collection*, 2025.  
> [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Notes |
|----------|------|-------|
| **1.0** | 2025-10 | Added `50_mri_brain_tumor_annotation_project` with complete segmentation dataset |
| **1.1 (Planned)** | 2026-Q1 | Add multi-label and detection MRI projects |
