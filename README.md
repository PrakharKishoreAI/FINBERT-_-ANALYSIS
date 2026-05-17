# Financial Sentiment Analysis using FinBERT

A deep learning NLP project for financial sentiment classification using FinBERT (BERT fine-tuned for finance domain text) and the Financial PhraseBank dataset.

This project classifies financial news sentences into:

- Positive
- Neutral
- Negative

Built using Hugging Face Transformers, PyTorch, and Scikit-learn with Kaggle GPU support.

---

## Project Overview

Financial sentiment analysis is a Natural Language Processing (NLP) task used to determine the sentiment of financial text such as:

- stock market news
- earnings reports
- analyst commentary
- company announcements
- financial headlines

General sentiment models often fail on finance-specific language because terms like:

- "profit warning"
- "bullish momentum"
- "market correction"
- "revenue growth"

have domain-specific meanings.

To solve this, this project uses **FinBERT**, a transformer model specifically trained for financial sentiment understanding.

---

## Features

- Financial domain sentiment classification
- FinBERT transformer model
- Financial PhraseBank dataset support
- Custom dataset preprocessing
- Label encoding
- Train / Validation / Test split
- Tokenization using Hugging Face tokenizer
- Fine-tuning with Trainer API
- GPU-compatible Kaggle notebook
- Evaluation metrics:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
- Confusion Matrix visualization
- Classification Report
- Custom real-time sentiment prediction

---

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Kaggle Notebook

---

## Model Used

### FinBERT

Model: `ProsusAI/finbert`

FinBERT is a BERT-based transformer model pre-trained specifically for financial text sentiment analysis.

Advantages:

- Better understanding of financial terminology
- Higher accuracy than generic BERT on finance data
- Handles contextual meaning in business language

Example:

Sentence:
> "The company reported strong quarterly earnings."

Prediction:
> Positive

Sentence:
> "The company suffered a major decline in operating profit."

Prediction:
> Negative

---

## Dataset

Dataset used:
**Financial PhraseBank (Sentences_75Agree.txt)**

Contains labeled financial news sentences with sentiment labels:

- positive
- neutral
- negative

Format:

```text
Sentence text @ sentiment
author
prakhar kishore
