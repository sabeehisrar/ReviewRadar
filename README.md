# ReviewRadar

A comprehensive NLP platform for product review sentiment classification and computer-generated fake review detection using classical machine learning and deep neural networks.

## Problem
Online e-commerce platforms suffer from deceptive computer-generated fake reviews and noisy customer feedback that distort genuine product ratings. Automated systems must capture subtle sentiment nuances while accurately filtering out synthetic, computer-generated reviews. This repository provides end-to-end NLP pipelines to address both tasks effectively.

## Approach
- **Models/Techniques**: Logistic Regression with Bag-of-Words/TF-IDF, Support Vector Machines (SVM), and Bidirectional LSTM Neural Networks utilizing pretrained **Word2Vec** and **GloVe** vector embeddings.
- **Data**: 47,000+ Amazon customer product reviews for sentiment classification, and 40,000+ labeled human vs. synthetic reviews (20k real, 20k fake) for fake review detection.

## Results

| Task | Model | Accuracy |
| :--- | :--- | :--- |
| **Sentiment Analysis** | Logistic Regression | **90%** |
| **Sentiment Analysis** | Deep Neural Network / LSTM | **89%** |
| **Fake Review Detection** | Support Vector Machine (SVM) | **87%** |
| **Fake Review Detection** | Bidirectional LSTM | **96%** |

*Comprehensive performance curves and charts are available in [`results/`](results/results.md).*

## Tech Stack
- **Languages**: Python 3.11
- **NLP & ML**: `scikit-learn`, `tensorflow` (Keras), `gensim` (Word2Vec/GloVe), `nltk`
- **Data & Visualization**: `pandas`, `numpy`, `matplotlib`, `seaborn`

## How to Run
1. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
2. Run notebooks in order under `/notebooks`:
   - `notebooks/01_sentiment_logistic.ipynb` — Baseline sentiment classification using Logistic Regression
   - `notebooks/02_sentiment_lstm.ipynb` — Neural network sentiment modeling with embeddings
   - `notebooks/03_fake_review_svm.ipynb` — Fake review detection with SVMs and Bag-of-Words
   - `notebooks/04_fake_review_lstm.ipynb` — Deep learning fake review detection (96% Accuracy)
