# 🤖 CodeAlpha Machine Learning Internship
### Transforming Data into Intelligence — 3 Real-World ML Projects

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.21-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![Tasks](https://img.shields.io/badge/Tasks_Completed-3%2F4-blue?style=for-the-badge)

---

## 👩‍💻 About Me
> I am **Sakshi Chougule**, a B.Tech CSE (AI & ML) student at
> Rajarambapu Institute of Technology, Sangli (Batch 2024-28).
> This repository contains all my Machine Learning projects
> completed during the **CodeAlpha ML Internship**.
> Each project solves a real-world problem using data-driven
> approaches and state-of-the-art ML algorithms.

---

## 🗂️ Repository Structure
📁 CodeAlpha_Task/
│
├── 📁 CodeAlpha_CreditScoringModel/
│     ├── 📓 CodeAlpha_CreditScoringModel.ipynb
│     └── 📊 german_credit_data.csv
│
├── 📁 CodeAlpha_DiseasePrediction/
│     ├── 📓 CodeAlpha_DiseasePrediction.ipynb
│     └── 📊 diabetes.csv
│
└── 📁 CodeAlpha_HandwrittenCharacterRecognition/
└── 📓 CodeAlpha_HandwrittenCharacterRecognition.ipynb
---

## 🏦 Task 1 — Credit Scoring Model

> **Can we predict if a person will repay their loan?**
> Using real financial data to protect banks from bad loans.

### 🎯 Problem Statement
Predict whether a person is **creditworthy (good/bad risk)**
using their financial and demographic information.

### 📊 Dataset
| Property | Details |
|---|---|
| Name | German Credit Data |
| Samples | 1000 patients |
| Features | 10 (Age, Credit Amount, Duration, etc.) |
| Target | Risk — Good (700) / Bad (300) |
| Challenge | Class Imbalance (70:30 ratio) |

### 🔬 Methodology
- ✅ Exploratory Data Analysis with 5 visualizations
- ✅ Label Encoding + Standard Scaling
- ✅ Outlier Removal using IQR method
- ✅ Class Imbalance handled with `class_weight='balanced'`
- ✅ 5-Fold Cross Validation
- ✅ Feature Importance Analysis

### 🤖 Model Comparison
| Model | Accuracy | ROC-AUC | CV Score |
|---|---|---|---|
| Logistic Regression | ~56% | ~0.66 | ~0.63 |
| Decision Tree | ~61% | ~0.59 | ~0.60 |
| **Random Forest** ✅ | **~75%** | **~0.74** | **~0.73** |

### 💡 Key Insight
> **Duration**, **Credit Amount**, and **Age** are the
> top 3 most important features for predicting credit risk.

---

## ✍️ Task 3 — Handwritten Character Recognition

> **Can a machine read human handwriting?**
> Teaching computers to recognize digits just like humans do.

### 🎯 Problem Statement
Build a deep learning model to recognize
**handwritten digits (0-9)** from grayscale images.

### 📊 Dataset
| Property | Details |
|---|---|
| Name | MNIST |
| Training Samples | 60,000 images |
| Testing Samples | 10,000 images |
| Image Size | 28×28 pixels |
| Classes | 10 (digits 0–9) |

### 🔬 Methodology
- ✅ Auto-downloaded dataset (no manual setup)
- ✅ Pixel normalization (0-255 → 0-1)
- ✅ CNN with 3 Convolutional Blocks
- ✅ BatchNormalization for stable training
- ✅ Dropout (0.5) to prevent overfitting
- ✅ EarlyStopping callback
- ✅ Misclassified sample visualization

### 🏗️ Model Architecture
| Layer | Details |
|---|---|
| Conv Block 1 | 32 filters + BatchNorm + MaxPooling |
| Conv Block 2 | 64 filters + BatchNorm + MaxPooling |
| Conv Block 3 | 128 filters + BatchNorm |
| Dense | 256 neurons + Dropout(0.5) |
| Output | 10 neurons + Softmax |

### 📈 Results
| Metric | Score |
|---|---|
| **Test Accuracy** | **99.22%** 🔥 |
| Test Loss | 0.0287 |
| Misclassified | Only 78 / 10,000 |

### 💡 Key Insight
> Every digit class achieved **99-100% precision and recall**.
> BatchNormalization was the key to fast and stable convergence.

---

## 🏥 Task 4 — Disease Prediction from Medical Data

> **Can we detect diabetes before it's too late?**
> Using patient data to help doctors make better decisions.

### 🎯 Problem Statement
Predict whether a patient is **diabetic or not**
using medical diagnostic measurements.

### 📊 Dataset
| Property | Details |
|---|---|
| Name | Pima Indians Diabetes Dataset |
| Samples | 768 patients |
| Features | 8 (Glucose, BMI, Age, Insulin, etc.) |
| Target | Outcome — Diabetic (1) / Non-Diabetic (0) |
| Challenge | Biologically impossible zero values |

### 🔬 Methodology
- ✅ Replaced impossible zero values with median
- ✅ Exploratory Data Analysis with 4 visualizations
- ✅ StandardScaler for feature normalization
- ✅ Stratified train-test split
- ✅ 4 models compared
- ✅ 5-Fold Cross Validation
- ✅ Feature Importance Analysis

### 🤖 Model Comparison
| Model | Accuracy | ROC-AUC | CV Score |
|---|---|---|---|
| Logistic Regression | 73.38% | 0.8126 | 0.7525 |
| SVM | 72.73% | 0.8139 | 0.7346 |
| XGBoost | 75.32% | 0.8044 | 0.7232 |
| **Random Forest** ✅ | **75.97%** | **0.8256** | **0.7703** |

### 💡 Key Insight
> **Glucose**, **BMI**, and **Insulin** are the strongest
> predictors of diabetes in this dataset.

---

## 📊 Overall Results Summary
| Task | Algorithm | Accuracy | Highlight |
|---|---|---|---|
| Credit Scoring | Random Forest | ~75% | Handles class imbalance |
| Handwritten Recognition | CNN | **99.22%** 🔥 | Best performing model |
| Disease Prediction | Random Forest | ~76% | Medical data preprocessing |

---

## 🛠️ Tech Stack
| Category | Tools |
|---|---|
| Language | Python 3.10 |
| ML Library | Scikit-learn, XGBoost |
| Deep Learning | TensorFlow 2.21, Keras |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook, Anaconda |

---

## 📬 Connect With Me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/sakshi-chougule)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/SakshiChougule2006)

---

⭐ **Star this repo if you found it helpful!**
