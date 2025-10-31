# 🧠 Annotated Data — Cardiology Clinical Case Notes

This folder contains the **final manually annotated dataset** for **20 cardiology Electronic Health Record (EHR)** cases.  
Annotations were performed using **[Doccano](https://github.com/doccano/doccano)**, following a standardized **36-label medical entity schema** optimized for **clinical NLP model training and evaluation**.

---

## 📂 File Description

| File Name | Description |
|------------|--------------|
| `20_cardio_cases_annotated_data_in_jsonl.jsonl` | Final Doccano export file containing 20 annotated cardiology case notes. Each line represents one EHR entry with entities labeled for NER model development. |

---

## ⚙️ Annotation Specifications

| Parameter | Details |
|------------|----------|
| **Tool Used** | Doccano (v1.x) |
| **Annotation Type** | Named Entity Recognition (NER) |
| **Export Format** | JSONL |
| **Entity Schema** | 36-label schema (`label_schema/label_config_36_final.json`) |
| **Cases Annotated** | 20 Cardiology Case Notes |
| **Language** | English |
| **Annotator** | [drpradeepAI](https://github.com/drpradeepAI) |

---

## 🧩 Example JSONL Structure

A simplified view of one annotated record:

```json
{
  "id": 1,
  "text": "The patient was admitted with chest pain radiating to the left arm. ECG showed ST elevation in V2-V6.",
  "entities": [
    [27, 37, "Symptom"],
    [59, 79, "Test_Name"],
    [80, 87, "Test_Result"]
  ]
}
💡 Key Highlights

Granular medical entity tagging for clinical text intelligence

Schema aligned with medical terminology for AI/NLP standardization

Quality checked manually for entity accuracy and context relevance

Interoperable format (JSONL) compatible with major ML frameworks

🩺 Context

This dataset is part of the
👉 20_Cardio_Cases_NLP_Project

within the Cardiology domain of
👉 ClinicalCaseNotesEHRs
 under the
👉 Natural_Language_Processing
 module of
the Medical-AI-Data-Annotation
 repository.

⭐ If you use this dataset or structure for your own projects, please credit drpradeepAI.
