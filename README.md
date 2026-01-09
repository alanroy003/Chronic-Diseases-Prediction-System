# Chronic Diseases Prediction System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn%20%7C%20XGBoost-orange)

<div align="center">
  <img src="Multiple-Disease-Prediction-Webapp-main/img/image.png" alt="App Screenshot" width="800"/>
</div>

## 📋 Overview

This project is a comprehensive **Machine Learning-based web application** designed to predict the likelihood of various chronic diseases. Built using **Streamlit**, it offers a user-friendly interface where users can input symptoms or specific medical parameters to receive instant risk assessments. The system aggregates multiple predictive models to cover a wide spectrum of health conditions.

## 🚀 Features

The application supports prediction for the following 10 conditions:

1.  **🧬 Multiple Disease Prediction (General):** Predicts a disease based on a list of selected symptoms using an XGBoost model.
2.  **🍬 Diabetes Prediction:** Estimates risk based on parameters like Glucose, BMI, Insulin, etc.
3.  **❤️ Heart Disease Prediction:** Analyzes cardiovascular risk factors (Chest Pain, BP, Cholesterol, etc.).
4.  **🧠 Parkinson's Disease Prediction:** Uses vocal measurements (MDVP, Jitter, Shimmer) for detection.
5.  **🫁 Lung Cancer Prediction:** Considers lifestyle factors like smoking, alcohol, and symptoms like coughing.
6.  **🥃 Liver Disease Prediction:** Analyzes liver function tests (Bilirubin, Albumin, Proteins).
7.  **🦠 Hepatitis Prediction:** Based on blood markers and demographics.
8.  **⚠️ Jaundice Prediction:** Evaluates bilirubin levels and other markers.
9.  **🧪 Chronic Kidney Disease Prediction:** Uses indicators like blood pressure, specific gravity, and blood tests.
10. **🎀 Breast Cancer Prediction:** Analyzes cell nucleus features (radius, texture, perimeter, etc.).

## 🛠️ Technologies Used

- **Language:** Python
- **Frontend:** Streamlit
- **ML Libraries:** Scikit-learn, XGBoost
- **Data Processing:** Pandas, NumPy
- **Visualization:** Plotly, Matplotlib, Seaborn
- **Model Handling:** Joblib, Pickle

## 💻 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python Package Manager)

### Steps

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/alanroy003/Chronic-Diseases-Prediction-System.git
    cd Chronic-Diseases-Prediction-System
    ```

2.  **Install dependencies:**

    ```bash
    pip install streamlit pandas numpy scikit-learn xgboost plotly matplotlib seaborn streamlit-option-menu
    ```

3.  **Run the Application:**
    Navigate to the directory containing the main application file.

    ```bash
    cd Multiple-Disease-Prediction-Webapp-main
    streamlit run app.py
    ```

## 📖 Usage

1.  Launch the app using the command above.
2.  Use the **Sidebar** to navigate between different prediction modules.
3.  **General Disease Prediction:**
    - Select your symptoms from the dropdown list.
    - Click "Predict" to see the result and probability.
4.  **Specific Diseases:**
    - Enter the required medical values (e.g., Age, BMI, Blood Pressure) into the input fields.
    - Click the result button.
5.  View the prediction result (Positive/Negative) along with precautions or descriptions where available.

## 📂 Project Structure

```text
Chronic-Diseases-Prediction-System/
├── Multiple-Disease-Prediction-Webapp-main/
│   ├── app.py                  # Main Streamlit application with all disease modules
│   ├── img/
│   │   └── image.png           # Application screenshot
│   ├── code/
│   │   ├── DiseaseModel.py     # Class for handling the general disease model
│   │   ├── helper.py           # Helper functions (e.g., symptom array preparation)
│   │   └── train.py            # Script to train the XGBoost model
│   ├── data/                   # Datasets used for training
│   ├── models/                 # Pre-trained .sav and .json models
│   └── ...
├── app.py                      # Simplified version of the app
├── README.md                   # Project documentation
└── ...
```

## Disclaimer

This system is for educational and informational purposes only. It is **not** a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.

## Credits

Developed by Alan Roy.
