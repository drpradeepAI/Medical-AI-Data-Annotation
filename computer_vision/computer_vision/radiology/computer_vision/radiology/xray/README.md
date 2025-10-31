# 🩻 X-Ray Mass Lesion Detection Dataset  
**Medical AI Data Annotation Project**

This folder contains the **Chest X-Ray Mass Lesion Detection Dataset**, annotated and structured for multi-format interoperability.  
It is part of the broader *Medical-AI-Data-Annotation* repository for radiology-based computer vision research.

---

## 📘 Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Objective:** Detection of **mass lesions**, including tumors, nodules, and opacities.  
- **Annotation Type:** Bounding Boxes  
- **Annotation Count:** 50 chest X-ray images annotated  
- **Annotation Tool:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Export Formats:** COCO, CSV, Pascal VOC, and YOLO  
- **Primary Task:** Object Detection (localization of lung mass lesions)  

This dataset serves as a high-quality, small-scale reference for medical AI model development, benchmarking, and educational purposes.

---

## 📁 Folder Structure
xray/
├── annotated_data/ # Bounding box annotations in 4 formats (COCO, CSV, VOC, YOLO)
│ ├── COCO/
│ ├── CSV/
│ ├── VOC/
│ └── YOLO/
│
├── raw_data/ # Original 50 chest X-ray images (unannotated)
│ └── 50_chest_xrays_raw_data_in_jpg/
│
├── metadata/ # Reserved for dataset descriptors and mapping files
│ └── .keep
│
├── screenshot/ # Project visual documentation (PDFs and PNGs)
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
| 0 | `mass_lesion` | Visible lung mass, tumor, or opacity in chest X-ray |

All annotation formats (COCO, CSV, VOC, YOLO) share this unified label schema.

---

## ⚙️ Dataset Workflow Summary

| Stage | Description |
|--------|-------------|
| **1. Raw Data Preparation** | 50 X-ray images curated for clear lung mass visualization. |
| **2. Manual Annotation (CVAT)** | Bounding boxes drawn around mass lesions using the CVAT web tool. |
| **3. Multi-format Export** | Annotations exported into COCO, CSV, VOC, and YOLO formats for flexibility. |
| **4. Documentation & QA** | Each stage documented via screenshots and PDF reports. |
| **5. Integration-Ready Output** | Structured dataset with placeholders for metadata and versioning. |

---

## 🧠 Applications

- AI model training for lung mass/nodule detection.  
- Educational demonstration of medical image annotation workflows.  
- Benchmarking across multiple annotation formats.  
- Conversion or dataset standardization tutorials.  

---

## 🧰 Recommended Tools

| Task | Suggested Tools |
|------|------------------|
| Annotation | CVAT, LabelImg, Roboflow |
| Visualization | FiftyOne, OpenCV, matplotlib |
| Conversion | CVAT Export Converter, Roboflow |
| Model Training | YOLOv8, Detectron2, TensorFlow Object Detection API |
| Validation | PyCOCOTools, XML parsers, pandas |

---

## 🔗 Cross-References

| Folder | Description |
|---------|-------------|
| [`raw_data/`](./raw_data) | Contains unannotated chest X-rays used for annotation. |
| [`annotated_data/`](./annotated_data) | Bounding box annotations in multiple formats. |
| [`metadata/`](./metadata) | Reserved for dataset descriptors and mappings. |
| [`screenshot/`](./screenshot) | Contains PDFs and screenshots documenting annotation stages. |

---

## 📸 Screenshot Previews

Visual references of the annotation process are available in:
- `01_project_overview.pdf`
- `02_raw_data_preannotation_preview.pdf`
- `03_annotated_sample_data.pdf`
- `04_export_settings_and_data.pdf`

They demonstrate dataset creation stages, from raw data setup to annotation export.

---

## 📜 License & Usage

This dataset and its derivatives are released for **research, educational, and non-commercial use** only.  
Users must comply with medical data ethics, privacy, and institutional review standards.

---

## 🔖 Citation (Suggested)

If you use this dataset or its structure in your work, please cite:
Dr. Pradeep AI, Medical-AI-Data-Annotation: X-Ray Mass Lesion Detection Dataset, 2025.
Available at: https://github.com/drpradeepAI/Medical-AI-Data-Annotation

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| 1.0 | 2025-10 | Initial release of 50 annotated chest X-rays with COCO, CSV, VOC, and YOLO formats. |
