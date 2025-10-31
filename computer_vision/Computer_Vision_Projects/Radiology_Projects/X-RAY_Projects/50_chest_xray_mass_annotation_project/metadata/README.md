# X-Ray Dataset Metadata

This folder is **reserved for metadata files** associated with the **X-Ray mass lesion detection dataset**.  
It acts as a centralized space for storing structured information that describes, indexes, and links the dataset’s contents across multiple formats and folders.

---

## 📘 Purpose

The metadata directory ensures **traceability**, **consistency**, and **context** for the X-ray dataset.  
It will later contain dataset-level descriptors that provide:
- Information about dataset structure and hierarchy.  
- Mapping between raw and annotated files.  
- Data versioning and changelogs.  
- Class label and annotation schema documentation.  
- Machine-readable descriptors for automation and reproducibility.

---

## 🩻 Related Dataset Context

| Property | Description |
|-----------|-------------|
| **Modality** | X-Ray (Chest Radiography) |
| **Task** | Mass Lesion Detection |
| **Annotations Available** | Bounding Boxes |
| **Annotation Formats** | COCO, CSV, Pascal VOC, YOLO |
| **Image Count** | 50 |
| **Tool Used** | [CVAT – Computer Vision Annotation Tool](https://cvat.org/) |

---

## 🧩 Planned Metadata Files

| Filename (Proposed) | Description |
|----------------------|-------------|
| `dataset_description.json` | Contains dataset summary, purpose, and structure. |
| `file_index_mapping.csv` | Maps raw image filenames to annotated data files. |
| `class_label_schema.json` | Defines class names, IDs, and descriptions. |
| `annotation_summary.csv` | Summarizes number of annotations per image. |
| `dataset_version_log.txt` | Records dataset version history and updates. |

---

## 📂 Folder Structure
metadata/
├── .keep # Placeholder for Git versioning
├── dataset_description.json # (planned)
├── file_index_mapping.csv # (planned)
├── class_label_schema.json # (planned)
└── dataset_version_log.txt # (planned)

---

## 💡 Integration Notes

| Related Folder | Description |
|----------------|-------------|
| `raw_data/` | Contains 50 original unannotated X-ray images. |
| `annotated_data/` | Contains bounding box annotations in COCO, CSV, VOC, and YOLO formats. |
| `screenshot/` | Documentation and visual audit files. |
| `metadata/` | Current folder — reserved for dataset descriptors, mappings, and version logs. |

---

## 📜 License

All metadata and dataset descriptors will be released under the same **open license** as the dataset itself.  
Intended for **research, educational, and AI development purposes** only.
