# ✍️ Handwritten Character Recognition
### CodeAlpha Machine Learning Internship — Task 3

![Python](https://img.shields.io/badge/Python-3.10-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.21-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

---

## 📌 Objective
Recognize handwritten digits (0-9) from images using
a Convolutional Neural Network (CNN) on the MNIST dataset.

---

## 📊 Dataset
| Property | Details |
|---|---|
| Name | MNIST |
| Training Samples | 60,000 |
| Testing Samples | 10,000 |
| Image Size | 28×28 pixels |
| Classes | 10 (digits 0-9) |

---

## 🏗️ Model Architecture
| Layer | Details |
|---|---|
| Conv Block 1 | 32 filters + BatchNorm + MaxPooling |
| Conv Block 2 | 64 filters + BatchNorm + MaxPooling |
| Conv Block 3 | 128 filters + BatchNorm |
| Dense | 256 neurons + Dropout(0.5) |
| Output | 10 neurons + Softmax |

---

## 📈 Results
| Metric | Score |
|---|---|
| **Test Accuracy** | **99.22%** 🔥 |
| Test Loss | 0.0287 |
| Misclassified | 78 / 10,000 |

---

## ✅ Key Findings
- CNN achieved 99.22% accuracy on MNIST
- BatchNormalization stabilized training
- Dropout (0.5) prevented overfitting
- Only 78 out of 10,000 digits misclassified

---

## 🛠️ Libraries Used
- Python, NumPy, Matplotlib, Seaborn
- TensorFlow, Keras
- Scikit-learn

---

## 👩‍💻 Author
**Sakshi Chougule**
B.Tech CSE (AI & ML) — Rajarambapu Institute of Technology
CodeAlpha ML Internship 2026
