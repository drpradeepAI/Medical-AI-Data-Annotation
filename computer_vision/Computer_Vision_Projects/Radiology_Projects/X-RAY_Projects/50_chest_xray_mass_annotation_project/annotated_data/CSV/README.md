# X-Ray Annotated Data – CSV Format

This folder contains **bounding box annotations** for **50 chest X-ray images** in **CSV format**.  
Each record corresponds to a single mass lesion bounding box labeled during annotation.  
The data is designed for flexible use in AI pipelines, especially for model prototyping, dataset visualization, and conversion.

---

## 🩻 Dataset Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Anatomical Region:** Thoracic Cavity  
- **Target:** Pulmonary Mass Lesions (e.g., tumors, nodules, opacities)  
- **Annotation Type:** Bounding Boxes  
- **File Format:** `.csv`  
- **Annotation Source:** Exported from [CVAT](https://cvat.org/)  
- **Associated Raw Images:** `raw_data/50_chest_xrays_raw_data_in_jpg/`  

---

## 📁 Folder Structure
CSV/
├── 50_chest_xrays_annotated_data_in_csv_format.csv # Annotation file in CSV format
└── .keep

---

## 📄 CSV File Schema

The CSV file contains structured tabular annotation data with the following columns:

| Column Name | Description |
|--------------|-------------|
| **filename** | Name of the corresponding X-ray image file |
| **width** | Image width in pixels |
| **height** | Image height in pixels |
| **class** | Object class (here: `mass_lesion`) |
| **xmin** | Top-left X coordinate of the bounding box |
| **ymin** | Top-left Y coordinate of the bounding box |
| **xmax** | Bottom-right X coordinate of the bounding box |
| **ymax** | Bottom-right Y coordinate of the bounding box |

---

### 🧩 Example
filename,width,height,class,xmin,ymin,xmax,ymax
image_001.jpg,1024,1024,mass_lesion,310,420,530,670
image_002.jpg,1024,1024,mass_lesion,280,330,500,590

---

## 🔍 Use Cases

- Quick parsing and visualization in **Python** or **Excel**  
- Converting to COCO, YOLO, or Pascal VOC formats  
- Evaluating dataset structure and annotation consistency  
- Simple integration with custom machine learning scripts or dashboards  

---

## ⚙️ Data Generation Workflow

1. Chest X-rays imported from `raw_data/`.  
2. Annotated using bounding boxes in **CVAT**.  
3. Exported as CSV via **CVAT CSV export tool**.  
4. Verified for coordinate alignment and format integrity.  

---

## 💡 Recommended Tools

| Purpose | Tool |
|----------|------|
| CSV Visualization | Microsoft Excel, Google Sheets, or pandas |
| Conversion | Roboflow, FiftyOne, CVAT Converter |
| Validation | pandas, NumPy, JSON-to-CSV scripts |
| Model Training | YOLOv8, TensorFlow Object Detection, Detectron2 |

---

## 🧠 Integration Notes

| Related Folder | Description |
|----------------|-------------|
| `COCO/` | JSON annotations for deep learning frameworks |
| `VOC/` | Pascal VOC XML format annotations |
| `YOLO/` | YOLO TXT annotations for object detection |
| `raw_data/` | Original chest X-ray images |

---

## 📜 License

This annotation dataset is released under an **Open Data License** for **educational and research purposes only**.  
Use of medical images must comply with privacy and ethical data-use standards.
