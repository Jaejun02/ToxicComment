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
1️⃣ **Clone the repository** from GitHub:
```bash
git clone <https://github.com/Jaejun02/ToxicComment.git>
cd ToxicComment
```
2️⃣ Install dependencies through **Conda environment**:
```bash
conda env create -f environment.yml
conda activate toxiccs
```
3️⃣ **Combine the model files** by running:
```bash
cat ./saved_model/model.safetensors_* > ./saved_model/model.safetensors
```
4️⃣ **Download your Kaggle API key** by going to Kaggle, then going to your account settings and clicking **Create New API Token**.

5️⃣ **Set up your Kaggle API key** by running:
```bash
mkdir -p ~/.kaggle
mv /path/to/your/kaggle.json ~/.kaggle/kaggle.json
chmod 600 ~/.kaggle/kaggle.json
```

6️⃣ **Open the Jupyter Notebook** (`toxic_comment_classifier.ipynb`) in JupyterLab or another compatible environment.

7️⃣ **Execute the cells** in order to preprocess data, train the model, and evaluate results.


---
## 🚀 Usage
☑️ **Hyperparameter Tuning**
Set `HP_TUNING = True` in `Config` class and run `toxic_comment_classifier.ipynb`.

☑️ **Further Tuning and Final Training**
Set `FT_TUNING = True` and `FULL_TRAINING = True` in `Config` class and rurn `toxic_comment_classifier.ipynb`.


---
## 📊 Model Evaluation
Best test F1 Score: 0.947.

---
## 📜 License
This project is licensed under the **MIT License**.

---
📌 **Author:** Jaejun Shim  
📆 **Date:** December 23, 2024