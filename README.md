
# Twitter Sentiment Analysis using BERT

A Natural Language Processing (NLP) project that performs **multi-class sentiment classification** on Twitter text using **BERT (bert-base-uncased)** and the Hugging Face Transformers library. The model classifies tweets into four sentiment categories: **Positive**, **Negative**, **Neutral**, and **Irrelevant**.

---

## 📌 Project Overview

This project demonstrates an end-to-end NLP pipeline for Twitter sentiment analysis, including:

- Data preprocessing and cleaning
- Text tokenization using BERT tokenizer
- Fine-tuning a pre-trained BERT model
- Model evaluation using standard classification metrics
- Sentiment prediction on unseen tweets

The project is implemented in **Python** using **Google Colab**, **PyTorch**, and the **Hugging Face Transformers** library.

---

## 🎯 Objectives

- Clean and preprocess Twitter text
- Remove unwanted characters and missing values
- Tokenize text using the BERT tokenizer
- Fine-tune a pre-trained BERT model
- Evaluate model performance
- Predict sentiments of new tweets

---

## 📂 Dataset

The project uses the **Twitter Sentiment Analysis** dataset.

### Dataset Columns

| Column | Description |
|---------|-------------|
| tweet_id | Unique Tweet ID |
| entity | Related company/person/topic |
| sentiment | Target label |
| tweet_content | Tweet text |

### Target Classes

- Positive
- Negative
- Neutral
- Irrelevant

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- NLTK
- PyTorch
- Hugging Face Transformers
- Datasets Library
- Google Colab

---

## 📦 Required Libraries

```bash
pip install transformers
pip install datasets
pip install torch
pip install nltk
pip install scikit-learn
pip install pandas
pip install numpy
```

---

## 📁 Project Structure

```
Twitter-Sentiment-Analysis/
│
├── Twitter_sentiment_analysis.ipynb
├── twitter_training.csv
├── twitter_validation.csv
├── README.md
└── requirements.txt
```

---

## 🔄 Workflow

### 1. Import Libraries

- Pandas
- NumPy
- NLTK
- Transformers
- Datasets
- Scikit-learn
- PyTorch

---

### 2. Load Dataset

```python
df = pd.read_csv("twitter_training.csv")
df2 = pd.read_csv("twitter_validation.csv")
```

---

### 3. Data Preprocessing

The preprocessing pipeline includes:

- Removing duplicate records
- Removing missing values
- Dropping unnecessary columns
- Cleaning tweet text
- Lowercasing text
- Removing HTML tags
- Removing punctuation
- Removing stopwords

---

### 4. Tokenization

Tweets are tokenized using

```
bert-base-uncased
```

Example:

```python
tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
```

---

### 5. Model

Pre-trained model:

```
BERT Base Uncased
```

```python
AutoModelForSequenceClassification
```

Number of classes:

```
4
```

---

### 6. Training

The model is fine-tuned using the Hugging Face `Trainer` API.

Typical training parameters include:

- Learning Rate
- Batch Size
- Epochs
- Weight Decay
- Evaluation Strategy

---

### 7. Evaluation

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📊 Results

The notebook evaluates the fine-tuned BERT model on the validation dataset and reports standard classification metrics to measure performance.

> **Note:** Replace this section with your actual results after training.

Example:

| Metric | Score |
|---------|--------|
| Accuracy | 95.97% |
| Precision | 95.99 |
| Recall | 95.97 |
| F1 Score | 95.97 |

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/Ramesh-sirvi/Twitter-Sentiment-Analysis.git
```

### Open Project

```bash
cd Twitter-Sentiment-Analysis
```

### Install Requirements

```bash
pip install -r requirements.txt
```

### Launch Notebook

```bash
jupyter notebook
```

or open the notebook directly in **Google Colab**.

---

## 📈 Future Improvements

- Hyperparameter tuning
- Use RoBERTa or DeBERTa models
- Deploy using Streamlit or Flask
- Real-time Twitter sentiment analysis
- Add model explainability using SHAP or LIME
- Experiment with larger transformer models

---

## 📚 Learning Outcomes

This project demonstrates practical experience with:

- Natural Language Processing (NLP)
- Text preprocessing
- BERT architecture
- Hugging Face Transformers
- Transfer Learning
- Multi-class Text Classification
- Model Evaluation
- Deep Learning using PyTorch

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Added new feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 👨‍💻 Author

**Ramesh Choudhary**

If you found this project useful, consider giving it a ⭐ on GitHub!
