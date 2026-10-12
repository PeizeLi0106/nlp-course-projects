# NLP Course Projects

Two collaborative course projects completed during the MSc in
Computer Science at Technische Universität Berlin.

Contributors: Peize Li and Benedikt Schäfer.

## Sentiment Analysis

Three-class sentiment classification of tweets using:
- Bag-of-Words and TF-IDF features
- Naive Bayes and feed-forward neural-network classifiers
- DistilBERT fine-tuning with Hugging Face Transformers
- GloVe embeddings for sentence similarity

Tools: Python, scikit-learn, NLTK, Hugging Face Transformers,
Gensim, pandas, and NumPy.

## Machine Translation

Neural machine translation experiments covering:
- English–Dutch GRU encoder–decoder models
- Word-level and character-level representations
- Word embeddings and additive attention
- Dutch–English–Swedish pivot translation with MarianMT
- Evaluation using BLEU and chrF

Tools: Python, TensorFlow/Keras, PyTorch, Hugging Face Transformers,
Gensim, and SacreBLEU.

## Repository Structure

- sentiment_analysis/notebooks/: sentiment analysis notebooks
- machine_translation/notebooks/: machine translation notebooks
- Each project has its own requirements.txt.

## Data and Model Files

Datasets, downloaded embeddings, and trained model checkpoints
are excluded from this repository.

## Project Context

These notebooks were developed collaboratively for coursework.
They document experiments and learning outcomes rather than
production-ready systems.

## Reports

- [Sentiment Analysis Report](sentiment_analysis/reports/sentiment_analysis_report.pdf)
- [Machine Translation Report](machine_translation/reports/machine_translation_report.pdf)

## Sentiment Dataset Access

The sentiment dataset, TweetSentiment.csv, was supplied through
the course and is not redistributed in this repository.

To run the sentiment notebooks, obtain the dataset through the
course and place it in sentiment_analysis/data/TweetSentiment.csv.