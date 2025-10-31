# 🫀 Cardiology Clinical Case Notes (EHRs)

20 complete cardiology episodes (admission → discharge) annotated for medical NLP.

## Structure
- `raw_data/` – original unannotated cases (`.csv`, `.json`)
- `annotated_data/` – Doccano export (`.json`/`.jsonl`)
- `label_schema/` – `label_config_36_final.json` (36-label schema)
- `metadata.csv` – optional case summary
- `README.md`

## Annotation
- Tool: Doccano
- Type: NER (and usable for RE)
- Format: JSON/JSONL (Doccano)
- Coverage: complaints, HPI, meds, tests+results, procedures, dx, plan

## Screenshots
See `../screenshots/` for Doccano UI proofs.
