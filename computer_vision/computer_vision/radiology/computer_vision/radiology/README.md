# 🩺 Radiology Datasets Collection  
**Medical-AI-Data-Annotation: Radiology Division**

This directory hosts a suite of curated and annotated **radiology imaging datasets**, including **CT Scans**, **MRI**, and **X-Ray** projects.  
Each dataset is carefully structured, annotated, and documented to support the development of **AI models in medical imaging**, particularly for **lesion detection, segmentation, and diagnosis assistance**.

---

## 🧠 Overview

| Modality | Primary Task | Annotation Type | Total Samples | Export Formats | Status |
|-----------|---------------|----------------|----------------|----------------|---------|
| **CT Scans** | Brain Tumor Segmentation | Segmentation Masks | 50 | CVAT XML, PNG | ✅ Completed |
| **MRI** | Brain Tumor Segmentation | Bounding Box + Mask | 50 | COCO, YOLO, CVAT XML, Segmentation | ✅ Completed |
| **X-Ray** | Chest Mass Lesion Detection | Bounding Box | 50 | COCO, CSV, Pascal VOC, YOLO | ✅ Completed |

All datasets follow a **consistent hierarchy** for raw data, annotations, screenshots, and metadata — ensuring easy reproducibility, conversion, and analysis across modalities.

---

## 📁 Folder Structure
radiology/
├── ct_scans/ # Brain tumor segmentation dataset (CT modality)
│ ├── raw_data/
│ ├── annotated_data/
│ ├── metadata/
│ └── screenshots/
│
├── mri/ # Brain tumor annotation dataset (MRI modality)
│ ├── raw_data/
│ ├── annotated_data/
│ ├── metadata/
│ └── screenshots/
│
├── xray/ # Chest X-ray mass lesion detection dataset
│ ├── raw_data/
│ ├── annotated_data/
│ ├── metadata/
│ └── screenshot/
│
└── README.md # Current master file (you are here)

---

## 🧩 Common Features Across All Datasets

- 📸 **Raw Data:** Clean, de-identified medical images in standard formats (JPG/PNG).  
- 🎯 **Annotations:** Bounding boxes, segmentation masks, or polygon regions—depending on modality.  
- 💾 **Multi-format Compatibility:** Exports available in COCO, CSV, YOLO, Pascal VOC, and CVAT XML.  
- 🧾 **Documentation:** Every project contains screenshots, PDFs, and structured READMEs explaining workflow.  
- 🔁 **Consistency:** Unified folder naming, metadata placeholders, and version control for all datasets.  
- 🧠 **Educational Focus:** Designed for learning annotation standards, dataset structuring, and AI training readiness.

---

## 🧬 Purpose and Design Philosophy

This radiology suite was developed to:
1. **Demonstrate a full medical data annotation pipeline** using open tools like CVAT.  
2. **Standardize datasets** for AI training and interoperability across frameworks.  
3. **Enable transparency** in dataset creation, labeling, and export format management.  
4. **Encourage open learning** for developers and researchers in medical computer vision.

---

## 🔧 Tools & Technologies

| Function | Tools Used |
|-----------|-------------|
| **Annotation** | [CVAT](https://cvat.org/), LabelImg |
| **Image Format Handling** | OpenCV, Pillow |
| **Data Conversion** | CVAT Exporter, custom scripts |
| **Documentation** | Markdown, screenshots, PDF exports |
| **Version Control** | GitHub (modular commit tracking for each dataset) |

---

## 🧠 Use Cases

- Developing computer vision AI models for medical image analysis.  
- Benchmarking multi-format annotation exports.  
- Medical dataset versioning and documentation demonstration.  
- Teaching structured dataset management for research labs.  

---

## 🔗 Quick Access to Subprojects

| Folder | Description |
|---------|--------------|
| [`ct_scans/`](./ct_scans) | CT Brain Tumor Segmentation Dataset |
| [`mri/`](./mri) | MRI Brain Tumor Annotation Dataset (bounding boxes + segmentation) |
| [`xray/`](./xray) | Chest X-Ray Mass Lesion Detection Dataset |

---

## 🧮 Data Schema Alignment

All datasets align with a unified labeling structure and documentation format:
{modality}/
├── raw_data/
├── annotated_data/
│ ├── COCO/
│ ├── CSV/ (if applicable)
│ ├── VOC/
│ ├── YOLO/
│ ├── segmentation_mask/ (for CT/MRI)
│ └── cvat_xml/
├── metadata/
└── screenshots/

---

## 🗂️ Planned Future Additions

- **Ultrasound Datasets** (Lesion Classification, Doppler Flow Analysis)  
- **PET Scans** (Tumor metabolic mapping annotations)  
- **Mammography Datasets** (Microcalcification and mass detection)  
- **Multimodal Fusion Datasets** (Integration of MRI, CT, and PET for hybrid AI training)

---

## 📜 License

These datasets are released for **educational and research purposes**.  
Redistribution or commercial use requires adherence to medical data ethics and institutional policies.  

---

## 🧾 Citation

If this collection is used in publications or research projects, please cite:
Dr. Pradeep AI, Medical-AI-Data-Annotation: Radiology Datasets Collection (CT, MRI, X-Ray), 2025.
Available at: https://github.com/drpradeepAI/Medical-AI-Data-Annotation
