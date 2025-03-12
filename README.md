# Hate Speech Message Classification

## Objectives

The goal of this project is to develop a complete machine learning pipeline for classifying hate speech messages. The project will detail the necessary steps for text classification and the evaluation of the results.

### Key Objectives:
- Select an appropriate machine learning technique for classification.
- Analyze and compare different supervised learning models for hate speech classification.
- Evaluate the results of each model based on precision, recall, and F1-score.

## Task Description

SureTech Innovations aims to implement a hate speech message classifier. To achieve this, you need to train several classification models, evaluate their performance, and choose the best-performing model.

The dataset you will use is the simplified **HateSpeech dataset** available at: [HateSpeech Dataset](https://github.com/almudenaris/TAA/blob/main/out.csv).

### Steps to Complete the Activity:

1. **Exploratory Data Analysis (EDA)**:
   - What machine learning task is being solved? What prior analysis is needed to determine whether it is possible to build the model? Perform an adequate exploratory data analysis based on the task to be solved and the provided dataset. Describe the necessary steps to prepare and analyze the data.

2. **Model Selection**:
   - Based on the task and dataset characteristics, decide which machine learning algorithms should be used. Implement three different models, train them, and justify the choice of algorithms for this specific task.

3. **Model Evaluation**:
   - Explain the evaluation metrics you will use to assess the performance of the models. Justify your choice of metrics. How should the models be evaluated? Evaluate the models trained in the previous step and explain the results.

## Dataset

The dataset provided has been adapted for this activity with the following preprocessing steps:

- Removal of missing and duplicate entries
- Removal of URLs, emojis, and mentions of newspapers
- Removal of empty rows
- Data cleaning and standardization:
    - Convert all text to lowercase
    - Remove punctuation
    - Remove numbers
    - Remove extra spaces
    - Remove words shorter than 2 characters
    - Remove stopwords
    - Tokenization
    - Lemmatization

- Feature extraction process:
    - Count of positive words (A)
    - Count of negative words (B)
    - Count of the most common bigrams (C)
    - Count of user mentions (D)
    - Sentiment category based on 'pysentimiento' library in Spanish (E)

- Standardization of features (A_t, ..E_t)
- Combination of features (f1*fi) (iA..iE) (Value1,..Value10)
