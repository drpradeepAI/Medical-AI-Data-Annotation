# 💀 CT Brain Tumor Segmentation Dataset  
**Medical AI Data Annotation Project**

This folder contains the **CT Brain Tumor Segmentation Dataset**, featuring 50 curated CT brain scans annotated for tumor identification and segmentation.  
It is part of the *Medical-AI-Data-Annotation* repository — a comprehensive initiative to develop standardized, multi-format datasets for AI-driven medical imaging research and education.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Modality** | CT (Computed Tomography) |
| **Region of Interest** | Brain |
| **Primary Condition** | Brain Tumor |
| **Dataset Size** | 50 CT brain images |
| **Annotation Tool** | [CVAT – Computer Vision Annotation Tool](https://cvat.org/) |
| **Annotation Type** | Polygonal and Pixel-wise segmentation |
| **Export Formats** | COCO JSON, YOLO TXT, CVAT XML, PNG Masks |
| **Resolution** | 512 × 512 px |
| **Color Mode** | Grayscale |
| **Purpose** | Segmentation model training, evaluation, and education |

This dataset provides a fully-documented workflow from raw CT scans to AI-ready segmentation masks.

---

## 📁 Folder Structure

50_ct_brain_tumor_annotation_project/
├── raw_data/ # Original CT brain images
├── annotated_data/ # Multi-format annotations
│ ├── COCO/
│ ├── YOLO/
│ ├── cvat_xml/
│ └── segmentation_masks/
├── metadata/ # Dataset descriptors and version info
├── screenshots/ # Documentation (PDFs, PNGs)
└── README.md # Current file

---

## 🧩 Annotation Schema

| Class ID | Label | Description |
|-----------|--------|-------------|
| 0 | `background` | Non-tumor brain regions |
| 1 | `tumor` | Visible tumor or abnormal growth region |

All annotation formats (COCO, YOLO, CVAT XML, PNG) follow this **unified schema** for interoperability.

---

## ⚙️ Dataset Workflow Summary

| Step | Description |
|------|-------------|
| **1. Data Preparation** | 50 CT brain scans curated and preprocessed to 512×512 resolution. |
| **2. Annotation (CVAT)** | Manual segmentation performed with polygon and brush tools. |
| **3. Exporting Formats** | Dataset exported to COCO, YOLO, CVAT XML, and segmentation mask formats. |
| **4. Documentation** | Screenshots and PDFs captured for transparency and reproducibility. |
| **5. Metadata Structuring** | Folder-level and dataset-level metadata organized for version tracking. |

---

## 🧬 Dataset Summary

| Property | Details |
|-----------|----------|
| **Annotation Formats** | COCO (.json), YOLO (.txt), CVAT (.xml), Segmentation (.png) |
| **Segmentation Classes** | Tumor, Background |
| **Annotation Type** | Polygonal + Pixel-wise |
| **Annotation Tool Version** | CVAT 1.1 |
| **Dataset Version** | v1.0 |
| **License** | Research & Educational Use |
| **Author** | Dr. Pradeep AI |

---

## 📂 Subfolder Details

### 🧠 `raw_data/`
Contains the original 50 CT brain scans in `.png` format — unannotated and ready for labeling workflows.  
➡️ [View Raw Data](./raw_data)

---

### 🎯 `annotated_data/`
Includes all annotation formats for compatibility across frameworks:  
- **COCO JSON:** For PyTorch & Detectron2  
- **YOLO TXT:** For YOLOv5–YOLOv8 models  
- **CVAT XML:** Editable re-import format  
- **Segmentation Masks:** Pixel-wise tumor maps  

➡️ [View Annotated Data](./annotated_data)

---

### 🧾 `metadata/`
Holds structural descriptors, mappings, and dataset logs for transparency and reproducibility.  
➡️ [View Metadata](./metadata)

---

### 🖼️ `screenshots/`
Contains visual documentation of the annotation pipeline —  
project setup, labeling interface, exports, and quality control visuals (PDF + PNG).  
➡️ [View Screenshots](./screenshots)

---

## 🧠 Applications

- Training and benchmarking segmentation models (U-Net, DeepLab, Mask R-CNN).  
- Demonstrating CVAT annotation workflows in radiology.  
- Educational tutorials on dataset creation for healthcare AI.  
- Portfolio or client showcase for computer vision projects.  

---

## 🧰 Recommended Tools

| Task | Tools |
|------|--------|
| Annotation | CVAT, Label Studio |
| Visualization | FiftyOne, OpenCV, matplotlib |
| Model Training | MONAI, U-Net, Detectron2, TensorFlow OD API |
| Evaluation | Dice, IoU, Precision/Recall metrics |

---

## 🧩 Compatibility

| Framework | Supported Format | Folder |
|------------|------------------|--------|
| PyTorch / Detectron2 | COCO JSON | `annotated_data/COCO` |
| YOLOv5–YOLOv8 | YOLO TXT | `annotated_data/YOLO` |
| CVAT | XML | `annotated_data/cvat_xml` |
| MONAI / U-Net | Segmentation PNG | `annotated_data/segmentation_masks` |

---

## 📜 License & Usage

This dataset is licensed for **research and educational purposes only**.  
Users must comply with ethical guidelines, privacy regulations, and institutional review standards.

---

## 🔖 Citation (Suggested)

> **Dr. Pradeep AI**  
> *Medical-AI-Data-Annotation: CT Brain Tumor Segmentation Dataset*, 2025.  
> GitHub Repository: [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| **1.0** | 2025-10 | Initial release of 50 annotated CT brain images |
| **1.1 (Planned)** | 2026-Q1 | Add metadata.json and expanded annotation samples |
