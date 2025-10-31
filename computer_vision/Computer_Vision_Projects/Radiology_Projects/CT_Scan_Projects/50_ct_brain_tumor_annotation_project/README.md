# 🧠 CT Scan Annotation Dataset – Medical AI (Brain Tumor Segmentation)

This folder contains a **curated medical imaging dataset** for **CT scan–based brain tumor segmentation and annotation**.  
It is part of the larger **Medical AI Data Annotation** repository focused on developing structured, high-quality datasets for training and validating deep-learning models in medical imaging.

---

## 📘 Overview
This dataset module demonstrates an end-to-end medical annotation workflow covering:
- **Raw CT brain images**
- **Multiple annotation export formats (COCO, YOLO, CVAT XML, Segmentation Masks)**
- **Supporting documentation and screenshots**
- **Metadata describing dataset organization and specifications**

It is designed to showcase **data quality, reproducibility, and transparency** for AI-driven medical research.

---

## 🧩 Folder Structure

ct_scans/
├── raw_data/ # Original 50 CT brain images in PNG format
├── annotated_data/ # Labeled data in four export formats (COCO, YOLO, CVAT_XML, Segmentation Masks)
│ ├── COCO/
│ ├── YOLO/
│ ├── cvat_xml/
│ └── segmentation_masks/
├── metadata/ # Dataset metadata and project versioning info
├── screenshots/ # PDF + PNG visual documentation of the entire annotation workflow
└── README.md # Current file (project overview)

---

## 🧬 Dataset Summary

| Property | Description |
|-----------|-------------|
| **Project Name** | CT Brain Tumor Segmentation |
| **Modality** | CT Scan |
| **Number of Images** | 50 |
| **Annotation Formats** | COCO (.json), YOLO (.txt), CVAT (.xml), Segmentation Masks (.png) |
| **Segmentation Classes** | Tumor, Background |
| **Resolution** | 512 × 512 pixels |
| **Annotation Tool** | CVAT 1.1 |
| **Annotation Type** | Polygonal + Pixel-wise |
| **Color Mode** | Grayscale |
| **Dataset Version** | v1.0 |
| **License** | Research & Non-commercial educational use |
| **Author** | Dr. Pradeep AI |

---

## 📂 Subfolders Explained

### 1. `raw_data/`
Contains the **original 50 CT brain images** used for segmentation and labeling.  
Both the uncompressed image folder and the zipped collection are available for convenience.

### 2. `annotated_data/`
Includes four industry-standard export formats:
- **COCO (.json):** Standard object detection/segmentation structure  
- **YOLO (.txt):** Lightweight bounding-box and mask coordinates per image  
- **CVAT XML:** Compatible with CVAT re-imports or other XML-based pipelines  
- **Segmentation Masks:** Pixel-wise labeled masks for tumor region classification  

Each format has its own folder with documentation and `.keep` files to maintain structure.

### 3. `metadata/`
Provides dataset summary information (image counts, formats, labels, and version details).  
Acts as a **dataset descriptor** for researchers and clients to understand structure at a glance.

### 4. `screenshots/`
Holds **visual documentation** of the annotation pipeline — project setup, labeling interface, and export settings — as both **PNG images** and **PDF summaries**.

---

## 🧠 Use Cases
This dataset is ideal for:
- Demonstrating **medical imaging annotation workflows**
- Benchmarking segmentation models (U-Net, Mask R-CNN, DeepLab)
- Creating tutorials for **CVAT and AI dataset preparation**
- Serving as a **portfolio project** for computer-vision freelancing in healthcare AI

---

## 🧾 Citation
If you refer to or reuse this dataset in research or training, please credit:

> **Dr. Pradeep AI – Medical AI Data Annotation (CT Scan Module)**  
> GitHub: [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧩 Future Additions
- Add `metadata.csv` and `metadata.json` for automated dataset parsing  
- Introduce new annotation samples (lung CT, chest CT, abdominal scans)  
- Include preprocessing scripts for normalization and mask generation  

---

**Author:** Dr. Pradeep AI  
**Repository:** Medical-AI-Data-Annotation  
**Module:** Computer Vision → Radiology → CT Scans  
**Version:** 1.0 (October 2025)
