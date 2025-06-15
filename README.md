# Pneumonia Detection from Chest X-Rays using CNN and Transfer Learning

Pneumonia is a severe lung infection that can be diagnosed through chest X-ray imaging. This project demonstrates how deep learning techniques can assist radiologists in diagnosing pneumonia by building a Convolutional Neural Network (CNN) that classifies chest X-ray images as **NORMAL** or **PNEUMONIA**.

---

## 🧠 Objective

To develop and evaluate a deep learning model for binary classification of chest X-ray images using:
- **Transfer Learning (ResNet50 and MobileNet)**
- **Model Explainability using Grad-CAM**

---

## 📂 Dataset

- **Name:** Chest X-Ray Images (Pneumonia) by Kermany et al.
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Description:** ~5,000 X-ray images categorized into `NORMAL` and `PNEUMONIA`, split into `train`, `val`, and `test` folders.

---

## 📊 Model Performance

| Model      | Accuracy | Precision | Recall | F1-Score |
|------------|----------|-----------|--------|----------|
| **ResNet50**  | 0.9071   | 0.9151    | 0.9071 | 0.9043   |
| **MobileNet** | 0.8686   | 0.8884    | 0.8686 | 0.8614   |

ResNet50 outperformed MobileNet in all evaluation metrics.

---

## 🔍 Explainable AI (XAI)

**Grad-CAM** (Gradient-weighted Class Activation Mapping) was used to visualize where the model is focusing when making predictions. This adds interpretability to the results and helps understand the decision-making of the deep learning model.

---

## 🧪 Project Workflow

### 1. Understand the Dataset
- Loaded and visualized X-ray samples.
- Analyzed class distribution.

### 2. Data Preprocessing
- Resized and normalized images.
- Applied data augmentation to improve generalization.

### 3. Model Development
- Built models using:
  - ✅ ResNet50
  - ✅ MobileNet
- Trained and fine-tuned both models.

### 4. Evaluation
- Metrics: Accuracy, Precision, Recall, F1-Score
- Confusion matrix and learning curves plotted.

### 5. Interpretability
- Applied Grad-CAM on sample predictions to visualize model attention.

---
