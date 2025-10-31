# 🩻 X-Ray Mass Lesion Detection Dataset  
**Medical AI Data Annotation Project**

This folder contains the **Chest X-Ray Mass Lesion Detection Dataset**, annotated and organized for **multi-format interoperability**.  
It is part of the larger *Medical-AI-Data-Annotation* repository focused on radiology-based computer vision research and AI model development.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Modality** | Chest X-Ray (Radiography) |
| **Objective** | Detection of **mass lesions** such as lung tumors, nodules, or dense opacities |
| **Annotation Type** | Bounding Boxes |
| **Dataset Size** | 50 X-ray images |
| **Annotation Tool** | [CVAT – Computer Vision Annotation Tool](https://cvat.org/) |
| **Export Formats** | COCO, CSV, Pascal VOC (XML), and YOLO |
| **Primary Task** | Object Detection – localizing visible lung mass lesions |

This dataset provides a high-quality reference for **medical AI development**, **educational visualization**, and **cross-format benchmarking**.

---

## 📁 Folder Structure

50_chest_xray_mass_annotation_project/
├── annotated_data/ # Bounding box annotations in 4 formats (COCO, CSV, VOC, YOLO)
│ ├── COCO/
│ ├── CSV/
│ ├── VOC/
│ └── YOLO/
│
├── raw_data/ # Original 50 unannotated chest X-ray images
│ └── 50_chest_xrays_raw_data_in_jpg/
│
├── metadata/ # Dataset descriptors and mapping files (placeholders)
│ └── .keep
│
├── screenshot/ # Visual documentation of annotation stages
│ ├── screenshots_png_images/
│ ├── 01_project_overview.pdf
│ ├── 02_raw_data_preannotation_preview.pdf
│ ├── 03_annotated_sample_data.pdf
│ └── 04_export_settings_and_data.pdf
│
└── README.md # Current documentation file

---

## 🧩 Annotation Schema

| Class ID | Label | Description |
|-----------|--------|-------------|
| 0 | `mass_lesion` | Visible lung mass, tumor, or dense opacity identified on the chest X-ray |

All formats (COCO, CSV, VOC, YOLO) follow this **single unified label schema** for interoperability.

---

## ⚙️ Dataset Workflow Summary

| Stage | Description |
|--------|-------------|
| **1. Raw Data Preparation** | Selection of 50 chest X-ray images with clearly visible lung masses or opacities. |
| **2. Annotation (CVAT)** | Manual bounding box annotation around mass lesions using CVAT web interface. |
| **3. Multi-format Export** | Dataset exported into COCO, CSV, Pascal VOC, and YOLO for cross-framework use. |
| **4. Documentation & QA** | Visual verification and report generation (PDF and screenshots). |
| **5. Integration-Ready Dataset** | Folder structured for training pipelines and format conversions. |

---

## 🧠 Applications

- Training and validating object detection models (YOLOv8, Detectron2, TensorFlow OD API).  
- Benchmarking cross-format annotation consistency.  
- Teaching medical image annotation methods.  
- Demonstrating clinical dataset structuring best practices.

---

## 🧰 Recommended Tools

| Purpose | Suggested Tools |
|----------|------------------|
| Annotation | CVAT, LabelImg, Roboflow |
| Visualization | FiftyOne, OpenCV, matplotlib |
| Conversion | CVAT Export Converter, Roboflow |
| Model Training | YOLOv8, Detectron2, TensorFlow OD API |
| Validation | PyCOCOTools, XML/CSV parsers, pandas |

---

## 🔗 Cross-References

| Folder | Description |
|---------|-------------|
| [`raw_data/`](./raw_data) | Source chest X-ray images used for annotation. |
| [`annotated_data/`](./annotated_data) | Bounding box annotations in COCO, CSV, VOC, and YOLO formats. |
| [`metadata/`](./metadata) | Contains mapping and descriptor placeholders. |
| [`screenshot/`](./screenshot) | Visual reports documenting annotation workflow. |

---

## 📸 Screenshot Previews

Annotation stages are illustrated in:
- `01_project_overview.pdf`  
- `02_raw_data_preannotation_preview.pdf`  
- `03_annotated_sample_data.pdf`  
- `04_export_settings_and_data.pdf`

These demonstrate dataset evolution from **raw input** to **export-ready annotation**.

---

## 📜 License & Usage

This dataset is provided under the **Research, Educational, and Non-Commercial Use License**.  
Users must ensure compliance with ethical, institutional, and privacy regulations for medical data.

---

## 🔖 Citation (Suggested)

> **Dr. Pradeep AI**  
> *Medical-AI-Data-Annotation: X-Ray Mass Lesion Detection Dataset* (Version 1.0, October 2025)  
> GitHub Repository: [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Update Description |
|----------|------|--------------------|
| **1.0** | 2025-10 | Initial release of 50 annotated chest X-rays (COCO, CSV, VOC, YOLO) |
| **1.1 (Planned)** | 2026-Q1 | Addition of mask-level segmentation and expanded metadata |
