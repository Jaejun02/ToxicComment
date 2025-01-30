# 📢 Toxic Comment Classification using DistilBERT

This project develops a **multi-label toxic comment classifier** using the **DistilBERT** architecture. It integrates **Optuna** for hyperparameter tuning, **stratified k-fold validation**, and **mixed-precision training** to enhance efficiency and performance.

---
## 🧐 About
Online discussions often contain harmful content, making automated moderation crucial. This project utilizes **natural language processing (NLP)** to classify comments into multiple toxicity categories. By leveraging **DistilBERT** as the feature extractor and a custom classifier head, the model achieves high accuracy in detecting toxic content.

---
## ✨ Key Features
✅ **Advanced text preprocessing** (regex-based cleaning, contractions handling)  
✅ **Multilabel stratified data splitting** for balanced training  
✅ **Custom classifier head** with layer normalization  
✅ **Hyperparameter optimization** using Optuna  
✅ **Mixed-precision training** for computational efficiency  
✅ **Model checkpointing** and metadata storage for reproducibility  

---
## ⚙️ Installation
### Prerequisites
Ensure you have Python installed and set up a **Conda environment**:
```bash
conda env create -f environment.yml
conda activate toxic-comment-classifier
```

---
## 🚀 Usage
1️⃣ **Clone the repository** from GitHub:
```bash
git clone <https://github.com/Jaejun02/ToxicComment.git>
cd toxic-comment-classifier
```
2️⃣ **Open the Jupyter Notebook** (`toxic_comment_classifier.ipynb`) in JupyterLab or another compatible environment.

3️⃣ **Execute the cells** in order to preprocess data, train the model, and evaluate results.

---
## 📊 Model Evaluation
The model is evaluated using **F1-score** and **cross-validation** techniques. Training metrics are logged to ensure transparency and performance tracking.

---
## 📜 License
This project is licensed under the **MIT License**.

---
📌 **Author:** Jaejun Shim  
📆 **Date:** December 23, 2024