# Detecting-Spam-Emails-Using-Tensorflow-in-Python


## 🚀 Project Overview  
Spam emails are unsolicited or unwanted messages sent in bulk, often cluttering inboxes and wasting user attention. This project focuses on building a **deep learning–based email classification system** that can automatically distinguish between **Spam** and **Ham (Not Spam)** emails using **TensorFlow** and **Natural Language Processing (NLP)** techniques.

The entire implementation is intentionally kept inside a **single Jupyter Notebook**, making the project easy to follow, reproduce, and learn from.

---

## 🎯 Objectives  
- **Automatically classify emails** as Spam or Ham  
- Apply **text preprocessing and NLP techniques**  
- Train an **LSTM-based deep learning model**  
- Achieve **high accuracy on unseen data**  

---

## 📂 Dataset Information  
- **File Name:** `Emails.csv`  
- **Total Records:** 5,171 emails  
- **Classes:**  
  - `spam` → Unwanted or promotional emails  
  - `ham` → Legitimate emails  

⚠️ The dataset was **imbalanced**, so the majority class (Ham) was **downsampled** to ensure fair model training.

---

## 🛠️ Tech Stack  
- **Language:** Python  
- **Libraries Used:**  
  - NumPy & Pandas (Data Handling)  
  - TensorFlow / Keras (Deep Learning)  
  - NLTK (Text Preprocessing)  
  - Scikit-learn (Train-Test Split)  
  - Matplotlib & Seaborn (Visualization)  
  - WordCloud (Text Insights)  

---

## 🧠 Approach & Workflow  

### 🔹 Data Preprocessing  
- Removed unnecessary email headers  
- Cleaned punctuation  
- Removed stopwords using NLTK  
- Normalized text for better learning  

### 🔹 Exploratory Data Analysis  
- Visualized class distribution  
- Generated **WordClouds** for Spam and Ham emails  

### 🔹 Text Vectorization  
- Tokenized text into numerical sequences  
- Applied padding to maintain equal sequence length  

---

## 🏗️ Model Architecture  
The model is built using **Keras Sequential API** and includes:

- **Embedding Layer** → Learns word representations  
- **LSTM Layer** → Captures sequential patterns in text  
- **Dense Layers** → Feature extraction  
- **Sigmoid Output Layer** → Binary classification  

This architecture is well-suited for **text classification problems**.

---

## ⚙️ Model Training  
- **Optimizer:** Adam  
- **Loss Function:** Binary Cross-Entropy  
- **Callbacks Used:**  
  - EarlyStopping (prevents overfitting)  
  - ReduceLROnPlateau (adaptive learning rate)  

Training was performed for multiple epochs with validation monitoring.

---

## 📊 Results  
- ✅ **Test Accuracy:** **97%**  
- ✅ **Test Loss:** 0.1202  

The model generalizes well and performs strongly on unseen data.

---

## 📁 Project Structure  

