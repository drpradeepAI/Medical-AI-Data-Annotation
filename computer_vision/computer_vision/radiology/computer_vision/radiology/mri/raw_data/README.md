# MRI Raw Data

This folder contains original (unannotated) MRI scan images used for medical image annotation and AI model development.

📁 Folder Structure
raw_data/
├── 50_mri_brain_raw_data_images/        # Contains 50 brain MRI images (JPEG format)
├── 50_mri_brain_tumor_raw_data_jpg_format.zip  # Compressed archive of brain tumor MRI images
└── .keep
🧠 Dataset Description

Modality: MRI (Magnetic Resonance Imaging)

Regions Covered: Brain

Conditions Included: Normal brain and brain tumor samples

File Format: .jpg

Image Count: 50 uncompressed + 1 compressed ZIP archive

These images are used as raw inputs before annotation and model training.
They serve as the source data for the annotated datasets available in the annotated_data/ folder.

🔍 Use Cases

Image segmentation and classification model training

Brain tumor detection and diagnosis AI research

Preprocessing pipeline testing (e.g., normalization, contrast enhancement)

⚙️ Data Origin and Processing

Images were curated from publicly available open medical imaging datasets.

All images have been resized and renamed consistently for training readiness.

No annotations or labels are included in this folder.

📜 Licensing

This dataset is released under an Open Data License for educational and research purposes only.
Please ensure compliance with local data handling and privacy regulations when using medical data.
