# 🧾 Metadata — Cardiology EHR Dataset (20 Annotated Cases)

This folder contains structured **metadata files** describing all **20 manually annotated cardiology EHR case notes**.  
These metadata files ensure **traceability, transparency, and reproducibility** of the dataset creation process.

Each metadata record links the **raw data**, **annotated output**, **schema version**, and **quality control status**, providing a complete view of the dataset pipeline.

---

## 📂 Files Overview

| File Name | Description |
|------------|--------------|
| `metadata.csv` | Tabular metadata file for spreadsheet-based review and quick reference. Includes case-level summaries, annotation mapping, and QA details. |
| `metadata.json` | Machine-readable JSON version of the same metadata — optimized for integration into data pipelines and NLP model training scripts. |

---

## 🧠 Metadata Schema (Fields Explained)

| Field | Description |
|--------|-------------|
| `case_id` | Unique identifier for each cardiology case (e.g., `case_001`–`case_020`). |
| `specialty` | Medical specialty (Cardiology). |
| `annotated_file` | The corresponding annotated dataset file name (e.g., `cardio_cases_annotated.json`). |
| `schema_version` | Version of the label configuration used (`36_labels_v1`). |
| `export_format` | Format of exported annotations (e.g., `doccano_json(v1)`). |
| `qa_status` | Quality assurance review status (e.g., `PENDING`, `PASSED`). |

---

## ⚙️ Purpose and Design

The metadata provides:

- **📋 Traceability:** Links every case from raw input to final annotated output.  
- **✅ Quality Assurance:** Tracks verification and curation status of each record.  
- **🤖 Automation:** Facilitates integration with machine learning pipelines.  
- **📚 Documentation:** Provides structured context for downstream research and dataset citation.  

---

## 📊 Example Records

### `metadata.csv` (sample)
```csv
case_id,specialty,annotated_file,schema_version,export_format,qa_status
case_001,Cardiology,cardio_cases_annotated.json,36_labels_v1,doccano_json(v1),PENDING
case_002,Cardiology,cardio_cases_annotated.json,36_labels_v1,doccano_json(v1),PENDING
...
case_020,Cardiology,cardio_cases_annotated.json,36_labels_v1,doccano_json(v1),PENDING
metadata.json (sample)
{
  "case_id": "case_001",
  "specialty": "Cardiology",
  "annotated_file": "cardio_cases_annotated.json",
  "schema_version": "36_labels_v1",
  "export_format": "doccano_json(v1)",
  "qa_status": "PENDING"
}
🩺 Integration Context

The metadata connects all key components of the dataset:

Raw Data → raw_data/

Annotations → annotated_data/

Label Schema → label_schema/

Screenshots → screenshots/

It acts as a central reference map for the 20_Cardio_Cases_NLP_Project
 within the
ClinicalCaseNotesEHRs
 collection under
Natural_Language_Processing

in the Medical-AI-Data-Annotation
 repository.

👨‍⚕️ Maintained by

drpradeepAI

Medical AI Data Annotator , Clinical NLP Specialist , MBBS Doctor

⭐ This metadata layer forms the backbone of dataset integrity, version control, and audit readiness.
