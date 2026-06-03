# 🧠 Alzheimer’s Disease Classification Using MRI (Deep Learning)

A deep learning system designed to classify Alzheimer’s Disease (AD) into four stages using structural MRI scans.  
This project evaluates multiple architectures (SimpleMLP, ResNet‑18, EfficientNet‑B0) and achieves **state‑of‑the‑art accuracy of 99.75%** using EfficientNet‑B0.

---

## 📌 Project Overview
Alzheimer’s Disease is a progressive neurodegenerative disorder that affects memory and cognitive function.  
Early detection is crucial, but MRI interpretation requires expert knowledge and can miss subtle structural changes.

This project develops an **AI‑powered diagnostic tool** capable of classifying MRI scans into:

- **Non‑Demented**
- **Very Mild Demented**
- **Mild Demented**
- **Moderate Demented**

The system uses deep learning to extract spatial and textural features from MRI images and provides fast, accurate predictions.

---

## 🎯 Objectives
- Build a robust MRI‑based AD classification model  
- Compare multiple architectures (MLP → ResNet‑18 → EfficientNet‑B0)  
- Achieve high accuracy with efficient computation  
- Deploy the model using **Gradio** and **Hugging Face Spaces**  
- Evaluate generalization using two different MRI datasets  

---

## 🗂 Dataset
Two datasets were used:

### **1. Kaggle MRI Dataset (Primary)**
- 33,984 images before balancing  
- 38,400 images after balancing  
- Four AD categories  
- Axial MRI slices  

### **2. Mendeley MRI Dataset (Secondary)**
- 6,400 T1‑weighted MRI images  
- Resized to 128×128  
- Used to test cross‑dataset generalization  

> Example from the dataset:  
> *“The primary dataset contains 33,984 MRI images before balancing… After balancing, 38,400 images were used.”*  
> 

---

## 🧪 Model Development Journey

### **1️⃣ SimpleMLP — Baseline**
- Fully connected network  
- Accuracy: **83%**  
- Weak spatial understanding  

### **2️⃣ ResNet‑18 — Deep CNN**
- Transfer learning from ImageNet  
- Accuracy: **94%**  
- Better spatial feature extraction  

### **3️⃣ EfficientNet‑B0 — Final Model**
- Best accuracy: **99.75%**  
- Lightweight & efficient  
- Excellent generalization  
- Accuracy on second dataset: **97.77%**

> *“EfficientNet‑B0 achieved the highest performance… reaching 99.75% accuracy.”*  
> 

---

## 📊 Results Summary

| Model             | Accuracy |
|------------------|----------|
| SimpleMLP        | 83.00%   |
| ResNet‑18        | 94.00%   |
| EfficientNet‑B0  | **99.75%** |

Cross‑dataset performance:

| Dataset | Model | Accuracy |
|---------|--------|----------|
| Mendeley MRI | EfficientNet‑B0 | **97.77%** |

---

## 🧱 System Architecture
The pipeline includes:

1. **Data Loading & Labeling**  
2. **Image Preprocessing**  
   - Resize → 224×224  
   - Convert to RGB  
   - Normalize (ImageNet stats)  
3. **Model Training**  
4. **Evaluation & Confusion Matrix**  
5. **Deployment (Gradio + Hugging Face)**  

---

## 🛠 Tech Stack
- Python  
- PyTorch  
- Torchvision  
- NumPy / Pandas  
- Matplotlib  
- Gradio  
- Hugging Face Spaces  

---

## 🚀 Deployment

### **Gradio Web App**
Upload an MRI scan → get prediction instantly.

### **Hugging Face Spaces**
Permanent online demo:  
https://huggingface.co/spaces/Yousef20/alzheimer-mri-detection

> *“The application was deployed on Hugging Face Spaces to provide stable access…”*  
> 

---

## 📦 Repository Structure


---

## 🔮 Future Work
- Add PET/fMRI multimodal inputs  
- Longitudinal progression prediction  
- Explainability (Grad‑CAM, SHAP)  
- Lightweight model quantization  
- Clinical workflow integration  

---

## 👥 Authors
- Yousef Alabri  
- Talal Alshehri  
- Omar Sahhari  
- Osama Raed  

Supervised by: **Prof. Mohamad Al Rahhal**

---

## 📄 License
MIT License

