🧠 Advanced Machine Learning Methods for Alzheimer’s Disease Classification
A deep learning system designed to classify Alzheimer’s Disease (AD) stages using structural MRI scans.
The project evaluates multiple neural network architectures and introduces an optimized model for accurate and efficient AD detection.

🏆 3rd Place Winner – Graduation Projects Competition, College of Applied Computer Sciences, King Saud University

📖 Overview
Alzheimer’s Disease is a progressive neurodegenerative disorder and the most common cause of dementia worldwide.
Early detection is essential, but interpreting MRI scans requires expert knowledge and may miss subtle structural changes.

This project develops an AI-powered diagnostic tool that classifies MRI brain scans into four categories:

Non-Demented

Very Mild Demented

Mild Demented

Moderate Demented

The system uses deep learning to extract meaningful spatial and textural features from MRI images.

🎯 Objectives
Build an AI-based system for Alzheimer’s Disease classification

Use MRI scans as a non-invasive diagnostic tool

Compare multiple deep learning architectures

Improve accuracy using transfer learning and data augmentation

Deploy the model through an interactive web interface

🧱 Model Development Pipeline
Phase 1 — SimpleMLP
A basic fully connected network used as a baseline.
Accuracy: 83%

Phase 2 — ResNet‑18
A transfer learning approach using a pre-trained CNN.
Accuracy: 94%

Phase 3 — EfficientNet‑B0 (Final Model)
Lightweight, efficient, and highest-performing model.
Accuracy (Dataset 1): 99.75%
Accuracy (Dataset 2): 97.77%

🧪 Datasets
Dataset 1 — Kaggle MRI Dataset
Class	Images
Non-Demented	9,600
Very Mild Demented	8,960
Mild Demented	8,960
Moderate Demented	6,464
Total	33,984


After balancing: 38,400 images

Dataset 2 — Mendeley MRI Dataset
Class	Images
Non-Demented	3,200
Very Mild Demented	2,240
Mild Demented	896
Moderate Demented	64
Total	6,400


Used to test generalization across datasets.

⚙️ Technologies Used
Programming
Python

Deep Learning
PyTorch

Torchvision

Data Processing
NumPy

Pandas

OpenCV

Visualization
Matplotlib

Deployment
Gradio

Hugging Face Spaces

Environment
Jupyter Notebook

Git / GitHub

🧠 Model Configuration (EfficientNet‑B0)
Optimizer: AdamW

Learning Rate: 3e‑4

Weight Decay: 1e‑3

Loss Function: CrossEntropyLoss

Input Size: 224×224

Epochs: 5

Batch Size: 64

Preprocessing
Resize images to 224×224

Convert grayscale → RGB

Normalize using ImageNet statistics

Shuffle dataset

Train/test split with seed = 42

📊 Results
Dataset 1
Model	Accuracy
SimpleMLP	83%
ResNet‑18	94%
EfficientNet‑B0	99.75%


Dataset 2
Model	Accuracy
EfficientNet‑B0	97.77%


🏆 Comparison with Previous Work
Model	Accuracy
ALZENET	97.31%
SVM	89.84%
Inception‑ResNet‑V2	79.12%
Our EfficientNet‑B0	99.75%


🌐 Deployment
Gradio Interface
A simple UI allowing users to upload MRI images and receive predictions instantly.

Hugging Face Spaces
Hosted online for public access and demonstration.

🔗 Demo:  
https://huggingface.co/spaces/Yousef20/alzheimer-mri-detection

🚀 Installation
bash
git clone https://github.com/yourusername/alzheimer-mri-classification.git
cd alzheimer-mri-classification
pip install -r requirements.txt
python app.py
📂 Project Structure
كتابة تعليمات برمجية
Alzheimer-MRI-Classification/
│
├── app.py
├── train.py
├── predict.py
├── requirements.txt
├── README.md
│
├── models/
│   └── efficientnet_b0.pth
│
├── notebooks/
│   └── experiments.ipynb
│
├── images/
│   ├── confusion_matrix.png
│   ├── accuracy_curve.png
│   └── demo.png
│
├── docs/
│   └── Final_Report.pdf
│
└── dataset/
🔮 Future Work
Multi-modal learning (MRI + PET)

Longitudinal patient progression prediction

Explainable AI (Grad‑CAM, SHAP)

Larger multi-center datasets

Clinical workflow integration

Model optimization for mobile/edge devices

👨‍💻 Team Members
Talal Alshehri

Yousef Alabri

Omar Sahhari

Osama Raed

Supervisor:  
Prof. Mohamad Mahmoud Al Rahhal
College of Applied Computer Sciences — King Saud University

📜 License
Academic and research use only.
Reuse is allowed with proper attribution.
