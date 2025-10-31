# 💀 CT Scan Projects  
**Medical AI Data Annotation – Radiology Division**

This directory contains all **CT scan–based medical imaging projects** developed under the *Medical-AI-Data-Annotation* repository.  
Each project focuses on **tumor segmentation, detection, and classification** from computed tomography (CT) scans to enable AI-powered radiological analysis and clinical model training.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Imaging Modality** | CT (Computed Tomography) |
| **Focus Area** | Brain and other anatomical regions (future expansion) |
| **Annotation Types** | Polygonal, Pixel-wise segmentation, Bounding boxes |
| **Annotation Tools** | [CVAT](https://cvat.org/), ITK-SNAP, 3D Slicer |
| **Export Formats** | COCO, YOLO, CVAT XML, PNG Masks |
| **Applications** | Tumor detection, segmentation, radiomics, and deep-learning model development |

This folder provides **structured, interoperable datasets** for building and benchmarking computer vision models in medical AI research.

---

## 📁 Folder Structure

CT_Scan_Projects/
├── 50_ct_brain_tumor_annotation_project/ # Segmentation dataset of 50 CT brain images
│ ├── annotated_data/
│ ├── metadata/
│ ├── raw_data/
│ ├── screenshots/
│ └── README.md
│
└── README.md # Current documentation file (you are here)

---

## 🧩 Current Project

### 🧠 [`50_ct_brain_tumor_annotation_project`](./50_ct_brain_tumor_annotation_project)
A curated dataset of **50 CT brain images**, manually annotated for **tumor segmentation**.  
Includes multiple export formats (COCO, YOLO, CVAT XML, PNG masks) and fully documented workflows with visual references.

**Highlights:**
- Manual annotations for brain tumor regions using CVAT  
- 512×512 standardized resolution for AI model readiness  
- Segmentation masks for semantic and instance-level use  
- Ideal for MONAI, U-Net, and Mask R-CNN training pipelines  

---

## 🔬 Planned Additions

| Project | Description | Status |
|----------|-------------|--------|
| `50_ct_brain_tumor_annotation_project` | Brain tumor segmentation dataset | ✅ Completed |
| `100_ct_multiregion_annotation_project` | Multi-organ CT segmentation (lungs, abdomen, skull) | 🧩 Planned |
| `ct_detection_project` | Bounding-box based lesion detection dataset | 🧩 In development |

---

## 🧠 Applications

- CT-based tumor and lesion segmentation model development  
- Cross-format annotation experiments for model interoperability  
- Educational demonstrations of AI dataset creation workflows  
- Benchmarking computer vision models for medical imaging  

---

## 🧰 Recommended Tools

| Task | Tools |
|------|--------|
| Annotation | CVAT, ITK-SNAP, 3D Slicer |
| Visualization | SimpleITK, matplotlib, OpenCV |
| Model Training | MONAI, PyTorch Lightning, U-Net, Detectron2 |
| Conversion | CVAT Export Converter, Roboflow |
| Evaluation | Dice, IoU, Hausdorff Distance |

---

## 🧩 Integration with Other Modalities

This folder belongs to the **Radiology Projects** suite, alongside:
- 🩻 [`X-RAY_Projects`](../X-RAY_Projects/) – Detection datasets for chest and skeletal pathologies  
- 🧠 [`MRI_Scan_Projects`](../MRI_Scan_Projects/) – Segmentation datasets for brain tumor analysis  

Together, these form a **multimodal foundation** for developing unified AI models across radiological imaging.

---

## 📜 License & Citation

All CT scan datasets are released for **research and educational purposes** only.  
Users must comply with ethical and institutional data use policies.

> **Citation (Suggested):**  
> Dr. Pradeep AI, *Medical-AI-Data-Annotation: CT Scan Projects Collection*, 2025.  
> [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| **1.0** | 2025-10 | Added `50_ct_brain_tumor_annotation_project` with segmentation data |
| **1.1 (Planned)** | 2026-Q1 | Expand to multi-region and detection-based CT datasets |
