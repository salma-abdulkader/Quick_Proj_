# 🩻 SPR X-Ray Age Prediction

This project aims to **predict human age from X-ray images** using deep learning models.  
Two different architectures were implemented and compared:  
- **MobileNetV2** (lightweight and fast)
- **DenseNet121** (deeper and more accurate)

---

## 📂 Project Files

| File Name | Description |
|------------|-------------|
| `s-spr-x-ray-agee_mobilenetv2.ipynb` | Implementation of the MobileNetV2 model for age prediction. |
| `spr-x-ray-age_densenet121.ipynb` | Implementation of the DenseNet121 model for age prediction. |

---

## 🧠 Models Overview

### 🔹 MobileNetV2
- Designed for **lightweight inference**.
- Faster training with less memory usage.
- Suitable for deployment on mobile or edge devices.

### 🔹 DenseNet121
- Deeper network with **dense connections**.
- Achieves higher accuracy.
- More computationally intensive.

---

## ⚙️ Workflow

1. **Dataset Preparation**
   - X-ray dataset (e.g., SPR Dataset or custom medical dataset).
   - Preprocessed (resize, normalization, augmentation).

2. **Model Building**
   - Transfer learning applied using pretrained CNN backbones.
   - Final dense layers customized for regression (age prediction).

3. **Training**
   - Loss: Mean Squared Error (MSE)
   - Optimizer: Adam
   - Metrics: MAE, RMSE

4. **Evaluation**
   - Model performance compared on validation and test sets.
   - Visualizations of predicted vs actual ages.

---

## 📊 Results Summary

| Model | MAE ↓ | RMSE ↓ | Accuracy ↑ | Notes |
|--------|--------|---------|-------------|--------|
| MobileNetV2 | *e.g., 4.8 years* | *6.2* | Fast, efficient | Lightweight |
| DenseNet121 | *e.g., 3.9 years* | *5.1* | More accurate | Higher resource usage |

*(Update the table with your actual results)*

---

## 🧰 Requirements

- Python 3.x  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib  
- Google Colab (Recommended)

Install dependencies:
```bash
!pip install tensorflow numpy pandas matplotlib scikit-learn
