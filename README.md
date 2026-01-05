# 🌬️ RESPIRA: Asthma Risk Prediction System

**Empowering You to Breathe Easier with AI-Driven Insights.**

---

## 📖 Introduction

**RESPIRA** is an innovative AI-powered system designed to predict the risk of asthma exacerbation based on personal health metrics and real-time environmental data. By combining patient history with pollution levels, RESPIRA provides personalized risk assessments and actionable health advice, helping individuals take proactive control of their respiratory health.

Whether you are a patient looking to manage your condition or a healthcare provider seeking data-driven insights, RESPIRA bridges the gap between environmental exposure and personal well-being.

## ✨ Key Features

*   **🤖 Advanced ML Model:** Utilizes a Random Forest Regressor to analyze complex relationships between health factors and air quality.
*   **🌍 Real-time Environmental Integration:** Considers critical pollutants like PM2.5, NO2, and Ozone (O3) alongside Air Quality Index (AQI) data.
*   **📊 Interactive Dashboard:** A user-friendly **Streamlit** web interface allows users to input their data and view instant risk predictions.
*   **📱 Mobile Ready:** Includes components for an Android application to bring risk assessment to your fingertips (see `RESPIRA/` folder).
*   **🛡️ Actionable Advice:** Provides specific recommendations based on the predicted risk score, such as wearing masks or using air purifiers.

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

## 🔄 Workflow

1.  **Data Ingestion:** The system aggregates data from multiple sources:
    *   *Patient Data:* Age, BMI, Smoking Status, Lung Function (FEV1).
    *   *Environmental Data:* PM2.5, NO2, Ozone levels, and AQI from global datasets.
2.  **Preprocessing & Feature Engineering:**
    *   Data cleaning and imputation of missing values.
    *   Calculation of composite indices like `Pollution_Index` and `Health_Risk_Score`.
3.  **Model Training:**
    *   A Random Forest model is trained to predict the Health Risk Score based on the engineered features.
4.  **Prediction Interface:**
    *   The Streamlit app accepts user inputs.
    *   The model processes these inputs to output a risk score and probability.
5.  **Guidance:**
    *   The system displays the diagnosis and suggests preventive measures.

## 🚀 How to Run (Prototype)

The core logic resides in the Jupyter Notebook `Asthma Risk Prediction AI Model`. To run the Streamlit interface directly:

1.  **Prerequisites:** Ensure you have Python installed with the necessary libraries (`streamlit`, `pandas`, `scikit-learn`, `joblib`).
2.  **Launch the App:**
    ```bash
    streamlit run "Asthma Risk Prediction AI Model"
    ```
    *(Note: You may need to extract the Python script from the notebook or convert it to a `.py` file first).*

## 📂 Project Structure

*   `Asthma Risk Prediction AI Model`: The main Jupyter Notebook containing data processing, model training, and the Streamlit app code.
*   `RESPIRA/`: Directory containing artifacts for the Android mobile application.
*   `asthma_prediction_model.pkl`: The serialized trained Machine Learning model.

---

*Breathing life into data for a healthier tomorrow.* 🍃
