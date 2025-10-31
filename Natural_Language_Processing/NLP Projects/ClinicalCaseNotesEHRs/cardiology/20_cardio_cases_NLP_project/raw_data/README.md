# 📄 Raw Data — Cardiology Clinical Case Notes

This folder contains the **original, unannotated Electronic Health Record (EHR)** texts used as the **source material** for the cardiology NLP annotation project.  
These notes represent complete patient encounters, prepared for downstream processing in **[Doccano](https://github.com/doccano/doccano)**.

---

## 📁 File Inventory

| File Name | Description |
|------------|--------------|
| `20_cardio_cases_raw_data_in_csv.csv` | Structured CSV file containing 20 cardiology case notes. Each row represents one patient episode covering admission to discharge. |
| `20_cardio_cases_raw_data_in_jsonl.jsonl` | Same dataset converted to **JSONL format** (Doccano-compatible) for direct import during annotation. Each line is a single case note record. |

---

## ⚙️ Dataset Specifications

| Attribute | Details |
|------------|----------|
| **Number of Cases** | 20 |
| **Medical Specialty** | Cardiology |
| **Language** | English |
| **Data Type** | Clinical text narratives (EHR-style) |
| **Structure** | Admission → Investigations → Treatment → Discharge Summary |
| **Anonymization** | All personally identifiable information (PII) has been fully removed |
| **Source Format** | Text manually transcribed and preprocessed for annotation consistency |

---

## 🧩 Example Schema (JSONL)

```json
{"text": "Patient admitted with acute chest pain radiating to the left arm. ECG shows ST elevation in leads V2–V6."}
💡 Usage Notes

The CSV file is ideal for quick inspection (Excel / Pandas).

The JSONL file should be used for Doccano imports and NLP preprocessing pipelines.

Each record corresponds to a single patient case note, containing rich medical language suitable for Named Entity Recognition (NER) tasks.

🩺 Context

This dataset is part of the
👉 20_Cardio_Cases_NLP_Project

within the Cardiology module of
👉 ClinicalCaseNotesEHRs
 under the
👉 Natural_Language_Processing
 component of
the Medical-AI-Data-Annotation
 repository.

⭐ Maintained by drpradeepAI
 — Medical AI Data Annotator & Clinical NLP Specialist.
