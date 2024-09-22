

# Quora Question Pair Similarity

This project predicts whether two questions on Quora are duplicates using natural language processing (NLP) techniques and machine learning models.

## Dataset
- **Source**: Kaggle's Quora Question Pairs dataset.
- **Features**:
  - `qid1`, `qid2`: Unique question IDs.
  - `question1`, `question2`: Text of the questions.
  - `is_duplicate`: Binary target indicating whether the questions are duplicates.

## Problem Statement
- **Objective**: Predict whether a pair of questions are duplicates to avoid redundant answers on Quora.

## Key Techniques
1. **Data Preprocessing**:
   - Cleaned and preprocessed text data (removed stopwords, applied stemming).
   - Generated features like word length, common words, and word share between question pairs.

2. **Advanced Feature Engineering**:
   - Extracted additional features like **fuzz ratio**, **word share**, and **noun similarity** using NLP and fuzzy matching.
   - Applied **TF-IDF Vectorization** to text data for both questions.

3. **Dimensionality Reduction**:
   - Applied **t-SNE** for 2D and 3D visualization of clusters formed by similar questions.

4. **Modeling**:
   - Implemented **Logistic Regression** and **XGBoost** to classify whether a question pair is duplicate or not.

## Results
- **Evaluation Metrics**: Used log-loss and confusion matrix to evaluate model performance.
- **Best Model**: Achieved competitive log-loss and accuracy using XGBoost.

## Conclusion
The project successfully predicts duplicate questions on Quora by leveraging NLP and machine learning models. Advanced features like TF-IDF and fuzzy matching improved prediction accuracy.

