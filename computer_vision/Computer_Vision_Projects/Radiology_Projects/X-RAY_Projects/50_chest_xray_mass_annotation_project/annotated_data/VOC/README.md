# X-Ray Annotated Data – Pascal VOC Format

This folder contains **bounding box annotations** for **50 chest X-ray images** in the **Pascal VOC XML format**.  
Each XML file defines the **object class (`mass_lesion`)** and its **bounding box coordinates** for lesion localization tasks in medical imaging AI.

---

## 🩻 Dataset Overview

- **Modality:** X-Ray (Chest Radiography)  
- **Target Condition:** Pulmonary Mass Lesions (tumors, nodules, opacities)  
- **Annotation Type:** Bounding Boxes  
- **Format:** Pascal VOC XML  
- **Annotation Count:** 50 files (1 per image)  
- **Exported From:** [CVAT – Computer Vision Annotation Tool](https://cvat.org/)  
- **Associated Images:** `raw_data/50_chest_xrays_raw_data_in_jpg/`

---

## 📁 Folder Structure
VOC/
├── 50_chest_xrays_annotated_data_in_voc_xml_format.xml # Pascal VOC annotation file
└── .keep

---

## 🧩 Pascal VOC XML Structure

Each annotation file follows the standard **Pascal VOC schema**:

```xml
<annotation>
    <folder>raw_data</folder>
    <filename>image_001.jpg</filename>
    <path>./raw_data/image_001.jpg</path>
    <size>
        <width>1024</width>
        <height>1024</height>
        <depth>3</depth>
    </size>
    <object>
        <name>mass_lesion</name>
        <pose>Unspecified</pose>
        <truncated>0</truncated>
        <difficult>0</difficult>
        <bndbox>
            <xmin>310</xmin>
            <ymin>420</ymin>
            <xmax>530</xmax>
            <ymax>670</ymax>
        </bndbox>
    </object>
</annotation>
Field Description
Field	Meaning
filename	X-ray image filename
size	Image width, height, and color channels
object	Contains class label and bounding box info
bndbox	Defines the bounding box in [xmin, ymin, xmax, ymax]
name	Object label — here, "mass_lesion"
🔍 Use Cases

Training object detection models such as Faster R-CNN, SSD, or YOLO (after conversion)

Dataset interoperability between medical imaging frameworks

Benchmarking lesion detection performance using Pascal VOC metrics (mAP, IoU)

⚙️ Data Generation Workflow

Chest X-rays collected from the raw_data/ folder.

Bounding boxes drawn in CVAT for visible lung lesions.

Exported as Pascal VOC XML.

Validated for label consistency and coordinate integrity.

💡 Recommended Tools
Purpose	Tool
Viewing XML	VS Code, Notepad++, XML Explorer
Conversion	Roboflow, FiftyOne, CVAT Converter
Training Frameworks	TensorFlow Object Detection API, Detectron2, MMDetection
Validation	Python xml.etree.ElementTree, lxml
🧠 Integration Notes
Related Folder	Description
COCO/	JSON-based annotations for multi-object detection
CSV/	Tabular annotations for quick analysis
YOLO/	TXT format annotations for YOLOv5–v8
raw_data/	Original X-ray images used for labeling
📜 License

This dataset is provided under an Open Data License for research and educational purposes only.
Users must ensure compliance with ethical standards and privacy regulations for medical data.
