# Machine Learning Portfolio - Arch Technologies 🚀🤖

## 📌 Repository Overview
This repository contains a collection of machine learning models, preprocessors, and evaluation metrics developed over two months. The projects range from computer vision and natural language processing (NLP) to predictive regression and tabular classification.

Due to the size of the model files (`.keras`, `.pkl`, `.joblib`), this repository utilizes **Git Large File Storage (LFS)**.

---

## 📂 Folder Structure & Projects

### 📅 1st Month: Deep Learning & NLP
Focused on neural networks and text processing.
* **MNIST Digit Classifier:** A deep learning model (`mnist_model.keras`) trained to recognize handwritten digits.
* **Spam Classifier:** An NLP model utilizing a TF-IDF Vectorizer (`tfidf_vectorizer.pkl`) to extract features from text messages and classify them as spam or ham.

### 📅 2nd Month: Traditional ML & Ensemble Methods
Focused on structured data, regression, and classification using scikit-learn and XGBoost.
* **California Housing Predictor:** An XGBoost regression model (`california_housing_xgb_model.pkl`) built to predict housing prices based on demographic and geographic data.
* **Iris Flower Classifier:** A classification model (`iris_classifier_model.joblib`) with its corresponding data scaler (`iris_scaler.joblib`) to predict flower species.
* **Model Evaluations:** Includes comprehensive visual metrics such as confusion matrices, learning curves, and feature importance graphs to validate model performance.

---

## ⚙️ How to Download the Models (Important!)
Standard cloning will not download the heavy model weights. You **must** have [Git LFS](https://git-lfs.github.com/) installed to pull the actual files.

\`\`\`bash
# 1. Install Git LFS
git lfs install

# 2. Clone the repository
git clone https://github.com/Mohsan-Raza123/model-Arch-technologies-.git

# 3. Pull the large model files
cd model-Arch-technologies-
git lfs pull
\`\`\`

---

## 🚀 How to Load the Models in Python

**Loading the Keras Model (Month 1):**
\`\`\`python
import tensorflow as tf
mnist_model = tf.keras.models.load_model('1st month/model/mnist_model.keras')
\`\`\`

**Loading the Scikit-Learn/XGBoost Models (Month 2):**
\`\`\`python
import joblib
import pickle

# Load Joblib model and scaler
iris_model = joblib.load('2nd month/iris_classifier_model.joblib')
iris_scaler = joblib.load('2nd month/iris_scaler.joblib')

# Load Pickle model
with open('2nd month/california_housing_xgb_model.pkl', 'rb') as file:
    california_model = pickle.load(file)
\`\`\`

---

## 👨‍💻 Author
**Mohsan Raza**
* BS Computer Science | COMSATS University Islamabad
* [Link to your LinkedIn Profile]
