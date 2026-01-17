
# Unsupervised Anomaly Detection

## 📌 Project Overview
This project focuses on detecting anomalies in industrial sensor data using **unsupervised machine learning techniques**.  
The objective is to identify unusual patterns or abnormal machine behavior without using labeled failure data.

The project applies **statistical preprocessing**, **dimensionality reduction**, and **multiple anomaly detection algorithms** to validate results.

---

## 📊 Dataset
- **Dataset:** AI4I 2020 Predictive Maintenance Dataset
- **Source:** Kaggle
- **Description:** Industrial sensor readings including temperature, rotational speed, torque, and tool wear.
- **Note:** The dataset is not uploaded to this repository. Please download it from Kaggle and upload it manually when running the notebook.

---

## 🛠️ Techniques Used
- Data Cleaning and Feature Selection
- Feature Scaling (StandardScaler)
- Principal Component Analysis (PCA) for dimensionality reduction
- **Isolation Forest** for anomaly detection
- **Local Outlier Factor (LOF)** for density-based anomaly detection
- Model comparison and overlap analysis
- Visualization of anomalies using PCA components

 Example:
```python
from sklearn.ensemble import IsolationForest
model = IsolationForest(contamination=0.05)

---

## 📈 Results
- Both Isolation Forest and LOF detected approximately **5% anomalous observations**
- **156 data points** were identified as anomalies by both models, indicating consistent detection
- PCA visualization helped clearly separate normal and anomalous observations

---

## 💻 Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## ▶️ How to Run
1. Download the dataset from Kaggle (AI4I 2020)
2. Upload the CSV file when running the notebook in Google Colab
3. Run all cells in order to reproduce the results

---

## 🎯 Learning Outcomes
- Understanding unsupervised anomaly detection
- Practical use of PCA for visualization
- Comparing multiple anomaly detection algorithms
- Gaining experience with real-world industrial data

---

## 📌 Author
**Anshika Rawat**
MCA Student (Machine Learning & AI – upcoming specialization)  
Aspiring Data Analyst / ML Analyst

## 📌 Disclaimer

This project was developed for **learning and academic purposes**.  
It demonstrates the application of unsupervised machine learning techniques and does not represent a production-level industrial deployment.
