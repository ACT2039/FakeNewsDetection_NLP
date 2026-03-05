# 📰 Fake News Detection using NLP

A machine learning project that classifies news articles as **Real or Fake** using **Natural Language Processing (NLP)** techniques and a **Logistic Regression classifier trained on TF-IDF features**.

---

# 📌 Project Overview

The rapid spread of misinformation online has made **fake news detection** an important problem.
This project applies **machine learning and NLP techniques** to automatically classify news articles as **real or fake** based on their textual content.

The model analyzes news article text and predicts whether it is **authentic journalism or misinformation**.

---

# 📊 Dataset

Dataset used: **Fake and Real News Dataset** from Kaggle.

The dataset contains two files:

| File       | Description                          |
| ---------- | ------------------------------------ |
| `Fake.csv` | Contains fake news articles          |
| `True.csv` | Contains verified real news articles |

Each record contains:

* Title
* Article text
* Subject
* Publication date

After preprocessing, the datasets are combined into a single labeled dataset for training.

---

# ⚙️ Machine Learning Pipeline

```
News Dataset
      ↓
Text Preprocessing
      ↓
TF-IDF Feature Extraction
      ↓
Train-Test Split
      ↓
Model Training
(Logistic Regression)
      ↓
Model Evaluation
      ↓
Fake News Prediction
```

---

# 🔧 Methodology

### 1️⃣ Data Preprocessing

* Combined real and fake news datasets
* Added binary labels (0 = Fake, 1 = Real)
* Shuffled dataset for balanced training

### 2️⃣ Text Cleaning

* Converted text to lowercase
* Removed punctuation and irrelevant characters
* Removed stopwords

### 3️⃣ Feature Engineering

Used **TF-IDF Vectorization** to convert text into numerical features representing word importance.

### 4️⃣ Model Training

Trained a **Logistic Regression classifier** on the TF-IDF feature matrix.

### 5️⃣ Model Evaluation

Model performance evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report

---

# 📈 Model Performance

The model achieved approximately:

**Accuracy: ~96%**

This indicates strong capability in distinguishing between real and fake news articles.

---

# 🖼️ Results

## Dataset Preview

![Dataset](images/dataset_preview.png)

---

## Model Accuracy

![Accuracy](images/accuracy_output.png)

---

## Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

---

# 🛠️ Technologies Used

* Python
* Pandas
* Scikit-learn
* Natural Language Processing (NLP)
* TF-IDF Vectorization
* Matplotlib
* Seaborn

---

# 📂 Project Structure

```
fake-news-detection-nlp
│
├── data
│   ├── Fake.csv
│   └── True.csv
│
├── notebooks
│   └── fake_news_detection.ipynb
│
├── images
│   ├── dataset_preview.png
│   ├── accuracy_output.png
│   └── confusion_matrix.png
│
├── requirements.txt
└── README.md
```

---

# 🚀 How to Run the Project

### 1️⃣ Clone the repository

```
git clone https://github.com/yourusername/fake-news-detection-nlp.git
```

### 2️⃣ Install dependencies

```
pip install -r requirements.txt
```

### 3️⃣ Run the notebook

Open the notebook:

```
notebooks/fake_news_detection.ipynb
```

Run all cells to train the model and evaluate results.

---

# 💡 Future Improvements

Potential improvements for the project:

* Implement **deep learning models (LSTM / BERT)**
* Build a **web application interface** for fake news detection
* Deploy the model using **Streamlit or Flask**
* Add **real-time news classification**

---

# 👨‍💻 Author

Charan Tej

Machine Learning & AI Enthusiast
Btech 2nd Year Student

---

