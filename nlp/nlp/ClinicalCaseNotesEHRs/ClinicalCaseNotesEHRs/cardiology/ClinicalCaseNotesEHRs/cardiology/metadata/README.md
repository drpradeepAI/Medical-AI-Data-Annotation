# 🧾 Metadata – Cardiology EHR Dataset (20 Annotated Cases)

This folder contains **metadata files** describing the 20 annotated cardiology case notes in structured formats.  
Metadata provides detailed context for each case, such as case ID, specialty, annotation file mapping, and quality assurance status.

---

## 📂 File Descriptions

| File | Description |
|------|--------------|
| `metadata.csv` | Case-level summary in tabular format (ideal for spreadsheet view). Includes case IDs, source files, annotation references, and QA status. |
| `metadata.json` | Same information in JSON structure for programmatic access or automated dataset loading. |

---

## 🧩 Metadata Schema (Fields Explained)

| Field | Description |
|--------|-------------|
| `case_id` | Unique identifier for each cardiology case (e.g., case_001 to case_020). |
| `specialty` | Medical specialty (Cardiology). |
| `source_raw_csv` | Filename of raw CSV input file. |
| `source_raw_json` | Filename of raw JSONL input file. |
| `annotated_file` | Corresponding annotated JSONL export file. |
| `label_schema_file` | Path to label configuration used for this annotation. |
| `admission_date` | (Optional) Date of case admission. |
| `discharge_date` | (Optional) Date of discharge. |
| `note_chars` | Number of characters in note (for length-based stats). |
| `note_sentences` | Number of sentences in the case note. |
| `annotations_count` | Total number of entity annotations in that case. |
| `export_format` | Format of annotated file (e.g., Doccano JSONL). |
| `schema_version` | Version of label schema used (v36_labels_final). |
| `annotator` | Name/ID of annotator (Dr. Pradeep). |
| `qa_status` | Review status (e.g., PENDING / PASSED). |
| `remarks` | Notes about case or special observations. |

---

## 🧠 Purpose

Metadata ensures:
- **Traceability** – each case is linked to raw, annotated, and schema files.  
- **Quality Control** – easy tracking of review status for every record.  
- **Automation** – compatible with dataset management and machine learning pipelines.  

---

## 📊 Example Snippet (CSV / JSON)

### `metadata.csv` sample:
```csv
case_id,specialty,annotated_file,qa_status,note_sentences,annotations_count
case_001,Cardiology,20_cardio_cases_annotated_data.jsonl,PASSED,28,63
case_002,Cardiology,20_cardio_cases_annotated_data.jsonl,PASSED,32,77
