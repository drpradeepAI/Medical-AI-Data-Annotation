# X-Ray Annotated Data – YOLO Format

This folder contains **bounding box annotations** for **50 chest X-ray images** formatted for **YOLO (You Only Look Once)** object detection models.  
Each `.txt` file defines the coordinates and class of detected **mass lesions** in a normalized format compatible with **YOLOv5, YOLOv7, and YOLOv8** frameworks.

---

## 🩻 Dataset Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Region of Interest:** Lungs  
- **Annotation Type:** Bounding Boxes  
- **Annotation Format:** YOLO TXT  
- **Condition Labeled:** Pulmonary Mass Lesions (e.g., tumors, nodules, opacities)  
- **Image Count:** 50  
- **Annotation Tool:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Associated Raw Images:** `raw_data/50_chest_xrays_raw_data_in_jpg/`  

---

## 📁 Folder Structure
YOLO/
├── 50_yolo_txt_format_data/ # Folder containing YOLO TXT label files
│ ├── image_001.txt
│ ├── image_002.txt
│ └── ...
├── 50_chest_xrays_annotated_data_in_yolo_txt_format.zip # Compressed archive
└── .keep

---

## 📄 YOLO TXT Format Specification

Each `.txt` annotation file corresponds to one image and contains lines in the following format:
<class_id> <x_center> <y_center> <width> <height>

All coordinates are **normalized** between **0 and 1** relative to the image dimensions.

---

### 🧩 Example

**For an image of size 1024×1024 px:**
0 0.4102 0.5324 0.2148 0.2549

| Field | Description |
|--------|-------------|
| `0` | Class ID (`mass_lesion`) |
| `0.4102` | Normalized x-coordinate of box center |
| `0.5324` | Normalized y-coordinate of box center |
| `0.2148` | Normalized bounding box width |
| `0.2549` | Normalized bounding box height |

---

## 🧠 Class Labels

| Class ID | Class Name | Description |
|-----------|-------------|-------------|
| 0 | `mass_lesion` | Visible lung lesion such as tumor, opacity, or nodule |

---

## 🔍 Use Cases

- **Training YOLO-based models** (v5, v7, v8, v10) for lesion detection  
- **Testing normalization accuracy** in medical imaging datasets  
- **Fine-tuning pretrained COCO/medical models** on chest X-rays  
- **Benchmarking lesion detection** in comparison with other annotation formats (COCO, VOC)

---

## ⚙️ Data Generation Workflow

1. **Raw X-rays** imported from `raw_data/`.  
2. **Bounding boxes** annotated manually in CVAT.  
3. **Exported in YOLO format** (TXT files).  
4. Validated and organized into `50_yolo_txt_format_data/`.  

---

## 💡 Recommended Tools

| Task | Tool |
|------|------|
| Label Editing | LabelImg, Roboflow, CVAT |
| Model Training | Ultralytics YOLOv8, YOLOv10 |
| Visualization | FiftyOne, OpenCV |
| Validation | Python scripts using `os` and `pandas` |

---

## 🧩 Integration Notes

| Related Folder | Description |
|----------------|-------------|
| `COCO/` | JSON-format annotations for multi-object datasets |
| `VOC/` | XML-format annotations for classic models |
| `CSV/` | Tabular dataset for preprocessing and conversion |
| `raw_data/` | Original unannotated chest X-ray images |

---

## 📜 License

This dataset is provided under an **Open Data License** for **research and educational purposes only**.  
Medical image data usage should always comply with ethical and institutional guidelines.
