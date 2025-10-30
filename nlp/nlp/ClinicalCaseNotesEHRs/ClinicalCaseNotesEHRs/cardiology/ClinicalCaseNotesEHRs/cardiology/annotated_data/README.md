# 🧠 Annotated Data – Cardiology Clinical Case Notes

This folder contains the **final annotated dataset** for 20 cardiology electronic health record (EHR) cases.  
All annotations were performed manually using **Doccano**, following a structured 36-label entity schema designed for medical NLP tasks.

---

## 📂 File Description

| File | Description |
|------|--------------|
| `20 cardio cases annotated data in jsonl.jsonl` | Exported Doccano annotations in JSONL format. Each line represents one annotated case note with named entities tagged for NLP model training. |

---

## 🧩 Annotation Details

- **Annotation Tool:** Doccano (v1.x)  
- **Annotation Type:** Named Entity Recognition (NER)  
- **Format:** JSONL (Doccano export format)  
- **Labels Used:** 36 medical entity labels (see `label_schema/label_config_36_final.json`)  
- **Number of Cases:** 20  
- **Language:** English  
- **Annotator:** Dr. Pradeep (drpradeepAI)

---

## 🧠 Data Schema Example

Below is a simplified example of the JSONL structure:

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
