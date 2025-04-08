# A Collaborative End-to-End Medical Algorithmic Audit of TriageAssist 

PREPARED FOR
+ Dr. AJung Moon, PhD (ajung.moon@mcgill.ca)
CEO, Prioritize™


PREPARED BY VANTAMED+
+ Miguel Ángel Carrillo Cobián (miguel.carrillocobian@mail.mcgill.ca), Responsible AI Auditor	                                                                
+ Leah Davis (leah.davis@mail.mcgill.ca), Responsible AI Auditor		

## Overview

This repository presents the results of an AI ethics audit of **TriageAssist**, a clinical decision support system developed by **Prioritize™**, designed to assist emergency room clinicians in triaging cardiovascular disease (CVD) cases. The audit was conducted by **Vantamed+**, an independent AI ethics consultancy, as part of McGill University’s **ECSE681 – Responsible AI** course.

TriageAssist is currently in a pilot deployment phase, with the goal of broader adoption in clinical environments. Given the high-stakes nature of emergency care and the known disparities in heart disease presentation and treatment between demographic groups—particularly biological sex—this audit focused on fairness, safety, and transparency.

## Repository Contents

### 📁 `TriageAssist_Audit_Code.ipynb`

This Jupyter Notebook contains the full technical audit pipeline and is organized into the following key sections:

- Exploratory Data Analysis (EDA) on heart disease data  
- Creation of Classification Models & Subgroup Testing
- Exploratory Error Analysis
- Adversarial Testing
- Reweighting
- Visualizations and recommendations  

### 📁 `heart.csv`
- Contains 918 anonymized patient records with 12 clinical and demographic attributes.
- Used as the core dataset for model training and evaluation. 
- [Source dataset on Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

### 📁 `Use Case 1 - TriageAssist.pdf`
- Detailed real-world deployment scenario of TriageAssist in a Montreal hospital.
- Includes rich qualitative insights through interviews with nurses, doctors, and a patient.
- Provides a socio-technical and ethical framing for the audit.

### 📁 `ECSE681 W2025 Final Project.pdf`
- Official project brief for the Responsible AI course at McGill University.
- Outlines audit objectives, context, scope, deliverables, and grading rubric.
- Frames the role of the student audit team as an AI ethics consultancy advising a real-world deployment.

## Running `TriageAssist_Audit_Code.ipynb`

To run the notebook successfully in your local environment, please ensure the following:

### ⚠️ Important Notes
- **Do not run the first code cell** unless you're using **Google Colab**, as it contains Colab-specific setup.
- **Adjust the path to the dataset** (`heart.csv`) in the second code cell to match your local file structure if necessary.

### 📦 Required Libraries
Make sure you have the following Python packages installed:

- `aif360`
- `google` (if using Google Colab)
- `matplotlib`
- `numpy`
- `pandas`
- `pathlib`
- `seaborn`
- `shap`
- `scikit-learn`

You can install them all at once using:

```bash
pip install aif360 google matplotlib numpy pandas seaborn shap scikit-learn
```
---

## Credits

- **Audit Team:**
    + Miguel Ángel Carrillo Cobián (miguel.carrillocobian@mail.mcgill.ca), Responsible AI Auditor	                                                                
    + Leah Davis (leah.davis@mail.mcgill.ca), Responsible AI Auditor	 

- **Course:** ECSE681 – Responsible AI, McGill University  

- **Instructor:** Dr. AJung Moon  

- **Use case developed by:** Shalaleh Rismani  

- **Dataset Source:** [Kaggle - Heart Failure Prediction](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)  
