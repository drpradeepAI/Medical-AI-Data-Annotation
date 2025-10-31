# 🧠 MRI Brain Tumor Segmentation Dataset  
**Medical AI Data Annotation Project**

This folder hosts the **MRI Brain Tumor Segmentation Dataset**, containing raw MRI scans, annotated segmentation masks, metadata placeholders, and project documentation.  
It demonstrates a complete medical imaging annotation pipeline built for AI research, model training, and education in radiology-based computer vision.

---

## 📘 Overview

| Attribute | Description |
|------------|--------------|
| **Modality** | MRI (Magnetic Resonance Imaging) |
| **Region of Interest** | Brain |
| **Primary Condition** | Brain Tumor (normal and abnormal cases included) |
| **Annotation Type** | Pixel-wise segmentation masks (CLASS & OBJECT level) |
| **Dataset Size** | 50 MRI images |
| **Annotation Tool** | [CVAT – Computer Vision Annotation Tool](https://cvat.org/) |
| **Export Formats** | CVAT XML, COCO JSON, YOLO TXT, Segmentation PNG |
| **Primary Task** | Tumor segmentation and boundary delineation |
| **Purpose** | Model development, benchmarking, and educational demonstrations |

This dataset ensures **multi-format interoperability**, allowing seamless use across frameworks such as PyTorch, TensorFlow, MONAI, and Detectron2.

---

## 📁 Folder Structure

50_mri_brain_tumor_annotation_project/
├── raw_data/ # Unannotated MRI brain scans
├── annotated_data/ # Labeled datasets (COCO, YOLO, XML, PNG)
├── metadata/ # Schema, mappings, and dataset descriptors
├── screenshots/ # Project documentation and workflow PDFs
└── README.md # Current documentation file

---

## 🔍 Folder Descriptions

### 🩺 **1. raw_data/**
Contains original, unannotated MRI brain scans — both normal and tumor-affected.  
These serve as the foundation for annotation tasks.  
➡️ [View Raw Data](./raw_data)

---

### 🧩 **2. annotated_data/**
Includes labeled MRI scans exported in multiple formats:
- **COCO JSON** → For PyTorch & Detectron2 pipelines  
- **YOLO TXT** → For YOLOv5–YOLOv8 frameworks  
- **CVAT XML** → Editable format for re-import to CVAT  
- **Segmentation Masks (PNG)** → Pixel-wise tumor boundaries for segmentation tasks  

➡️ [View Annotated Data](./annotated_data)

---

### 📑 **3. metadata/**
Reserved for dataset-level descriptors and schema mappings.  
Currently contains `.keep`, but future versions will include dataset dictionaries and class summaries.  
➡️ [View Metadata](./metadata)

---

### 🖼️ **4. screenshots/**
Contains **visual documentation** of the annotation workflow:
- Project overview reports (PDF)  
- Raw data samples  
- Annotated examples  
- Export summaries  

➡️ [View Screenshots](./screenshots)

---

## ⚙️ Data Preparation Workflow

| Step | Process | Tool/Output |
|------|----------|-------------|
| **1. Data Collection** | MRI brain scans curated from medical imaging datasets | DICOM → PNG |
| **2. Manual Annotation** | Tumor segmentation performed using CVAT (polygon/brush tools) | CVAT |
| **3. Export & Conversion** | Annotations exported in multiple formats (COCO, YOLO, XML, PNG) | CVAT Export |
| **4. Documentation** | Workflow screenshots and reports generated | PDF, PNG |
| **5. Validation** | Visual and logical QA of segmentation masks | Human + Automated checks |

---

## 🧠 Applications

- Tumor boundary segmentation and morphology analysis  
- AI model development for radiology diagnostics  
- Annotation workflow benchmarking  
- Cross-format dataset conversion research  
- Educational demonstrations for medical AI training  

---

## 🧰 Recommended Tools

| Task | Tool |
|------|------|
| Annotation | CVAT, ITK-SNAP, 3D Slicer |
| Visualization | FiftyOne, Roboflow, matplotlib |
| Model Training | MONAI, U-Net, nnU-Net, Detectron2 |
| Format Conversion | CVAT Exporter, Roboflow |
| Evaluation | Dice Coefficient, IoU, Hausdorff Distance |

---

## 🧩 Compatibility

| Framework | Format | Folder |
|------------|---------|--------|
| PyTorch / Detectron2 | COCO JSON | `annotated_data/COCO` |
| YOLOv5–YOLOv8 | YOLO TXT | `annotated_data/YOLO` |
| CVAT | XML | `annotated_data/cvat_xml` |
| MONAI / U-Net | Segmentation PNG | `annotated_data/segmentation_mask` |

---

## 📜 License & Usage

This dataset is released for **research and educational purposes** under an **Open Data License**.  
Users must follow medical data ethics, privacy standards, and institutional research guidelines.

---

## 🔖 Citation (Suggested)

> **Dr. Pradeep AI**  
> *Medical-AI-Data-Annotation: MRI Brain Tumor Segmentation Dataset*, 2025.  
> GitHub Repository: [https://github.com/drpradeepAI/Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🧾 Version Control

| Version | Date | Description |
|----------|------|-------------|
| **1.0** | 2025-10 | Initial release: 50 MRI brain scans with segmentation and multi-format exports |
| **1.1 (Planned)** | 2026-Q1 | Addition of COCO-style mask JSON and expanded metadata descriptors |
