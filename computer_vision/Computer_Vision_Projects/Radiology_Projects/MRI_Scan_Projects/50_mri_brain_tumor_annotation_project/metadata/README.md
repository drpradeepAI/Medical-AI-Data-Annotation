# MRI Metadata

This folder is reserved for **metadata files** that describe the MRI dataset’s structure, annotations, and contextual details.  
Although it is currently empty, it will later serve as the **central reference point** for all dataset-level descriptive information.

---

## 📘 Purpose

The **metadata** folder will contain supporting files that define:
- Dataset-level information (size, structure, formats)
- Image acquisition details (scanner type, sequence parameters, etc.)
- Annotation schema and label definitions
- Dataset versioning and changelogs
- Cross-references between raw data and annotations

---

## 🧱 Example Files (to be added later)

| Filename | Description |
|-----------|--------------|
| `dataset_description.json` | Dataset-wide metadata (study count, image count, modality, etc.) |
| `annotation_schema.json` | Defines label classes, color codes, and annotation attributes |
| `mapping_table.csv` | Links between raw image filenames and corresponding annotation files |
| `version_log.txt` | Documents dataset updates and revisions |
| `license.txt` | License or terms of data use |

---

## ⚙️ Integration with Other Folders

| Folder | Relation to Metadata |
|---------|----------------------|
| `raw_data/` | Metadata may include acquisition parameters and filenames mapping |
| `annotated_data/` | Label schema and export history referenced here |
| `screenshots/` | Documentation metadata may link to progress visuals |
| `README.md` (root) | Summarizes project-level metadata for quick reference |

---

## 🧠 Future Use

Once populated, this folder will enhance:
- Dataset transparency  
- Reproducibility and validation  
- Standardization for AI and research workflows  

---

## 📜 Note

At present, only a `.keep` file is stored to maintain folder structure.  
Additional metadata files will be added progressively as the project evolves.
