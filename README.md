Problem Statement

During natural disasters, a large number of tweets are posted online. Emergency response teams need a fast way to identify tweets that report real disaster situations. This project builds a text-classification pipeline to automatically classify tweets as disaster or non-disaster, helping authorities prioritize critical information.

Dataset Description
The dataset is taken from the Kaggle “Real or Fake Disaster Tweets” competition.
It contains short tweets labeled as:
1 → Real disaster
0 → Not a disaster
The dataset was provided in ZIP format and extracted programmatically for reproducibility. Each record includes the tweet text and its corresponding label.

Setup Instructions
Clone the repository
Install required libraries:
pip install -r requirements.txt
Run the Jupyter notebook to reproduce preprocessing, feature engineering, model training, and evaluation.
All random seeds are fixed to ensure reproducible results.

Results Summary
Multiple models and feature representations were evaluated:
Naïve Bayes with Bag-of-Words performed well and was fast, but less accurate.
Logistic Regression with TF-IDF achieved the best overall performance.

Word2Vec embeddings captured semantic meaning but slightly underperformed TF-IDF due to loss of word order.

Overall, TF-IDF combined with Logistic Regression provided the best balance between accuracy, efficiency, and interpretability for this task.
