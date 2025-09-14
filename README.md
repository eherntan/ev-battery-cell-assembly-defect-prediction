# EV-Battery-Cell-Assembly-Defect-Prediction
This project simulates the Lamination process in EV battery cell assembly. This project demonstrates how machine learning can support process engineers by predicting defect likelihood and highlighting the most critical process parameters.Achieved **73%accuracy**, with **71% recall on OK cells** and **76% recall on defective cells**. Identified opportunities to improve **defect detection recall** using class balancing (SMOTE, weighted loss).

## Features Simulated
- **Lamination Temperature (°C)**  
- **Lamination Pressure (N)**  
- **Short-side Sealer Temperature (°C)**  
- **Long-side Sealer Temperature (°C)**  
- **Short-side Sealer Pressure (N)**  
- **Long-side Sealer Pressure (N)**  
- **Heater Temperature (°C)**  

These features were generated as **synthetic data** using normal distributions around typical process windows (5,000 samples).  
Defect probability was modeled using engineering logic — e.g., low sealing temperature or low lamination pressure increases defect risk.  

---

## Machine Learning Approach
- Generated **synthetic dataset** with domain-informed defect logic.  
- Built and trained classification models:
  - **Random Forest Classifier**  
- Evaluated models using:
  - **Classification Report** (precision, recall, F1-score)   
  - **Feature Importance Analysis**  

---

## Key Results
- Achieved **73% prediction accuracy** on test data.  
- **Feature Importance Analysis** confirmed lamination temperature is the critical defect driver **(~30%)**

---

## Tech Stack
- Python  
- NumPy, Pandas  
- scikit-learn  
- Matplotlib, Seaborn  
