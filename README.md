# FashionMNIST Clothing Classification with CNN

This project involves building, training, and evaluating a custom Convolutional Neural Network (CNN) using PyTorch for multi-class image classification on the FashionMNIST dataset.

---

## 🧠 Project Overview

- **Objective:** Classify 10 types of clothing items in the FashionMNIST dataset using a CNN built from scratch.
- **Framework:** PyTorch

---

## 🏗️ Architecture

The CNN architecture consists of:
- **3 Convolutional Layers** with ReLU activation and MaxPooling
- **3 Fully Connected Layers** (FC1 → FC2 → FC3)
- **Softmax** output layer for 10 classes

---

## 📈 Key Results

- **Best Accuracy:** 91.1% with 10% validation split using SGD (lr = 0.1)
- **Best AUC Score:** 0.9900 for one-vs-all evaluation (label '2' vs rest)
- **Optimizer Comparison:**  
  - SGD Accuracy: 90.48%  
  - Adam Accuracy: 10.00%  
- **Learning Rate Tuning (SGD):**  
  - 0.001: 41.21%  
  - 0.01: 82.49%  
  - 0.1: 89.37%  
  - 1 & 10: 10.00% (unstable)

---

## 🧪 Experiments

- **Validation Splits Tested:** 0%, 10%, 20%, 30%, 40%
- **Learning Rates Tested:** 0.001, 0.01, 0.1, 1, 10
- **Optimizers:** SGD and Adam
- **Evaluation Metrics:** Accuracy and AUC

---

## 🔧 Installation

```bash
pip install torch torchvision matplotlib
