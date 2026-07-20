# 📰 Fake News Detection using NLP

A Machine Learning and Natural Language Processing (NLP) based project that classifies news articles as **Fake** or **Real** using the TF-IDF Vectorizer and Linear Support Vector Classifier (LinearSVC).

---

## 📌 Overview

Fake news spreads rapidly through social media and online platforms. This project uses Natural Language Processing (NLP) techniques to analyze news text and classify it as **Fake** or **Real**. The model is trained on a labeled dataset of fake and real news articles.

---

## ✨ Features

- Detects Fake and Real News
- Text Preprocessing
- Stopword Removal
- Lemmatization
- TF-IDF Feature Extraction
- Machine Learning Classification
- High Accuracy Prediction
- Model Evaluation using Accuracy, Precision, Recall and F1-Score

---

# 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Matplotlib
- WordCloud

---

# 📂 Project Structure

```
Fake_News_Classification/
│
├── Fake.csv
├── True.csv
├── fake-news-with-tf-idf-0-99385.ipynb
├── README.md
└── requirements.txt
```

---

# 📊 Dataset

The project uses two datasets.

### Fake.csv
Contains fake news articles.

### True.csv
Contains real news articles.

Both datasets are merged into a single dataframe before preprocessing.

---

# ⚙ Working Process

## Step 1 - Load Dataset

Load Fake.csv and True.csv using Pandas.

```python
fake = pd.read_csv("Fake.csv")
true = pd.read_csv("True.csv")
```

---

## Step 2 - Data Preprocessing

- Merge both datasets
- Assign labels
- Remove punctuation
- Convert text to lowercase
- Remove stopwords
- Lemmatization

---

## Step 3 - Feature Extraction

The cleaned text is converted into numerical vectors using

- TF-IDF Vectorizer

---

## Step 4 - Model Training

The dataset is divided into

- Training Data
- Testing Data

Then a LinearSVC model is trained.

---

## Step 5 - Prediction

The trained model predicts whether a news article is

- Fake News
- Real News

---

## Step 6 - Model Evaluation

The model performance is evaluated using

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

# 📈 Output

Example Output

```
Accuracy : 99.38%

Classification Report

Precision : 99%

Recall : 99%

F1 Score : 99%
```

---

# 💻 Installation

Clone the repository

```
git clone https://github.com/Sadiya6767/Fake_News_Classification.git
```

Move into the project folder

```
cd Fake_News_Classification
```

Install dependencies

```
pip install -r requirements.txt
```

If requirements.txt is not available

```
pip install pandas numpy matplotlib scikit-learn nltk wordcloud spacy
```

Download required NLTK data

```python
import nltk

nltk.download('stopwords')
nltk.download('punkt')
nltk.download('wordnet')
nltk.download('omw-1.4')
```

Run the notebook

```
jupyter notebook
```

Open

```
fake-news-with-tf-idf-0-99385.ipynb
```

Run all cells.

---

# 🧪 Testing

Users can enter their own news text and predict whether it is Fake or Real using the trained model.

---

# 📚 Machine Learning Pipeline

```
Dataset

↓

Text Cleaning

↓

Stopword Removal

↓

Lemmatization

↓

TF-IDF Vectorizer

↓

Train-Test Split

↓

LinearSVC Model

↓

Prediction

↓

Accuracy Evaluation
```

---

# 🚀 Future Improvements

- Streamlit Web Application
- Flask API
- Deep Learning Model (LSTM/BERT)
- Live News URL Detection
- Real-time Fake News Detection

---

# 👩‍💻 Author

**Sadiya**

GitHub:
https://github.com/Sadiya6767
