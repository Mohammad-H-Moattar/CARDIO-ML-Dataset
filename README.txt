CARDIO-ML: A Multi-modal Clinical ECG Dataset for Machine Learning
Overview
The CARDIO-ML Dataset is a comprehensive, multi-modal collection designed to bridge the gap between electrocardiogram (ECG) signal data and rich clinical context. It integrates high-quality ECG recordings in image format with extensive, structured clinical data from 574 patients, supporting the development of robust, clinically-aware machine learning models in cardiology.
This dataset addresses key limitations in existing resources by providing:
•	Demographic Diversity: Ages 6 to 98 years.
•	Clinical Richness: Over 11 tables of clinical data, including vital signs, laboratory results, medical history, and patient outcomes.
•	High-Quality Annotations: ECG signals labeled via a dual-expert consensus process by board-certified cardiologists and emergency medicine physicians.
•	Real-World Relevance: Collected from routine clinical workflows at two major academic medical centers.
Dataset Download
Due to size constraints, the complete dataset is hosted externally:
https://drive.google.com/drive/folders/1u1jzVb8r2Rekel5BSrZ2moNMh-56DKiL?usp=drive_link
Dataset Structure
The dataset is organized into the following main directories and files:
text
CARDIO-ML_Dataset/
│
├── ECGS
│   
├── Clinical_Data/
│   ├── 01_Core_Patient_Data.csv
│   ├── 02_Diagnosis_Treatment_Summary.csv
│   ├── 03_Emergency_Admission_Metrics.csv
│   ├── 04_Complete_Blood_Count.csv
│   ├── 05_Metabolic_Panel_Cardiac_Enzymes.csv
│   ├── 06_Inflammatory_Markers.csv
│   ├── 07_Coagulation_Profile.csv
│   ├── 08_Urinalysis.csv
│   ├── 09_Arterial_Blood_Gas.csv
│   └── 10_Comprehensive_Medical_History.csv
└── README.md (This file)
Clinical Data Tables Description
File Name	Description
01_Core_Patient_Data.csv	Central table with demographics, vitals, core lab results, and outcomes.
02_Diagnosis_Treatment_Summary.csv	Patient's clinical pathway from initial complaint to final diagnosis and treatment.
03_Emergency_Admission_Metrics.csv	Triage information and initial vital signs at emergency department admission.
04_Complete_Blood_Count.csv	Complete Blood Count (CBC) with differential results.
05_Metabolic_Panel_Cardiac_Enzymes.csv	Basic metabolic panel and cardiac enzyme tests (e.g., Troponin-I).
06_Inflammatory_Markers.csv	ESR and CRP test results.
07_Coagulation_Profile.csv	PTT, PT, and INR test results.
08_Urinalysis.csv	Complete urinalysis results.
09_Arterial_Blood_Gas.csv	Arterial Blood Gas (ABG) analysis results.
10_Comprehensive_Medical_History.csv	Patient's long-term health background.
Data Processing
The ECG signals underwent a rigorous preprocessing pipeline:
1.	Scanning: High-resolution digitization of paper-based ECG traces.
2.	Grid Removal: Isolation of the clean ECG waveform from the background grid.
3.	Quality Control: Manual removal of low-quality or distorted images.
4.	Normalization & Enhancement: Size normalization, binarization, noise reduction, and contrast enhancement.
5.	Cropping: Images were cropped to include at least four consecutive heartbeats.
Dataset Statistics
•	Total Patients: 574
•	Age Range: 6 - 98 years (Mean: 51.33 ± 18.03)
•	Gender Distribution: Male (M) / Female (F)
•	ECG Recordings: 12-lead, image format (PNG)
•	Clinical Variables: 150+ parameters across 11 data tables
•	Annotation Method: Dual-expert consensus (Cardiologist + Emergency Physician)
Potential Use Cases
•	Multi-modal Machine Learning: Fuse image-based ECG data with tabular clinical data.
•	Arrhythmia Detection: Develop and benchmark classification models.
•	Clinical Outcome Prediction: Predict mortality, hospitalization risk, or disease progression.
•	Biomedical Signal Processing: Test novel ECG signal analysis and computer vision techniques.
•	Educational Tool: Teach concepts in cardiology, data science, and medical informatics.
Limitations
•	Imbalanced Labels: Some cardiac conditions are represented by fewer samples.
•	Image-Based ECGs: The dataset contains processed images rather than raw signal waveforms, which may limit certain signal processing applications.
•	Retrospective Data: Collected from clinical records, with inherent limitations of retrospective studies.
License and Citation
License
This dataset is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). You are free to share and adapt the material for any purpose, even commercially, provided you give appropriate credit.
Contributing
We welcome contributions from the community! Please feel free to:
•	Report bugs or suggest enhancements by opening an issue
•	Submit pull requests for improvements to the code or documentation
•	Share your research outcomes using this dataset
Contact and Support
For questions, collaboration inquiries, or to report issues, please contact:
•	Corresponding Author: Mohammad Hossein Moattar - mhmoattar@iau.ac.ir
Acknowledgments
We extend our gratitude to:
•	The medical staff of 22 Bahman Hospital and Ghaem Hospital, Mashhad, Iran.
•	The cardiologists and emergency physicians who provided expert annotations.
•	The data curation team for their meticulous work in preparing this dataset.

