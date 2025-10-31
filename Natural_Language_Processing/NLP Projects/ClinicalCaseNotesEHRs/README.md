# 🩺 Clinical Case Notes (EHRs) — Medical NLP Annotation Dataset

This folder contains **specialty-wise annotated Electronic Health Record (EHR)** case notes curated for **medical NLP research and AI model development**.  
Each case represents a complete clinical narrative — from **admission to discharge**, encompassing history, examination, investigation, diagnosis, treatment, and follow-up details.

All annotations are created manually by a **medical professional (MBBS Doctor)** using **[Doccano](https://github.com/doccano/doccano)** and follow a **36-label clinical entity schema** standardized across specialties.

---

## 🧠 Dataset Overview

- 📋 **Type:** Clinical text dataset (EHR case notes)  
- 💬 **Language:** English  
- ⚙️ **Annotation Type:** Named Entity Recognition (NER)  
- 🧩 **Schema:** 36 predefined medical entity labels  
- 🔐 **PII:** All personal identifiers are removed (fully anonymized)  
- 🧑‍⚕️ **Annotated By:** Dr. Pradeep (MBBS Doctor | Medical AI Data Annotator)

---

## 📁 Folder Structure

| Folder / File | Description |
|----------------|-------------|
| `cardiology/` | Contains 20 fully annotated Cardiology case notes, metadata, schema, and documentation. |
| *(Upcoming)* `neurology/` | To include annotated cases of neurological disorders. |
| *(Upcoming)* `pulmonology/` | To include respiratory disease EHR annotations. |
| *(Upcoming)* `oncology/` | Planned dataset for oncology-related case notes. |
| `README.md` | Overview and structure of the Clinical Case Notes dataset series. |

---

## 🩹 Annotation Standards

| Aspect | Details |
|--------|----------|
| **Tool Used** | Doccano (v1.x) |
| **Annotation Type** | NER (Named Entity Recognition) |
| **Entity Schema** | 36-label medical schema (`label_config_36_final.json`) |
| **Output Format** | JSONL (Doccano export) |
| **Annotation Quality Control** | Manual review and validation for each case |
| **Version Control** | Managed under Git for transparency and reproducibility |

---

## 🧩 Example Entity Categories

| Category | Examples |
|-----------|-----------|
| **Symptoms** | Chest pain, headache, cough, fever |
| **Tests & Results** | ECG, MRI, X-ray, HbA1c, Echocardiogram |
| **Diagnoses** | Myocardial infarction, diabetes mellitus, pneumonia |
| **Medications** | Aspirin, Insulin, Paracetamol |
| **Procedures** | Angioplasty, Biopsy, Intubation |
| **Follow-up & Advice** | Lifestyle modification, rehabilitation, review after 1 month |

---

## 📊 Current Coverage

| Specialty | Cases | Status | Annotation Level |
|------------|--------|---------|------------------|
| 🫀 **Cardiology** | 20 | ✅ Completed | Full 36-label entity tagging |
| 🧠 **Neurology** | – | ⏳ In Progress | Planned |
| 🌬️ **Pulmonology** | – | ⏳ Planned | Planned |
| 🧬 **Oncology** | – | ⏳ Planned | Planned |

---

## 🧭 Purpose and Use

This dataset collection is built for:
- Training and evaluating **clinical NLP models**  
- Supporting **medical entity recognition, relation extraction, and summarization** tasks  
- Enabling **AI-assisted healthcare analytics and clinical decision support research**  
- Providing **open, reusable resources** for interdisciplinary researchers bridging medicine and AI  

---

## 👨‍⚕️ Created & Maintained By

**Dr. Pradeep (drpradeepAI)**  
MBBS Doctor • Medical AI Data Annotator • Clinical NLP Specialist
