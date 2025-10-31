# 👁️ Computer Vision Projects  
**Medical-AI-Data-Annotation Repository (Medical Imaging Division)**

This directory contains all **medical computer vision–based data annotation projects** developed under the *Medical-AI-Data-Annotation* repository.  
It focuses exclusively on **clinical and biomedical imaging domains** such as **Radiology, Pathology, Ophthalmology, Dermatology, and Endoscopy**, following a unified and reproducible annotation framework.

---

## 🧠 Overview

| Medical Domain | Example Projects | Primary Tasks | Status |
|----------------|------------------|----------------|---------|
| 🩻 **Radiology** | CT, MRI, X-Ray | Tumor & lesion detection, segmentation | ✅ Active |
| 🔬 **Pathology** | Microscopy & histopathology | Tissue region labeling, cellular segmentation | 🧩 Planned |
| 👁️ **Ophthalmology** | Fundus & OCT | Retinopathy, glaucoma, and macular segmentation | 🧩 Planned |
| 🩹 **Dermatology** | Skin lesion datasets | Lesion classification, boundary segmentation | 🧩 Planned |
| 🩺 **Endoscopy** | GI tract imaging | Polyp detection & mucosal segmentation | 🧠 Concept Stage |

All medical imaging projects here are curated for **AI model development**, **educational use**, and **research benchmarking** — compliant with medical ethics and standard annotation conventions.

---

## 📁 Folder Structure

Computer_Vision_Projects/
├── Radiology_Projects/ # CT, MRI, and X-Ray datasets (active)
│ ├── CT_Scan_Projects/
│ ├── MRI_Scan_Projects/
│ └── X-RAY_Projects/
│
├── Pathology_Projects/ # Microscopy & histopathology image datasets (planned)
│
├── Ophthalmology_Projects/ # Fundus & OCT eye datasets (planned)
│
├── Dermatology_Projects/ # Skin lesion datasets (planned)
│
├── Endoscopy_Projects/ # Gastrointestinal imaging datasets (concept stage)
│
└── README.md # This overview file

---

## 🩺 Active Division

### [`Radiology_Projects`](./Radiology_Projects)
Contains **CT, MRI, and X-Ray datasets** annotated for segmentation, detection, and classification tasks.  
Each subproject includes raw medical scans, annotated data (multi-format), metadata, and visual workflow documentation.

**Current Projects:**
- 💀 CT Brain Tumor Segmentation  
- 🧠 MRI Brain Tumor Segmentation  
- 🩻 Chest X-Ray Mass Lesion Detection  

➡️ [Explore Radiology Projects →](./Radiology_Projects)

---

## ⚙️ Annotation Standards

| Component | Description |
|------------|--------------|
| **Annotation Tools** | [CVAT](https://cvat.org/), Label Studio, ITK-SNAP, QuPath |
| **Supported Formats** | COCO, YOLO, Pascal VOC, CVAT XML, PNG Masks, CSV |
| **Annotation Types** | Bounding Boxes, Polygonal Regions, Pixel Masks |
| **Schema Policy** | Unified label schema across all medical imaging modalities |
| **Documentation** | Every dataset includes README, screenshots, and PDF workflow summaries |

All annotations are **manually verified** for consistency and precision, ensuring dataset integrity suitable for medical AI applications.

---

## 🧬 Unified Dataset Structure

Each medical dataset follows a standardized hierarchy:

{Project_Name}/
├── raw_data/ # Original de-identified medical images
├── annotated_data/ # Multi-format labeled outputs (COCO, YOLO, XML, Masks)
├── metadata/ # Schema, mapping files, and dataset logs
├── screenshots/ # Visual documentation and workflow evidence
└── README.md # Dataset overview

This consistency ensures smooth integration with **MONAI**, **Detectron2**, **YOLOv8**, and other medical AI frameworks.

---

## 🧰 Recommended Tools & Frameworks

| Function | Tools |
|-----------|--------|
| Annotation | CVAT, Label Studio, ITK-SNAP, QuPath |
| Visualization | MONAI Viewer, FiftyOne, OpenCV, matplotlib |
| Training | MONAI, PyTorch Lightning, Detectron2, TensorFlow |
| Evaluation | Dice, IoU, Hausdorff Distance, Precision/Recall |
| Documentation | Markdown, GitHub, PDF reports |

---

## 🧠 Vision & Design Philosophy

1. **Medical Exclusivity:** Focus solely on clinical and diagnostic imaging datasets.  
2. **Standardization:** Uniform folder, schema, and export logic across all medical domains.  
3. **Transparency:** Include documentation at every project stage (raw → annotated → exported).  
4. **Research Readiness:** Ensure compatibility with open-source AI frameworks and hospital R&D settings.  
5. **Expandability:** Scalable to all major medical imaging fields without structural change.

---

## 🧩 Upcoming Additions

| Division | Planned Projects | Description | Status |
|-----------|------------------|-------------|---------|
| 🔬 Pathology | Histopathology Slide Annotation | Tumor/tissue region labeling | 🧩 Planned |
| 👁️ Ophthalmology | Fundus & OCT datasets | Retinopathy & macular segmentation | 🔄 In Design |
| 🩹 Dermatology | ISIC-style lesion datasets | Lesion detection & classification | 🧠 Concept Stage |
| 🩺 Endoscopy | Polyp detection datasets | GI tract imaging segmentation | 🧩 Planned |

---

## 📜 License

All datasets under this directory are released for **non-commercial research and educational use** only.  
Users must adhere to ethical standards and data privacy regulations relevant to medical imaging.

---

## 🧾 Citation

If you use these datasets or their structure, please cite:

> **Dr. Pradeep AI**, *Medical-AI-Data-Annotation: Computer Vision Projects (Medical Imaging Division)*, 2025.  
> [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| **1.0** | 2025-10 | Added Radiology Division (CT, MRI, X-Ray Projects) |
| **1.1 (Planned)** | 2026-Q1 | Add Pathology, Ophthalmology, and Dermatology divisions |
