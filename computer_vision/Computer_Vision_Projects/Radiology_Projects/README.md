# 🩺 Radiology Datasets Collection  
**Medical-AI-Data-Annotation: Radiology Division**

This directory hosts the **complete suite of radiology imaging projects**, including **CT Scans**, **MRI**, and **X-Ray** datasets.  
Each project demonstrates structured medical image annotation workflows for **tumor detection, lesion segmentation, and diagnostic AI model training** — all following a unified organizational and documentation standard.

---

## 🧠 Overview

| Modality | Primary Task | Annotation Type | Sample Count | Export Formats | Status |
|-----------|---------------|----------------|---------------|----------------|---------|
| 💀 **CT Scans** | Brain Tumor Segmentation | Pixel-wise Mask | 50 | CVAT XML, PNG | ✅ Completed |
| 🧠 **MRI** | Brain Tumor Segmentation | Polygon + Mask | 50 | COCO, YOLO, CVAT XML, PNG | ✅ Completed |
| 🩻 **X-Ray** | Chest Mass Lesion Detection | Bounding Box | 50 | COCO, CSV, Pascal VOC, YOLO | ✅ Completed |

All datasets are **multi-format compatible**, **ethically structured**, and designed for easy plug-and-play integration with AI frameworks like **MONAI**, **YOLOv8**, and **Detectron2**.

---

## 📁 Folder Structure

Radiology_Projects/
├── CT_Scan_Projects/ # CT Brain Tumor Segmentation
│ └── 50_ct_brain_tumor_annotation_project/
│
├── MRI_Scan_Projects/ # MRI Brain Tumor Annotation
│ └── 50_mri_brain_tumor_annotation_project/
│
├── X-RAY_Projects/ # Chest X-Ray Mass Lesion Detection
│ └── 50_chest_xray_mass_annotation_project/
│
└── README.md # Current file (Radiology overview)

---

## 🧩 Core Features Across All Modalities

- 🧾 **Unified Folder Structure:** Consistent organization with `raw_data/`, `annotated_data/`, `metadata/`, and `screenshots/`.  
- 🎯 **Multi-format Exports:** COCO, YOLO, VOC, CSV, CVAT XML, and PNG masks supported.  
- 🧠 **Standardized Schema:** Common label definitions across modalities.  
- 📸 **Visual Documentation:** Each dataset includes PDF reports and screenshots showing annotation workflows.  
- 💡 **Reproducibility:** Version-controlled via GitHub for open, modular dataset development.  

---

## 🧬 Design Philosophy

The **Radiology Division** embodies three key goals:
1. **Demonstration:** End-to-end AI dataset preparation pipeline for medical imaging.  
2. **Standardization:** Unified structure across modalities for interoperability and conversion.  
3. **Education:** Enable learners, researchers, and engineers to understand and replicate medical AI workflows.

---

## 🧰 Tools & Technologies

| Function | Tools / Frameworks |
|-----------|--------------------|
| **Annotation** | [CVAT](https://cvat.org/), LabelImg, ITK-SNAP |
| **Visualization** | FiftyOne, OpenCV, MONAI Viewer |
| **Format Conversion** | CVAT Exporter, Roboflow, custom scripts |
| **Model Training** | YOLOv8, Detectron2, MONAI, U-Net |
| **Documentation** | Markdown, GitHub, PDF summaries |
| **Version Control** | GitHub commit-based modular tracking |

---

## 🔗 Quick Access to Subprojects

| Folder | Description |
|---------|--------------|
| 💀 [`CT_Scan_Projects/`](./CT_Scan_Projects) | CT Brain Tumor Segmentation Dataset |
| 🧠 [`MRI_Scan_Projects/`](./MRI_Scan_Projects) | MRI Brain Tumor Annotation Dataset |
| 🩻 [`X-RAY_Projects/`](./X-RAY_Projects) | Chest X-Ray Mass Lesion Detection Dataset |

---

## 🧮 Cross-Modality Schema Alignment

All datasets maintain a **common directory logic** for ease of automation and metadata parsing.

{modality}_Projects/
└── {dataset_name}/
├── raw_data/
├── annotated_data/
│ ├── COCO/
│ ├── YOLO/
│ ├── VOC/
│ ├── segmentation_masks/
│ └── cvat_xml/
├── metadata/
├── screenshots/
└── README.md

This structure ensures interoperability and straightforward integration with deep learning pipelines or dataset loaders.

---

## 🧠 Use Cases

- Building AI models for **tumor/lesion segmentation and detection**  
- Benchmarking multi-format annotation exports  
- Educational demonstration of dataset curation pipelines  
- Radiology AI workflow automation and documentation templates  

---

## 🚀 Planned Expansions

| Future Dataset | Task | Status |
|----------------|------|--------|
| 🩸 **Ultrasound (USG)** | Lesion classification and Doppler analysis | 🔄 In Design |
| 🔥 **PET Scans** | Tumor metabolic mapping | 🧩 Planned |
| 🎀 **Mammography** | Microcalcification and mass detection | 🧩 Planned |
| 🧬 **Multimodal Fusion** | MRI + CT + PET hybrid AI dataset | 🧠 Concept Stage |

---

## 📜 License

All radiology datasets are provided for **non-commercial research and education**.  
Users must comply with institutional ethics, patient privacy, and open-data usage standards.

---

## 🧾 Citation

If you use this repository or its structure in your research or projects, please cite:

> **Dr. Pradeep AI**  
> *Medical-AI-Data-Annotation: Radiology Datasets Collection (CT, MRI, X-Ray)*, 2025.  
> GitHub: [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| **1.0** | 2025-10 | Added CT, MRI, and X-Ray dataset divisions with complete documentation |
| **1.1 (Planned)** | 2026-Q1 | Add ultrasound and multimodal datasets |
