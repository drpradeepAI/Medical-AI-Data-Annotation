# MRI Annotated Data – YOLO Format

This folder contains **MRI brain tumor annotated data** in **YOLO text format** (`.txt`), ready for use in object detection and segmentation model training.

---

## 📁 Folder Structure
YOLO/
├── 50_mri_annotated_yolo_txt_formats/ # YOLO-format annotation files
├── 50_mri_brain_tumor_annotated_data_YOLO_txt_format.zip # Compressed archive of YOLO annotations
└── .keep

---

## 🧠 Dataset Description

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Region:** Brain  
- **Condition:** Brain Tumor  
- **Annotation Format:** YOLO (You Only Look Once)  
- **Annotation Files:** `.txt` files (one per image)  
- **Image Source:** `raw_data/50_mri_brain_raw_data_images/`  

Each annotation `.txt` file corresponds to a single MRI image and follows the **YOLO labeling convention**:
<class_id> <x_center> <y_center> <width> <height>
All coordinates are **normalized (0–1)** relative to image width and height.

---

## 🔍 Use Cases

- Training YOLOv5, YOLOv7, YOLOv8, or Ultralytics models  
- Converting annotations between COCO, CVAT, and Pascal VOC formats  
- Rapid experimentation in brain tumor detection pipelines  

---

## ⚙️ Data Preparation Pipeline

1. MRI images annotated in CVAT.  
2. Exported as YOLO TXT format (`YOLO 1.1`).  
3. Verified for bounding box correctness and normalized coordinates.  
4. Available as individual `.txt` files and a zipped archive.  

---

## 💡 Recommended Tools

- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)  
- [CVAT](https://cvat.org/) for format exports  
- [Roboflow](https://roboflow.com/) for visualization & augmentation  
- [FiftyOne](https://voxel51.com/fiftyone/) for dataset inspection  

---

## 🧩 Example

Example YOLO label file:
0 0.532 0.477 0.214 0.302
Here:
- `0` → class ID for *tumor*  
- `0.532`, `0.477` → center coordinates (x, y)  
- `0.214`, `0.302` → width and height of bounding box (normalized)

---

## 📜 License

This dataset is released under an **Open Data License** for **research and educational purposes**.  
Ensure compliance with ethical guidelines and medical data privacy standards when using it.
