# 🧩 Label Schema – 36-Label Configuration for Cardiology EHR Annotation

This folder contains the **label configuration file** used during manual annotation of 20 cardiology electronic health record (EHR) case notes in *Doccano*.

The schema defines the complete list of medical entity types, their display colors, and category hierarchy, ensuring consistent tagging across all annotations.

---

## 📂 File Description

| File | Description |
|------|--------------|
| `20cardio case label_config_36 in json.json` | Doccano label configuration file containing 36 predefined medical entity labels with color and shortcut settings. |

---

## 🧠 Purpose

This label configuration file was imported into **Doccano** before annotation began.  
It ensures **standardized entity labeling** across cases and supports future reuse for other clinical specialties.

---

## ⚙️ Technical Details

- **File Format:** JSON  
- **Compatible Tool:** Doccano (v1.x or later)  
- **Schema Version:** v36_labels_final  
- **Label Count:** 36  
- **Structure Example:**

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
  ...
]
