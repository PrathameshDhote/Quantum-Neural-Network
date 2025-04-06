# 🍽️ Quantum Sentiment Analysis on Restaurant Reviews

This project implements sentiment analysis using a **Quantum Neural Network (QNN)** based **Variational Quantum Classifier (VQC)** with the **COBYLA optimizer**, and compares it with a classical **Support Vector Classifier (SVC)**. The dataset used includes restaurant reviews labeled as positive or negative.

---

## 📌 Overview

- **Dataset**: Sample restaurant reviews (positive/negative sentiment)
- **Quantum Model**: Variational Quantum Classifier (VQC)
- **Optimizer**: COBYLA (Constrained Optimization BY Linear Approximations)
- **Classical Baseline**: Support Vector Classifier (SVC)
- **Goal**: Explore the capability of QML in NLP sentiment classification

---

## 🧠 Technologies Used

- Python 🐍
- Qiskit 🧪
- scikit-learn
- Matplotlib
- NumPy, Pandas

---

## ⚙️ Model Architecture

### 🔹 Quantum Model (VQC)

- **Feature Map**: `PauliFeatureMap`
- **Ansatz**: Two-layer parameterized quantum circuit
- **Optimizer**: COBYLA (gradient-free)
- **Backend**: Qiskit Aer Simulator

### 🔸 Classical Model (SVC)

- Standard SVC from `sklearn.svm`
- Trained on the same vectorized feature representation of text

---

## 📊 Training Visualization

![Objective Function Plot](ss.png)

The graph above shows the **Objective Function Value vs Iteration** during training of the VQC model using the COBYLA optimizer.

### 🔍 Observations:

- High fluctuations initially as the optimizer explores.
- Objective function steadily decreases with iterations.
- Indicates effective convergence towards a local minimum.

**🕒 Training Time**: `374.69 seconds`

---

## 📈 Performance Comparison

| Model             | Accuracy | Training Time |
|------------------|----------|----------------|
| VQC (Quantum)    | ~59%     | 374.69s        |
| SVC (Classical)  | ~98%     | ~Z seconds     |

> 📌 Replace `XX`, `YY`, and `Z` with your actual values.

---

## 🧪 How to Run

### ✅ Setup

```bash
pip install qiskit scikit-learn pandas matplotlib


