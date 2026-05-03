# Heart Disease Predictor

A machine learning web application for predicting the risk of heart disease based on patient health metrics. Built with Streamlit and scikit-learn.

## 📋 Overview

This project uses a K-Nearest Neighbors (KNN) classifier trained on heart disease data to predict whether a patient is at high or low risk of heart disease. The application provides an interactive web interface where users can input their health parameters and receive instant predictions.

## ✨ Features

- **Interactive Web Interface**: User-friendly Streamlit app for easy input of health metrics
- **Real-time Predictions**: Instant risk assessment based on trained machine learning model
- **Comprehensive Input Fields**: Covers all major heart disease risk factors including:
  - Age
  - Sex
  - Chest pain type
  - Resting blood pressure
  - Cholesterol levels
  - Fasting blood sugar
  - Resting ECG results
  - Maximum heart rate
  - Exercise-induced angina
  - ST depression (Oldpeak)
  - ST slope
- **Visual Feedback**: Clear risk indicators with success/error messages

## 🛠️ Technologies Used

- **Python**: Core programming language
- **Streamlit**: Web application framework
- **scikit-learn**: Machine learning library for KNN classifier
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **joblib**: Model serialization
- **matplotlib/seaborn**: Data visualization (in analysis notebook)

## 📊 Dataset

The model is trained on a heart disease dataset containing patient records with various health metrics and corresponding heart disease diagnoses. The dataset includes both numerical and categorical features that are preprocessed and encoded for optimal model performance.

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/heart-disease-predictor.git
   cd heart-disease-predictor
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## 🎯 Usage

1. **Run the Streamlit app:**
   ```bash
   streamlit run app10.py
   ```

2. **Open your browser** and navigate to the provided local URL (typically `http://localhost:8501`)

3. **Enter patient information** in the input fields

4. **Click "Predict"** to get the heart disease risk assessment

## 📈 Model Details

- **Algorithm**: K-Nearest Neighbors (KNN)
- **Preprocessing**: Standard scaling for numerical features, one-hot encoding for categorical variables
- **Features**: 11 input features after preprocessing
- **Output**: Binary classification (0: Low Risk, 1: High Risk)

## 📁 Project Structure

```
heart-disease-predictor/
│
├── app10.py                 # Main Streamlit application
├── heart.ipynb              # Jupyter notebook for data analysis and model training
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation
├── KNN_heart.pkl           # Trained KNN model
├── scaler.pkl              # Feature scaler
└── columns.pkl             # Feature column names
```

## 🔍 Data Analysis

The `heart.ipynb` notebook contains:
- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Feature engineering
- Model training and evaluation
- Comparison of multiple algorithms (Logistic Regression, SVM, KNN, Naive Bayes, Decision Tree)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## ⚠️ Disclaimer

This application is for educational and informational purposes only. It should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare providers for medical concerns.