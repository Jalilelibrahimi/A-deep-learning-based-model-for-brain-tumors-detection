# 🧠 Brain Tumor Detection using Neutrosophic Domain and Transfer Learning

## 📌 Overview
This repository presents a deep learning-based framework for automatic brain tumor detection using MRI images. The proposed approach integrates **Neutrosophic image transformation** with **transfer learning models (VGG16 and ResNet50)** to improve classification performance and robustness.

The system addresses uncertainty and noise in medical images by transforming them into three domains:
- Truth (T)
- Indeterminacy (I)
- Falsity (F)

---

## 🚀 Key Contributions
- ✅ Hybrid framework combining Neutrosophic logic and deep transfer learning  
- ✅ Comparative evaluation across multiple image domains  
- ✅ High-performance classification (up to **99.11% accuracy**)  
- ✅ Robust handling of noisy and uncertain MRI data  

---

## 🧠 Methodology

### 1. Preprocessing
- Resize images to 224×224
- Normalize pixel values

### 2. Neutrosophic Transformation
Each image is decomposed into:
- **T (Truth)** → texture information  
- **I (Indeterminacy)** → uncertainty/boundaries  
- **F (Falsity)** → background  

### 3. Models
- VGG16 (Transfer Learning)
- ResNet50 (Transfer Learning)

### 4. Training
- Epochs: 30  
- Dropout: 0.5  
- Optimized using TensorFlow/Keras  

---

## 📊 Results

| Model      | Domain        | Accuracy |
|------------|-------------|----------|
| ResNet50   | Truth       | **99.11%** |
| ResNet50   | Original    | 98.22% |
| VGG16      | Truth       | 98.11% |

✔ Best performance achieved using **ResNet50 + Truth domain**

---

## 📁 Dataset
- Source: Kaggle Brain MRI Dataset  
- 3000 labeled images:
  - Tumor: 1500  
  - Normal: 1500  

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/brain-tumor-detection-neutrosophic.git
cd brain-tumor-detection-neutrosophic
pip install -r requirements.txt
