# 🩻 X-Ray Projects  
**Medical AI Data Annotation – Radiology Division**

This directory hosts all **X-Ray–based computer vision projects** under the *Medical-AI-Data-Annotation* repository.  
Each project focuses on curating, annotating, and structuring medical imaging datasets for AI model development, educational use, and multi-format interoperability.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Imaging Modality** | X-Ray (Radiography) |
| **Focus Areas** | Detection and segmentation of visible thoracic pathologies |
| **Annotation Types** | Bounding Boxes, Segmentation Masks (future), and Metadata Mapping |
| **Annotation Tools** | [CVAT](https://cvat.org/), LabelImg, Label Studio |
| **Export Formats** | COCO, CSV, Pascal VOC, YOLO |
| **Applications** | Object detection, AI benchmarking, dataset standardization, medical education |

Each project folder below contains a structured dataset prepared for training and testing computer vision algorithms in radiology.

---

## 📁 Folder Structure

X-RAY_Projects/
├── 50_chest_xray_mass_annotation_project/ # Annotated dataset for lung mass lesion detection
│ ├── annotated_data/
│ ├── raw_data/
│ ├── metadata/
│ ├── screenshot/
│ └── README.md
│
└── README.md # Current documentation file (you are here)

---

## 🧠 Current Project

### 📦 [`50_chest_xray_mass_annotation_project`](./50_chest_xray_mass_annotation_project)
A curated dataset of 50 chest X-ray images annotated for **mass lesion detection** (tumors, nodules, opacities).  
Annotations are available in COCO, CSV, Pascal VOC, and YOLO formats for cross-framework experimentation.

**Highlights:**
- High-quality manual bounding box annotations using CVAT  
- Visual documentation and versioned metadata placeholders  
- Integration-ready for YOLOv8, Detectron2, TensorFlow OD API  
- Educational and research-friendly dataset organization  

---

## 🔬 Planned Additions

| Project | Description | Status |
|----------|-------------|--------|
| `50_chest_xray_mass_annotation_project` | Mass lesion detection dataset (50 images) | ✅ Completed |
| `100_chest_xray_multiclass_project` | Multi-class detection (mass, effusion, consolidation, pneumothorax) | 🧩 Planned |
| `xray_segmentation_project` | Mask-level segmentation of chest pathologies | 🧩 In progress |

---

## 🧰 Recommended Toolchain

| Task | Suggested Tools |
|------|------------------|
| Annotation | CVAT, LabelImg, Label Studio |
| Visualization | FiftyOne, OpenCV, matplotlib |
| Format Conversion | CVAT Export Converter, Roboflow |
| Model Training | YOLOv8, Detectron2, TensorFlow Object Detection API |
| Quality Assurance | PyCOCOTools, XML/CSV validators |

---

## 🧩 Integration with Other Modalities

This folder is part of the **Radiology Projects** division, which also includes:
- 🧠 [`MRI_Scan_Projects`](../MRI_Scan_Projects/) – Brain tumor segmentation and detection datasets  
- 💀 [`CT_Scan_Projects`](../CT_Scan_Projects/) – CT-based tumor segmentation and object-level labeling  

Together, these three modalities provide a unified foundation for multimodal radiology AI development.

---

## 📜 License & Citation

All X-Ray datasets are released for **research and educational purposes** only.  
Users must follow institutional, ethical, and privacy standards when using or redistributing these datasets.

> **Citation (Suggested):**  
> Dr. Pradeep AI, *Medical-AI-Data-Annotation: X-Ray Projects Collection*, 2025.  
> [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Notes |
|----------|------|-------|
| **1.0** | 2025-10 | Initial release with `50_chest_xray_mass_annotation_project` |
| **1.1 (Planned)** | 2026-Q1 | Add multi-class and segmentation datasets |
