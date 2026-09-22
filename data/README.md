# Dataset Information

This project utilizes two primary benchmark review datasets:

1. **Amazon Product Reviews Dataset (Sentiment Analysis)**
   - **Size**: 47,000+ customer reviews.
   - **Task**: Binary and multi-class sentiment classification.
   - **Features**: Pretrained Word2Vec & GloVe word embeddings.

2. **Computer-Generated Fake Reviews Dataset (Fake Review Detection)**
   - **Size**: 40,000+ labeled reviews (20,000 human-written, 20,000 computer-generated).
   - **Task**: Detection of synthetic / deceptive fake reviews.
   - **Features**: Bag-of-Words, TF-IDF, and sequential neural network tokenizers.

> **Note**: Due to file size limits, raw datasets and word embedding models (`glove.6B.100d.txt` / `GoogleNews-vectors-negative300.bin`) are excluded from repository version control. Download links and loading scripts are detailed in the respective notebooks under `notebooks/`.
