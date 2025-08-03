# 🧠 Breast Cancer Detection using Artificial Neural Networks (ANN)

This project builds an Artificial Neural Network (ANN) to predict whether a breast tumor is **benign** or **malignant** using the Breast Cancer Wisconsin dataset. It demonstrates the full ML pipeline from data preprocessing to deployment-ready model prediction.

---

## 📌 Problem Statement

Early and accurate detection of breast cancer is crucial for patient survival. This project uses machine learning to classify tumors based on their characteristics, helping support early diagnosis and treatment planning.

---

## 🧪 Tech Stack

- Python
- Libraries: `NumPy`, `Pandas`, `Seaborn`, `Matplotlib`
- Scikit-learn
- TensorFlow / Keras
- Deployment Tools: `joblib`, `.keras` model saving

---

## 📁 Dataset

Dataset used is **Breast Cancer Wisconsin (Diagnostic)** from `sklearn.datasets`.

- 🔬 Features: 30 numerical features like radius, texture, smoothness, symmetry, etc.
- 🎯 Target:  
  - 0 = **Malignant (Dangerous)**  
  - 1 = **Benign (Not Dangerous)**

---

## 🚀 Project Workflow

1. **Data Loading** and Exploration using Pandas and Seaborn  
2. **Data Preprocessing**:
   - Null value check
   - Standardization using `StandardScaler`
3. **Model Building**:
   - ANN with 2 hidden layers (`ReLU` activation)
   - Output layer with `sigmoid` activation
4. **Model Training**:
   - Optimizer: `Adam`
   - Loss: `binary_crossentropy`
   - Epochs: 200, Batch size: 16
5. **Evaluation**:
   - Accuracy on test data
   - `model.evaluate()` results printed
6. **Deployment Preparation**:
   - Trained model saved as `.keras`
   - Scaler saved using `joblib`
7. **User Prediction System**:
   - Takes 30 input features from user
   - Predicts tumor type using trained model

---

## 🧪 Example Prediction (Terminal Input/Output)

```bash
Enter 30 features as a list (e.g., [17.99, 10.38, ..., 0.0]):

Prediction: Benign (Class 1)
