# Course Review Sentiment Analysis
A sentiment analysis project that automatically classifies customer reviews as positive or negative using machine learning.

This project analyzes user course reviews to predict sentiment using **text data**.  
It includes **multiclass rating prediction (1–5)** and **binary sentiment classification (Good/Bad)**.

## Dataset
- Source: `user_courses_review_09_2023.csv`
- Columns used: `review_comment`, `review_rating`
- Missing values removed; ratings cleaned and converted to integers

## Approach
- Text preprocessing: lowercase, remove URLs, numbers, punctuation
- TF-IDF vectorization (unigrams + bigrams)
- Handle class imbalance with RandomOverSampler
- Model: Multinomial Naive Bayes
- Evaluation: Accuracy and classification report

## Binary Sentiment Logic
- Ratings 4–5 → Good  
- Ratings 1–3 → Bad

## Results
The model predicts sentiment effectively, showing good performance on both multiclass and binary tasks.

