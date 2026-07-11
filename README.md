# ❤️ Heart Disease Prediction App

A Machine Learning web application built using **Python, Streamlit, and SVM** that predicts the risk of Cardiovascular Disease based on patient health parameters.

## 📌 Project Overview
Cardiovascular diseases are one of the leading causes of death worldwide. Early detection can help in prevention and treatment. 
This project uses the Kaggle "Cardiovascular Disease Dataset" to train an SVM model and deploy it as an interactive Streamlit web app.

**Disclaimer**: This app is for educational/demonstration purposes only. It is NOT a medical diagnosis tool. Please consult a doctor for medical advice.

## ✨ Features
- User-friendly web interface using Streamlit
- Predicts LOW RISK / HIGH RISK of heart disease
- Shows probability percentage
- Takes 11 health parameters as input
- Uses StandardScaler for data preprocessing

## 🛠️ Tech Stack
- **Language**: Python 3.9+
- **Libraries**: pandas, numpy, scikit-learn, joblib, streamlit
- **Model**: Support Vector Machine (SVM) with StandardScaler
- **Dataset**: Cardiovascular Disease Dataset from Kaggle

## 📂 Dataset Features
| Feature | Description |
| --- | --- |
| Age | Age in years |
| Gender | 1 = Female, 2 = Male |
| Height | Height in cm |
| Weight | Weight in kg |
| Systolic BP | Systolic blood pressure |
| Diastolic BP | Diastolic blood pressure |
| Cholesterol | 1=Normal, 2=Above Normal, 3=Well Above Normal |
| Glucose | 1=Normal, 2=Above Normal, 3=Well Above Normal |
| Smoker | 0=No, 1=Yes |
| Alcohol | 0=No, 1=Yes |
| Physical Activity | 0=No, 1=Yes |
| Target | 0=No Disease, 1=Disease |

## 🚀 How to Run This Project

### 1. Clone/Download the project
```bash
git clone <your-repo-link>
cd Heart-Disease-Prediction

2. Install dependencies
pip install streamlit pandas numpy scikit-learn joblib

3. Train the model
Run the Jupyter/Colab notebook first to generate:svm_model.pklscaler.pkl

4. Run the Streamlit App
python -m streamlit run Web_heart_disease_prediction.py
Then open http://localhost:8501 in your browser.

📊 Model Performance
Algorithm: Support Vector Machine
Accuracy: ∼72-75% on test data
Note: Model is biased towards Age. Needs more balanced data for better real-world performance.

🔮 Future Improvements
Use more balanced dataset / SMOTE
Add more algorithms: Random Forest, XGBoostAdd data visualization and EDA
Deploy on Streamlit Cloud / Heroku
