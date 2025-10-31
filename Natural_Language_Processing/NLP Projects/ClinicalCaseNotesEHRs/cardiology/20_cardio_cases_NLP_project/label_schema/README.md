# 🧩 Label Schema — 36-Label Configuration for Cardiology EHR Annotation

This folder contains the **Doccano label configuration file** used during manual annotation of **20 cardiology Electronic Health Record (EHR)** case notes.  
The schema defines a standardized set of **36 medical entity labels** with assigned colors, shortcuts, and categories — ensuring annotation consistency, reproducibility, and cross-specialty compatibility.

---

## 📁 File Description

| File Name | Description |
|------------|--------------|
| `20cardio_case_label_config_36_in_json.json` | Doccano-compatible configuration file defining 36 medical entity labels, their color mappings, and shortcut keys for efficient tagging. |

---

## 🧠 Purpose

The label configuration file was imported into **[Doccano](https://github.com/doccano/doccano)** before annotation to establish a consistent annotation protocol.  
It enables:
- Uniform entity definitions across annotators  
- Schema portability for future **multi-specialty clinical NLP projects**  
- Simplified re-annotation and model retraining  

---

## ⚙️ Technical Specifications

| Parameter | Details |
|------------|----------|
| **Format** | JSON |
| **Tool Compatibility** | Doccano (v1.x and later) |
| **Schema Version** | `v36_labels_final` |
| **Entity Count** | 36 |
| **Entity Hierarchy** | Clinical categories grouped under Symptoms, Diagnoses, Investigations, Medications, Procedures, etc. |

---

## 🧩 Example Schema Structure

```json
[
  {
    "id": 1,
    "text": "Symptom",
    "prefix_key": "s",
    "background_color": "#FFD700"
  },
  {
    "id": 2,
    "text": "Diagnosis",
    "prefix_key": "d",
    "background_color": "#FF8C00"
  },
  {
    "id": 3,
    "text": "Medication_Name",
    "prefix_key": "m",
    "background_color": "#90EE90"
  }
]
🩺 Schema Design Highlights

36 curated medical entities aligned with clinical text ontology

Optimized for Named Entity Recognition (NER) tasks in healthcare NLP

Designed for cross-department reuse (Cardiology, Neurology, Pulmonology, etc.)

Follows non-overlapping entity rule for Doccano compatibility

🔗 Repository Context

This schema supports the
👉 20_Cardio_Cases_NLP_Project

within the Cardiology domain of
👉 ClinicalCaseNotesEHRs
 under
👉 Natural_Language_Processing

in the Medical-AI-Data-Annotation
 repository.

⭐ Maintained by drpradeepAI
 — Medical AI Data Annotator,MBBS Doctor & Clinical NLP Specialist.
