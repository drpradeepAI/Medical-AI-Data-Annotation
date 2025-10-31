# X-Ray Annotated Data

This directory contains **bounding box annotations** for **50 chest X-ray images** curated for **mass lesion detection** tasks.  
Each subfolder represents a different **annotation format** (COCO, CSV, Pascal VOC, and YOLO), enabling flexible use across major deep learning frameworks.

---

## 🩻 Project Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Region of Interest:** Lungs and Thoracic Cavity  
- **Primary Task:** Object Detection (Mass Lesion Localization)  
- **Annotation Type:** Bounding Boxes  
- **Image Count:** 50 chest X-ray images  
- **Condition Annotated:** Pulmonary mass lesions (e.g., tumors, nodules, opacities)  
- **Annotation Source:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Associated Raw Dataset:** `raw_data/50_chest_xrays_raw_data_in_jpg/`  

---

## 📁 Folder Structure
annotated_data/
├── COCO/ # COCO 1.0 JSON annotations
│ └── 50_chest_xrays_annotated_data_in_coco_json_format.json
│
├── CSV/ # CSV tabular annotations
│ └── 50_chest_xrays_annotated_data_in_csv_format.csv
│
├── VOC/ # Pascal VOC XML annotations
│ └── 50_chest_xrays_annotated_data_in_voc_xml_format.xml
│
├── YOLO/ # YOLO TXT annotations
│ └── 50_yolo_txt_format_data/
│ ├── image_001.txt
│ └── ...
│
└── .keep # Placeholder for version control

---

## 🧩 Annotation Format Comparison

| Format | File Type | Framework Compatibility | Key Features |
|--------|------------|--------------------------|---------------|
| **COCO** | `.json` | Detectron2, MMDetection, PyTorch | Supports multi-class & segmentation metadata |
| **CSV** | `.csv` | Custom scripts, pandas, Roboflow | Easy for analysis & preprocessing |
| **Pascal VOC** | `.xml` | TensorFlow, SSD, Faster R-CNN | Classic structured XML format |
| **YOLO** | `.txt` | YOLOv5–YOLOv10, Ultralytics | Lightweight, normalized coordinates |

---

## 🧠 Annotation Schema

All formats use a **single class label** for detection:
| Class ID | Label Name | Description |
|-----------|-------------|-------------|
| 0 | `mass_lesion` | Visible lung mass, tumor, or opacity in chest X-ray |

---

## ⚙️ Annotation Workflow

1. **Raw Data Source:** 50 high-quality chest X-ray images from open medical datasets.  
2. **Annotation Tool:** Annotated manually in **CVAT** using bounding boxes.  
3. **Formats Exported:** COCO, CSV, Pascal VOC, and YOLO TXT formats.  
4. **Verification:** Cross-checked for coordinate accuracy and class consistency.  

---

## 💡 Use Cases

- Training **object detection models** for thoracic pathology localization  
- Benchmarking AI model performance across annotation standards  
- Cross-format dataset conversion & analysis  
- Teaching dataset structuring in medical AI projects  

---

## 🔧 Recommended Tools

| Task | Suggested Tool |
|------|----------------|
| Annotation & Export | CVAT, LabelImg, Roboflow |
| Visualization | FiftyOne, OpenCV, matplotlib |
| Conversion | Roboflow, CVAT Export Converter |
| Model Training | YOLOv8, Detectron2, TensorFlow Object Detection API |
| Dataset Validation | PyCOCOTools, XML Parsers, pandas |

---

## 🧩 Integration Notes

| Related Folder | Description |
|----------------|-------------|
| `raw_data/` | Contains unannotated chest X-ray images |
| `metadata/` | Reserved for dataset descriptors or image mapping |
| `screenshot/` | Project overview and annotation visual previews |

---

## 📜 License

This annotated dataset is provided under an **Open Data License** for **educational and research purposes only**.  
Usage must comply with medical data privacy and ethical research guidelines.
