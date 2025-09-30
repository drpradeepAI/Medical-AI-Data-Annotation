# MI Case 001 – Cardiology

This folder contains the **raw clinical case note**, the **label schema**, 
and the **final annotated export** for a cardiology case.  
Annotations were done manually using [Doccano](https://github.com/doccano/doccano).

---

## Folder Structure

- `raw/`  
  Contains the **original clinical case note** before annotation.

- `labels/`  
  Defines the **entity schema** used in annotation (Diagnosis, Symptom, Sign, 
  Procedure, Test Result, Medication).

- `annotated/`  
  Contains the **final annotated file** (exported from Doccano in JSONL format), 
  which can be used directly for training NLP models.

---

## Usage

- Use `annotated/` for **NER model training** or data analysis.  
- Use `labels/` for **entity mapping** during preprocessing.  
- Keep `raw/` for **reference and reproducibility**.

---

## Notes
- This is the **first annotated case (Cardiology)** in the clinical notes series.  
- More cases across different specialties will be added in similar folder structures.
