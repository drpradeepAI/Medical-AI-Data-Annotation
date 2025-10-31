# 🫀 Cardiology Clinical Case Notes — Annotated EHR Dataset

This folder contains the **Cardiology module** of the *Clinical Case Notes (EHR)* series — a structured, manually annotated medical NLP dataset created using **[Doccano](https://github.com/doccano/doccano)**.  
It comprises **20 Electronic Health Record (EHR)** case notes annotated by a **medical professional (MBBS Doctor)** for use in **clinical NLP, AI model training, and medical information extraction research.**

---

## 📘 Dataset Overview

Each case represents a real-world styled **clinical episode**, encompassing:
- Patient presentation and admission details  
- Clinical investigations and procedures  
- Diagnosis and treatment plans  
- Follow-up or discharge summary  

The dataset is meticulously annotated using a **36-label medical entity schema** developed specifically for healthcare NLP applications.

---

## 📁 Folder Structure

| Folder / File | Description |
|----------------|--------------|
| `20_cardio_cases_NLP_project/` | Contains all files related to the 20 annotated cardiology cases. |
| ┣ 📄 `raw_data/` | Original unannotated case texts (CSV & JSONL formats). |
| ┣ 📄 `annotated_data/` | Final Doccano export files with entity annotations. |
| ┣ 📄 `label_schema/` | 36-label schema (`label_config_36_final.json`) defining all medical entities and color mappings. |
| ┣ 📄 `metadata/` | Structured metadata (`.csv` and `.json`) linking all raw and annotated cases. |
| ┣ 📄 `screenshots/` | Visual workflow proof (Doccano project setup, labeling, and export stages). |
| 📜 `README.md` | Overview documentation for this Cardiology dataset module. |

---

## ⚙️ Annotation Details

| Parameter | Description |
|------------|--------------|
| **Tool Used** | Doccano (v1.x) |
| **Annotation Type** | Named Entity Recognition (NER) |
| **Entity Schema** | 36 predefined medical entity labels |
| **Data Format** | JSON / JSONL |
| **Language** | English |
| **Cases Annotated** | 20 Cardiology case notes |
| **Anonymization** | All identifiable details removed |

---

## 🧩 Example Entity Types (from 36-label schema)

| Category | Examples |
|-----------|-----------|
| **Symptoms** | Chest pain, breathlessness, palpitations |
| **Tests / Results** | ECG, Troponin, Echo findings |
| **Diagnoses** | Myocardial infarction, cardiomyopathy |
| **Medications** | Aspirin, Clopidogrel, Atorvastatin |
| **Procedures** | Angioplasty, CABG, ECHO |
| **Follow-up / Advice** | Lifestyle modification, cardiac rehab |

---

## 🧠 Applications

This dataset is designed for:
- **Clinical NLP model training** (NER, relation extraction, summarization)  
- **AI-assisted EHR analytics and research**  
- **Medical text classification and ontology development**  
- **Educational use** in biomedical data science and AI for healthcare  

---

## 🩺 About the Creator

**Dr. Pradeep (drpradeepAI)**  
MBBS Doctor • Medical AI Data Annotator • Clinical NLP Specialist  

- Experienced in **medical data curation**, **NLP schema design**, and **AI-based text annotation workflows**.  
- Focused on building open, transparent, and reusable **medical AI datasets** that bridge healthcare and technology.  
- Repository: [Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)

---

## 🔗 Context in Repository

This Cardiology dataset is part of the  
👉 **[`ClinicalCaseNotesEHRs`](../README.md)** project under  
👉 **[`Natural_Language_Processing`](../../../README.md)** within the  
**[Medical-AI-Data-Annotation](https://github.com/drpradeepAI/Medical-AI-Data-Annotation)** repository.

---

⭐ *A foundational dataset for advancing healthcare NLP — developed by a practicing physician bridging medicine and machine intelligence.*
