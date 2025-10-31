# MRI Annotated Data

This directory contains **annotated MRI brain tumor datasets** prepared in multiple widely used formats — **COCO, YOLO, CVAT XML, and Segmentation Mask** — enabling flexible use across diverse computer vision frameworks and AI research pipelines.

---

## 🧠 Dataset Overview

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Region:** Brain  
- **Condition:** Brain Tumor  
- **Purpose:** Object detection and segmentation model development  
- **Image Source:** `raw_data/50_mri_brain_raw_data_images/`  
- **Annotation Tools Used:** [CVAT](https://cvat.org/), manual expert review  

Each subfolder provides the same annotation dataset exported into different formats, making it compatible with multiple AI model architectures.

---

## 📂 Folder Structure
annotated_data/
├── COCO/ # COCO 1.0 JSON format annotations
├── YOLO/ # YOLO TXT format annotations
├── cvat_xml/ # CVAT XML export format
├── segmentation_mask/ # Pixel-level segmentation masks
└── .keep

---

## 🔍 Annotation Formats

### **1. COCO Format**
- File: `50_mri_brain_tumor_annotated_data_COCO_1.0_json_format.json`
- Suitable for: PyTorch, Detectron2, MMDetection, TensorFlow Object Detection API
- Structure includes:
  - `images` → metadata (filename, size)
  - `annotations` → bounding boxes, segmentation points
  - `categories` → class definitions (e.g., tumor)

➡️ Folder: [`COCO/`](./COCO)

---

### **2. YOLO Format**
- Directory: `50_mri_annotated_yolo_txt_formats/`
- Compressed File: `50_mri_brain_tumor_annotated_data_YOLO_txt_format.zip`
- Format:
<class_id> <x_center> <y_center> <width> <height>
(All coordinates are normalized between 0–1.)
- Suitable for: YOLOv5, YOLOv8, Ultralytics, Roboflow  

➡️ Folder: [`YOLO/`](./YOLO)

---

### **3. CVAT XML Format**
- File: `50_mri_brain_tumor_annotated_data_CVAT_xml_format.xml`
- Stores object metadata, bounding boxes, and polygon segmentation using pixel coordinates.
- Useful for importing/exporting back to CVAT or converting between formats.

➡️ Folder: [`cvat_xml/`](./cvat_xml)

---

### **4. Segmentation Mask Format**
- Files:
- `50_mri_brain_tumor_annotated_data_segmentation_mask_CLASS_.png`
- `50_mri_brain_tumor_annotated_data_segmentation_mask_OBJECT_.png`
- `labelmap.txt`
- Provides pixel-wise labels for **semantic** and **instance** segmentation tasks.  
- Ideal for U-Net, DeepLabV3+, and Mask R-CNN training.

➡️ Folder: [`segmentation_mask/`](./segmentation_mask)

---

## ⚙️ Data Generation Workflow

1. MRI images collected → `raw_data/`  
2. Annotated using **CVAT** with expert guidance  
3. Exported to multiple formats (COCO, YOLO, CVAT XML, Segmentation)  
4. Each format validated for coordinate alignment and consistency  

---

## 💡 Applications

- Brain tumor detection and localization  
- Tumor segmentation and volumetric analysis  
- Model benchmarking across detection frameworks  
- Annotation conversion and dataset standardization research  

---

## 🧰 Recommended Tools

| Purpose | Recommended Tool |
|----------|------------------|
| Visualization | FiftyOne, Roboflow, CVAT |
| Training | Ultralytics YOLO, Detectron2, MONAI |
| Conversion | CVAT, Label Studio Converter |
| Inspection | PyCOCOTools, OpenCV, NumPy |

---

## 📜 License

All annotations are released under an **Open Data License** for **research and educational purposes**.  
Ensure compliance with **ethical and privacy regulations** when using medical data.
