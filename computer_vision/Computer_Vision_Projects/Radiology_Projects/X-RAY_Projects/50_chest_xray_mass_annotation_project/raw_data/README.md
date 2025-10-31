# X-Ray Raw Data

This folder contains **unannotated chest X-ray images** used as the source dataset for bounding box–based **mass lesion detection**.  
All images in this directory are **raw input scans** that serve as the foundation for annotations stored in the `annotated_data/` folder.

---

## 🩻 Dataset Overview

- **Modality:** X-Ray (Digital Radiography)  
- **Anatomical Region:** Chest  
- **Primary Target:** Detection of visible mass lesions  
- **Annotation Type:** Bounding Boxes (in annotated dataset)  
- **File Format:** `.jpg`  
- **Image Count:** 50 chest X-ray images  
- **Data Type:** Frontal (PA/AP) chest X-rays  

---

## 📁 Folder Structure
raw_data/
├── 50_chest_xrays_raw_data_in_jpg/ # Folder containing 50 raw X-ray images
│ ├── image_001.jpg
│ ├── image_002.jpg
│ └── ...
├── 50_chest_xrays_raw_data_in_jpg.zip # Compressed archive of the same dataset
└── .keep

---

## 🧠 Dataset Description

These chest X-ray images represent **diverse thoracic cases**, curated for use in **mass lesion object detection** tasks.  
Each image is preprocessed and standardized for consistent annotation and model training.

- **Preprocessing Steps Applied:**
  - Image resizing to uniform dimensions  
  - Removal of duplicated or low-contrast images  
  - Normalized intensity levels suitable for AI pipelines  

---

## 🔍 Use Cases

- Training models for **mass lesion detection** using bounding boxes  
- Evaluating deep learning architectures such as **YOLOv5–YOLOv8**, **Faster R-CNN**, and **RetinaNet**  
- Generating baseline models for chest pathology localization  

---

## ⚙️ Recommended Tools

| Purpose | Tool |
|----------|------|
| Image Visualization | ImageJ, RadiAnt Viewer, or VS Code |
| Annotation | CVAT, Roboflow, LabelImg |
| Preprocessing | OpenCV, NumPy, Pillow |
| Model Training | Ultralytics YOLO, Detectron2, TensorFlow Object Detection API |

---

## 🧩 Integration Notes

| Folder | Description |
|---------|-------------|
| `annotated_data/` | Contains corresponding bounding box annotations in YOLO, COCO, and VOC formats |
| `metadata/` | Will store mapping files or acquisition logs (if available) |
| `screenshot/` | Contains documentation or preview images of annotated bounding boxes |

---

## 📜 License

This dataset is provided under an **Open Data License** for **research and educational purposes only**.  
Ensure compliance with ethical, privacy, and institutional data-use regulations when working with medical imagery.
