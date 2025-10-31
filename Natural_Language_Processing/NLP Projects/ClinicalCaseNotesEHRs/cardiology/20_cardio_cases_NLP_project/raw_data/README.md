# 📄 Raw Data – Cardiology Clinical Case Notes

This folder contains the **original unannotated EHR case notes** used as input for medical NLP annotation in Doccano.

---

## 📂 Files Description

| File | Description |
|------|--------------|
| `20 cardio cases raw data in csv.csv` | Raw text data for 20 cardiology case notes stored in CSV format. Each row represents one complete patient episode from admission to discharge. |
| `20 cardio cases raw data in jsonl.json` | Same dataset converted to JSONL format (Doccano-compatible). Used directly for import into Doccano annotation tool. |

---

## 🧠 Data Overview
- **Number of cases:** 20  
- **Specialty:** Cardiology  
- **Structure:** Admission notes → Investigations → Procedures → Discharge summary  
- **Language:** English  
- **Anonymization:** All personally identifiable information (PII) removed.

---

## 🧩 Usage Notes
- The CSV file is meant for readability and tabular viewing (e.g., Excel, Pandas).  
- The JSONL file follows the Doccano import schema:
  ```json
  {"text": "Patient admitted with acute chest pain..."}
