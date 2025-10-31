# X-Ray Annotated Data – COCO Format

This folder contains **bounding box annotations** for **50 chest X-ray images** in **COCO JSON format**.  
The annotations correspond to regions of interest (ROIs) representing **mass lesions** in the lungs, enabling AI models to learn **object detection** and **localization** tasks.

---

## 🩻 Dataset Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Condition:** Pulmonary Mass Lesions (e.g., tumors, nodules, opacities)  
- **Annotation Type:** Bounding Boxes  
- **Format:** COCO (Common Objects in Context) JSON  
- **Number of Images:** 50  
- **Export Tool:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Image Source:** `raw_data/50_chest_xrays_raw_data_in_jpg/`  

---

## 📁 Folder Structure
COCO/
├── 50_chest_xrays_annotated_data_in_coco_json_format.json # COCO 1.0 annotation file
└── .keep

---

## 🧩 COCO Schema Overview

Each annotation entry in the JSON file follows the COCO structure:
```json
{
  "images": [
    {
      "id": 1,
      "file_name": "image_001.jpg",
      "width": 1024,
      "height": 1024
    }
  ],
  "annotations": [
    {
      "id": 1,
      "image_id": 1,
      "category_id": 1,
      "bbox": [x, y, width, height],
      "area": 4500.0,
      "iscrowd": 0
    }
  ],
  "categories": [
    {
      "id": 1,
      "name": "mass_lesion",
      "supercategory": "thoracic_pathology"
    }
  ]
}
Field Description
Field	Meaning
images	Metadata for each X-ray image
annotations	Bounding box coordinates and region details
categories	Defines the class label (mass_lesion)
bbox	Format → [x_min, y_min, width, height] in pixels
🔍 Use Cases

Training COCO-compatible object detection models like:

YOLOv8 (after conversion)

Detectron2

TensorFlow Object Detection API

Benchmarking medical AI systems for mass lesion localization

Inter-format conversion to YOLO or Pascal VOC for cross-framework experiments

⚙️ Data Generation Workflow

Raw X-ray images imported from raw_data/.

Annotated using bounding boxes in CVAT.

Exported in COCO 1.0 JSON format.

Verified using COCO-API
 and FiftyOne
.

💡 Recommended Tools
Task	Tool
Annotation	CVAT
Visualization	FiftyOne, Roboflow
Model Training	Detectron2, YOLOv8, MMDetection
Validation	PyCOCOTools, JSONLint
📜 License

This annotated dataset is released under an Open Data License for research and educational use only.
Ensure compliance with medical data privacy and ethical guidelines before redistribution or model training.
