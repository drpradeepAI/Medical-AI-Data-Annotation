# MRI Dataset – Brain Tumor Annotation Project

This folder contains a **comprehensive MRI brain tumor dataset**, including **raw scans, annotated data, metadata, and documentation screenshots**.  
It demonstrates the complete data annotation pipeline for medical AI research and development.

---

## 🧠 Overview

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Anatomical Region:** Brain  
- **Primary Condition:** Brain Tumor (includes normal and abnormal scans)  
- **Data Purpose:** Model development for tumor detection, segmentation, and classification  
- **Annotation Tool:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Exported Formats:** COCO, YOLO, CVAT XML, Segmentation Mask  

The dataset is structured for **multi-format interoperability**, making it directly usable with popular deep learning frameworks like PyTorch, TensorFlow, and MONAI.

---

## 📁 Folder Structure
mri/
├── raw_data/ # Original unannotated MRI images
├── annotated_data/ # Labeled data in multiple formats (COCO, YOLO, XML, Mask)
├── metadata/ # Reserved for dataset descriptors, schema, and mapping files
├── screenshots/ # Visual documentation and workflow PDFs
└── README.md # This overview file

---

## 🔍 Folder Descriptions

### **1. raw_data/**
Contains unannotated MRI scans used as base input for annotation.  
Each image represents either a normal or tumor-affected brain region.  
➡️ [View Raw Data](./raw_data)

---

### **2. annotated_data/**
Includes labeled MRI datasets exported in multiple annotation formats:
- **COCO JSON** → Standard format for PyTorch/Detectron2  
- **YOLO TXT** → Optimized for YOLOv5–YOLOv8 training  
- **CVAT XML** → Editable format for re-import into CVAT  
- **Segmentation Mask** → Pixel-level tumor boundaries  

➡️ [View Annotated Data](./annotated_data)

---

### **3. metadata/**
Reserved for descriptive and structural metadata such as dataset schema, mapping tables, or version logs.  
Currently contains only a `.keep` file, but intended for future dataset descriptors.  
➡️ [View Metadata](./metadata)

---

### **4. screenshots/**
Contains **visual documentation**, including:
- Project overview PDFs  
- Annotation preview images  
- Export configuration references  
These files visually demonstrate the data pipeline and final outputs.  
➡️ [View Screenshots](./screenshots)

---

## ⚙️ Data Preparation Workflow

1. **Data Collection:** MRI brain scans curated from open-access medical datasets.  
2. **Annotation:** Conducted via CVAT with class-level (tumor/background) and object-level segmentation.  
3. **Export & Validation:** Annotations exported to COCO, YOLO, XML, and mask formats.  
4. **Documentation:** Screenshots and PDFs created to ensure reproducibility.  

---

## 🧩 Compatibility

| Framework | Supported Format | Folder |
|------------|------------------|--------|
| PyTorch / Detectron2 | COCO JSON | `annotated_data/COCO` |
| Ultralytics YOLOv5–v8 | YOLO TXT | `annotated_data/YOLO` |
| CVAT | XML | `annotated_data/cvat_xml` |
| MONAI / U-Net | PNG Masks | `annotated_data/segmentation_mask` |

---

## 💡 Applications

- Brain tumor detection and localization  
- Tumor segmentation and boundary extraction  
- Cross-format dataset conversion testing  
- AI-assisted medical imaging workflows  
- Annotation tool benchmarking  

---

## 🧰 Recommended Tools

| Task | Tool |
|------|------|
| Annotation | [CVAT](https://cvat.org/), Label Studio |
| Visualization | FiftyOne, Roboflow |
| Model Training | YOLOv8, Detectron2, MONAI |
| Format Conversion | Label Studio Converter, CVAT Exporter |

---

## 📜 License

This dataset and its documentation are released under an **Open Data License**  
for **educational and non-commercial research purposes**.  
Ensure compliance with ethical and privacy guidelines in medical data use.

---

## 🧾 Citation

If you use this dataset or its structure in your work, please cite:

> “Medical-AI-Data-Annotation: MRI Brain Tumor Dataset (2025)”  
> Created by Dr. Pradeep A.I.  
> [GitHub Repository](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)
