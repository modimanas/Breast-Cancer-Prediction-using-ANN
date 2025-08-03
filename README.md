# 🧠 Breast Cancer Prediction using ANN

[![Made with Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Colab](https://img.shields.io/badge/Run%20in-Colab-blue?logo=googlecolab)](https://colab.research.google.com/)

A deep learning model built with an Artificial Neural Network (ANN) to classify breast tumors as benign or malignant. Implemented in Python using TensorFlow and trained on the Breast Cancer Wisconsin dataset.

---

## 📚 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Results](#results)
- [Files Included](#files-included)
- [Author](#author)

---

## 📝 Overview

Breast cancer is among the leading causes of cancer deaths worldwide. This project uses an ANN to detect breast cancer from patient data — assisting in early diagnosis and potential life-saving outcomes.

---

## 📊 Dataset

- **Source**: `sklearn.datasets.load_breast_cancer()`
- **Instances**: 569 samples
- **Features**: 30 numerical features
- **Target Classes**:
  - `0`: Malignant
  - `1`: Benign

---

## 🧠 Model Architecture

The Artificial Neural Network (ANN) has the following layers:

- **Input Layer**: 30 input features
- **Hidden Layer 1**: 16 neurons with ReLU activation
- **Hidden Layer 2**: 8 neurons with ReLU activation
- **Output Layer**: 1 neuron with Sigmoid activation

**Optimizer**: Adam  
**Loss Function**: Binary Crossentropy  
**Epochs**: 200  
**Batch Size**: 16  
**Validation Split**: 0.1

---

## 🛠️ Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
```
---

## 🚀 How to Use

1. Open the file `21_7_2025_BREAST_CANCER_USING_ANN.ipynb` in Jupyter or Google Colab.
2. Run all the cells to train the model and save it.
3. After training, the model will be saved as `breast_cancer_model.keras`.
4. You can input any 30-feature test data like this:

```python
Enter 30 features as a list (e.g., [17.99, 10.38, ..., 0.0]):
---
```
#### 📌 “Results” Section:
```markdown
## 📈 Results

```python
Test Accuracy: ~96.49%

