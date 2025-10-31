# MRI Annotated Data – CVAT XML Format

This folder contains **MRI brain tumor annotations** exported in **CVAT XML format**, ideal for interoperability between labeling tools and dataset conversion workflows.

---

## 📁 Folder Structure
cvat_xml/
├── 50_mri_brain_tumor_annotated_data_CVAT_xml_format.xml # CVAT export file
└── .keep

---

## 🧠 Dataset Description

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Region:** Brain  
- **Condition:** Brain Tumor  
- **Annotation Format:** CVAT XML  
- **Annotation Source:** Created using [CVAT (Computer Vision Annotation Tool)](https://cvat.org/)  
- **Associated Images:** Available in `raw_data/50_mri_brain_raw_data_images/`

This XML file stores annotation data such as bounding boxes, polygon masks, and object metadata structured according to **CVAT’s internal XML schema**.

---

## 🧩 CVAT XML Schema Overview

Each annotated object includes details such as:
```xml
<image id="0" name="image_001.jpg" width="512" height="512">
    <box label="tumor" xtl="120" ytl="180" xbr="260" ybr="320"/>
</image>
Where:

label → Object class (e.g., tumor)

xtl, ytl → Top-left corner coordinates

xbr, ybr → Bottom-right corner coordinates

All coordinates are in pixel values, matching the source image dimensions.

🔍 Use Cases

Importing into CVAT for further editing

Converting to YOLO, COCO, or Pascal VOC formats

Training AI models that use XML-based label structures

Dataset archival with metadata preservation

⚙️ Data Preparation Steps

MRI images annotated in CVAT using bounding boxes and masks.

Exported as CVAT XML format.

Verified and cleaned for structural consistency.

Linked with corresponding MRI raw data images.

💡 Recommended Tools

CVAT
 — for creating or re-importing XML annotations

FiftyOne
 — for visual verification

Label Studio Converter
 — for format conversion

📜 License

This dataset is released under an Open Data License for educational and research purposes only.
Users must comply with medical data ethics and privacy regulations.
