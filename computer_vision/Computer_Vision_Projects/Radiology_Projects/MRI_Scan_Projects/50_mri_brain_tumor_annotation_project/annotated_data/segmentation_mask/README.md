# MRI Annotated Data – Segmentation Mask Format

This folder contains **MRI brain tumor annotations** represented as **segmentation masks**.  
Each mask image corresponds pixel-by-pixel to its original MRI scan, marking tumor and background regions for precise segmentation model training.

---

## 📁 Folder Structure
segmentation_mask/
├── 50_mri_brain_tumor_annotated_data_segmentation_mask_CLASS_.png # Class-level segmentation masks
├── 50_mri_brain_tumor_annotated_data_segmentation_mask_OBJECT_.png # Object-level segmentation masks
├── labelmap.txt # Label index and color map reference
└── .keep

---

## 🧠 Dataset Description

- **Modality:** MRI (Magnetic Resonance Imaging)  
- **Region:** Brain  
- **Condition:** Brain Tumor  
- **Annotation Format:** Segmentation Mask (CLASS & OBJECT level)  
- **Image Type:** PNG (grayscale or indexed color)  
- **Dimensions:** Match original MRI images in `raw_data/50_mri_brain_raw_data_images/`  

Each pixel value in a mask represents a **class label** (e.g., 0 = background, 1 = tumor).  
The dataset supports **semantic** and **instance** segmentation pipelines.

---

## 🧩 Types of Masks

| Mask Type | Description |
|------------|--------------|
| **CLASS Mask** | Encodes regions based on class category (e.g., tumor vs background). |
| **OBJECT Mask** | Encodes each tumor instance as a unique object ID for instance-level segmentation. |

---

## 🗂️ labelmap.txt Format

The `labelmap.txt` file defines class mappings used in both CLASS and OBJECT masks:
0: Background
1: Tumor

(Additional labels can be added for multi-class medical segmentation.)

---

## 🔍 Use Cases

- Training **U-Net, DeepLabV3+, Mask R-CNN**, or **Segment Anything (SAM)** models  
- Evaluating tumor boundaries and morphology  
- Developing pixel-level medical imaging AI systems  
- Converting segmentation masks to COCO RLE or polygon formats  

---

## ⚙️ Data Generation Pipeline

1. MRI images annotated in **CVAT** using polygonal segmentation.  
2. Exported as **segmentation masks** (both class and object modes).  
3. Label consistency verified using `labelmap.txt`.  
4. Mask images aligned with original MRI scan dimensions.

---

## 💡 Recommended Tools

- [CVAT](https://cvat.org/) — for mask export and visualization  
- [FiftyOne](https://voxel51.com/fiftyone/) — for dataset inspection  
- [Roboflow](https://roboflow.com/) — for mask augmentation  
- [MONAI](https://monai.io/) — for medical segmentation model training  

---

## 📜 License

This segmentation dataset is released under an **Open Data License** for **research and educational purposes**.  
Ensure adherence to medical data ethics and privacy guidelines when using these masks.
