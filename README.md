# BW Predict – Birth Weight Prediction System

## Project Overview
BW Predict is an academic project focused on predicting fetal birth weight using clinical maternal data and ultrasound measurements.  
The system is designed as a web-based clinical decision support tool that integrates a modern MVC architecture with a machine learning model.

This project was developed as part of an academic course and is not intended for clinical deployment.

---

## System Architecture
The system follows a Client–Server MVC architecture:

- **View (Frontend)**: Vue.js  
  Provides a responsive user interface for medical staff to enter maternal and fetal data and view prediction results.

- **Controller (Backend)**: Node.js  
  Handles API requests, validates clinical data, and communicates with the machine learning engine.

- **Model (ML Engine)**: Python  
  Implements a Random Forest regression model for fetal birth weight prediction.

---

## Machine Learning Approach
- **Algorithm**: Random Forest Regressor  
- **Explainability**: SHAP (SHapley Additive exPlanations)  
- **Input Data**:
  - Maternal data (age, BMI, gestational age, medical background)
  - Ultrasound biometry (HC, AC, FL)
- **Output**:
  - Predicted birth weight (grams)
  - Confidence interval
  - Feature contribution explanations

---

## Database Design
The database schema is designed to support prediction tracking and model evaluation:

- **User** – medical staff member
- **Prediction** – metadata and predicted weight
- **MaternalData** – clinical input features
- **BirthOutcome** – actual birth weight and prediction deviation

---

## Repository Contents
- `Detailed Design- niv and oran.docx` – Full system detailed design  
- `README.md` – Project overview and documentation  
- UML diagrams – Class and sequence diagrams (if included in repository)

---

## Academic Note
This repository contains documentation and design artifacts only.  
No real patient data is included.  
The project is intended solely for academic and educational purposes.

