# Amazon Reviews Sentiment Analysis

## Project Topic
Sentiment Analysis of Amazon Product Reviews Using NLP and Machine Learning.

## Problem Statement
Amazon receives a huge volume of customer reviews every day. These reviews contain valuable signals about product quality, customer satisfaction, delivery issues, and common complaints. Manually reading and classifying thousands of reviews is time-consuming and impractical. This project builds an automated sentiment analysis pipeline to classify reviews as positive or negative and support faster business insight generation.

## Project Objective
The goal of this project is to build an end-to-end sentiment analysis workflow using real Amazon review data. The project loads and cleans text data, explores review patterns visually, converts text into TF-IDF features, trains a Logistic Regression classifier, evaluates model performance, and compares the baseline against a zero-shot LLM benchmark.

## Dataset
- Source: `amazon_polarity` from Hugging Face
- Task: Binary sentiment classification
- Labels:
  - `0` = negative
  - `1` = positive
- License: Apache 2.0

## Project Workflow
1. Load real Amazon review data from Hugging Face.
2. Combine title and content into a single review text field.
3. Clean and normalize text.
4. Explore the dataset with visualizations.
5. Transform text using TF-IDF vectorization.
6. Train a Logistic Regression classifier.
7. Evaluate performance with accuracy, Macro F1, recall, and confusion matrix.
8. Compare results with a zero-shot LLM baseline.

## Files
- `amazon_sentiment_project.py`: end-to-end Python script for the project
- `requirements.txt`: Python dependencies
- `.gitignore`: excludes cache and notebook checkpoint files

## How To Run
Install dependencies:

```bash
pip install -r requirements.txt
```

Run the project:

```bash
python3 amazon_sentiment_project.py
```

## Example Outputs
The project can produce:
- sentiment distribution charts
- review length visualizations
- confusion matrix
- model comparison chart
- final recommendation summary

## Recommendation
TF-IDF + Logistic Regression is the recommended production baseline for this project because it is fast, interpretable, and inexpensive to deploy. A zero-shot LLM is useful as a benchmark, but it is slower and generally less practical for high-volume inference.

## Suggested Repository Structure
```text
Amazon-Reivews-Sentiment-Analysis/
├── amazon_sentiment_project.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Disclaimer: This project is for educational and portfolio demonstration purposes only. It uses the publicly available `amazon_polarity` dataset and is not affiliated with or endorsed by Amazon.

