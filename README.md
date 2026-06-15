# 🧠 Advanced Machine Learning Methods for Alzheimer's Disease Classification

> Deep Learning-based system for Alzheimer's Disease (AD) stage classification using structural MRI scans.

🏆 **3rd Place Winner – Graduation Projects Competition**  
College of Applied Computer Sciences, King Saud University

---

## 📖 Overview

Alzheimer’s Disease (AD) is a progressive neurodegenerative disorder and the leading cause of dementia worldwide. Early diagnosis plays a crucial role in slowing disease progression and improving patient care. However, interpreting MRI scans requires significant expertise and subtle structural changes may be difficult to detect manually.

This project presents an AI-powered diagnostic system that automatically classifies brain MRI scans into four Alzheimer's disease stages using deep learning techniques.

### Classification Categories

- 🟢 Non-Demented
- 🟡 Very Mild Demented
- 🟠 Mild Demented
- 🔴 Moderate Demented

The proposed system leverages advanced convolutional neural networks and transfer learning techniques to extract meaningful spatial and textural features from MRI images.

---

## 🎯 Project Objectives

- Develop an AI-based Alzheimer's Disease classification system.
- Utilize MRI scans as a non-invasive diagnostic modality.
- Evaluate and compare multiple deep learning architectures.
- Improve performance through transfer learning and data augmentation.
- Deploy the final model through an interactive web application.

---

# 🧱 Model Development Pipeline

## Phase 1 — SimpleMLP

A fully connected neural network used as a baseline model.

| Metric | Value |
|----------|----------|
| Accuracy | 83% |

---

## Phase 2 — ResNet-18

Transfer learning approach using a pre-trained ResNet-18 architecture.

| Metric | Value |
|----------|----------|
| Accuracy | 94% |

---

## Phase 3 — EfficientNet-B0 (Final Model)

EfficientNet-B0 achieved the highest performance while maintaining computational efficiency.

| Dataset | Accuracy |
|----------|----------|
| Dataset 1 | 99.75% |
| Dataset 2 | 97.77% |

---

# 🧪 Datasets

## Dataset 1 — Kaggle MRI Dataset

| Class | Images |
|---------|---------:|
| Non-Demented | 9,600 |
| Very Mild Demented | 8,960 |
| Mild Demented | 8,960 |
| Moderate Demented | 6,464 |
| **Total** | **33,984** |

### Data Balancing

After augmentation and balancing:

**Total Images = 38,400**

---

## Dataset 2 — Mendeley MRI Dataset

| Class | Images |
|---------|---------:|
| Non-Demented | 3,200 |
| Very Mild Demented | 2,240 |
| Mild Demented | 896 |
| Moderate Demented | 64 |
| **Total** | **6,400** |

Used exclusively to evaluate model generalization across different datasets.

---

# ⚙️ Technologies Used

## Programming Language

- Python

## Deep Learning

- PyTorch
- Torchvision

## Data Processing

- NumPy
- Pandas
- OpenCV

## Visualization

- Matplotlib

## Deployment

- Gradio
- Hugging Face Spaces

## Development Environment

- Jupyter Notebook
- Git
- GitHub

---

# 🧠 EfficientNet-B0 Configuration

| Parameter | Value |
|------------|------------|
| Optimizer | AdamW |
| Learning Rate | 3e-4 |
| Weight Decay | 1e-3 |
| Loss Function | CrossEntropyLoss |
| Input Size | 224 × 224 |
| Epochs | 5 |
| Batch Size | 64 |

### Preprocessing Pipeline

- Resize images to 224 × 224
- Convert grayscale images to RGB
- Normalize using ImageNet statistics
- Shuffle dataset
- Train/Test split using `seed = 42`

---

# 📊 Results

## Dataset 1 Performance

| Model | Accuracy |
|---------|---------:|
| SimpleMLP | 83.00% |
| ResNet-18 | 94.00% |
| EfficientNet-B0 | **99.75%** |

---

## Dataset 2 Performance

| Model | Accuracy |
|---------|---------:|
| EfficientNet-B0 | **97.77%** |

---

# 🏆 Comparison with Previous Work

| Model | Accuracy |
|---------|---------:|
| ALZENET | 97.31% |
| SVM | 89.84% |
| Inception-ResNet-V2 | 79.12% |
| **Our EfficientNet-B0** | **99.75%** |


![Confusion-matrix](Confusion-matrix.png)

---

# 🌐 Deployment

## Gradio Interface

A user-friendly web interface allowing users to upload MRI scans and receive instant predictions.

## Hugging Face Spaces

Online deployment for public access and demonstration.
![Interface](demo.png)

### 🔗 Live Demo
![result](result.png)
**https://huggingface.co/spaces/Yousef20/alzheimer-mri-detection**

---


---

# 📂 Project Structure

```text
Alzheimer-MRI-Classification/
│
├── README.md
├── Final_Report.pdf
├── notebook/
├── model/
└── images/
```

---

# 🔮 Future Work

- Multi-modal learning (MRI + PET)
- Longitudinal patient progression prediction
- Explainable AI techniques (Grad-CAM, SHAP)
- Training on larger multi-center datasets
- Integration into clinical workflows
- Optimization for mobile and edge devices

---

# 👨‍💻 Team Members

- Talal Alshehri
- Yousef Alabri
- Omar Sahhari
- Osama Raed

### Academic Supervisor

**Prof. Mohamad Mahmoud Al Rahhal**

College of Applied Computer Sciences  
King Saud University



