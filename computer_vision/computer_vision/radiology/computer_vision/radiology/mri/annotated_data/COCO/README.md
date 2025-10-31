# MRI Annotated Data – COCO Format

This folder contains **MRI brain tumor annotated data** in **COCO JSON format**, suitable for use in computer vision model training and evaluation.

---

## 📁 Folder Structure
COCO/
├── 50_mri_brain_tumor_annotated_data_COCO_1.0_json_format.json # COCO-style annotation file
└── .keep

---

## 🧠 Dataset Description

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Region:** Brain  
- **Condition:** Brain Tumor  
- **Annotation Format:** COCO (Common Objects in Context)  
- **Annotation File:** `50_mri_brain_tumor_annotated_data_COCO_1.0_json_format.json`  
- **Image Source:** Corresponding MRI images available in the `raw_data/` folder  

This JSON file contains bounding box or segmentation-based annotations compliant with the **COCO dataset standard**, used in many deep learning frameworks such as **PyTorch, TensorFlow, Detectron2**, etc.

---

## 🧩 COCO Annotation Schema Overview

Each entry in the JSON file follows the COCO structure:
- `images`: metadata of each MRI image (file name, width, height, etc.)
- `annotations`: tumor region details (bounding boxes, segmentation, and image references)
- `categories`: list of object classes (e.g., "tumor", "brain", etc.)

---

## 🔍 Use Cases

- **Training COCO-compatible detection/segmentation models**  
- **Benchmarking medical imaging models**  
- **Validating YOLO or CVAT-converted datasets**  
- **Cross-format conversion** to YOLO, Pascal VOC, or CVAT XML  

---

## ⚙️ Data Preparation

1. Raw images are stored in `raw_data/50_mri_brain_raw_data_images/`.  
2. Annotation was performed manually or semi-automatically.  
3. Exported from CVAT as `COCO 1.0 JSON format`.  

---

## 💡 Recommended Tools

- [CVAT](https://cvat.org/) for annotation  
- [Roboflow](https://roboflow.com/) or [FiftyOne](https://voxel51.com/fiftyone/) for dataset visualization  
- [PyCOCOTools](https://github.com/cocodataset/cocoapi) for loading and validating JSON annotations  

---

## 📜 License

This annotated dataset is released for **research and educational purposes** under an **Open Data License**.  
Please ensure compliance with ethical standards and data privacy norms when using medical datasets.
