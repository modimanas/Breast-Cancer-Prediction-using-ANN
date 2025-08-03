# 🧠 Breast Cancer Prediction using ANN

This project builds an Artificial Neural Network (ANN) to predict breast cancer (Malignant or Benign) using the well-known Breast Cancer Wisconsin dataset from `sklearn.datasets`.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Demo](#demo)
- [Project Structure](#project-structure)
- [License](#license)

---

## 📖 Overview

Breast cancer is one of the most common cancers affecting women worldwide. Early detection and diagnosis play a vital role in increasing the chances of successful treatment.

This project utilizes a basic ANN built with TensorFlow/Keras to predict the type of tumor using 30 numerical features derived from digitized images of a fine needle aspirate (FNA) of a breast mass.

---

## 📊 Dataset

- 📦 Source: `sklearn.datasets.load_breast_cancer()`
- 💡 Features: 30 numerical attributes (mean, standard error, worst of various cell measurements)
- 🎯 Target: 
  - 0: Malignant (dangerous)
  - 1: Benign (non-cancerous)

---

## 🏗️ Model Architecture

The ANN is a simple feedforward network:

- **Input Layer:** 30 features
- **Hidden Layer 1:** 16 neurons, ReLU activation
- **Hidden Layer 2:** 8 neurons, ReLU activation
- **Output Layer:** 1 neuron, Sigmoid activation

Compiled with:
- **Loss Function:** `binary_crossentropy`
- **Optimizer:** Adam (learning rate = 0.001)
- **Metric:** Accuracy

---

## ⚙️ Installation

Clone the repo and install the dependencies:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
pip install -r requirements.txt

