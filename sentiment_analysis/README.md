# Sentiment Analysis

A two-person NLP course project comparing traditional classifiers
and a pretrained Transformer for tweet sentiment classification.

## Dataset

TweetSentiment.csv was supplied through the course and is not
included in this repository.

Place it at:
data/TweetSentiment.csv

## Notebooks

1. task1_dataExploration.ipynb — dataset exploration and visualization.
2. task2_preprocessing.ipynb — text cleaning and preprocessing.
3. task3_classification.ipynb — Naive Bayes and neural-network baselines.
4. task4_textualSimilarity.ipynb — GloVe embeddings and cosine similarity.
5. task5_pretrained.ipynb — DistilBERT fine-tuning and evaluation.

Run task2 before task3: it generates
data/TweetSentiment_preprocessed.csv.

## Running the Notebooks

Dependencies are listed in requirements.txt. Package-version
compatibility has not yet been verified in a fresh environment.

Open the notebooks in Jupyter with the working directory set to
sentiment_analysis/notebooks, so the relative data paths resolve.

Run cells from top to bottom within each notebook.
Some steps require internet access to download NLTK resources,
pretrained embeddings, or models. DistilBERT training benefits
from a GPU and may take substantially longer on a CPU.

## Results and Evaluation

DistilBERT achieved approximately 79.3% accuracy and 0.80 macro F1
for three-class sentiment classification.

The evaluation split was also used for model selection during
training; these are not results from an independent final test set.

See the [project report](reports/sentiment_analysis_report.pdf)
for experiments, comparisons, and analysis.