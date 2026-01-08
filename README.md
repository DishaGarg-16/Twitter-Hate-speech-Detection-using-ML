# Twitter Sentiment Analysis using Machine Learning

This project implements a machine learning pipeline to perform sentiment analysis on Twitter data. It classifies tweets into three sentiment categories: **Positive**, **Negative**, and **Neutral**.

## Project Overview

The goal of this project is to analyze the sentiment of tweets using various Natural Language Processing (NLP) techniques and Machine Learning algorithms. The notebook walks through the entire process from data loading and cleaning to model training and evaluation.

## Approach

The project follows these key steps:

1.  **Data Preprocessing**:
    *   **Data Loading**: The dataset (`Twitter_Data.csv`) is loaded using Pandas.
    *   **Cleaning**: Handling missing values (`dropna`).
    *   **Text Normalization**: Removing special characters, numbers, and Twitter handles (e.g., `@user`) to clean the text data.

2.  **Exploratory Data Analysis (EDA)**:
    *   Analyzed the distribution of sentiment classes (Positive, Neutral, Negative).
    *   Visualized frequent words using **WordCloud**.

3.  **Feature Extraction**:
    *   Converted textual data into numerical vectors using **TF-IDF (Term Frequency-Inverse Document Frequency) Vectorizer**.

4.  **Model Building**:
    The following Machine Learning classifiers were trained and tested:
    *   **Naive Bayes**
    *   **Logistic Regression**
    *   **Support Vector Machine (SVM)**
    *   **Decision Tree Classifier**

5.  **Model Evaluation**:
    Models were evaluated based on:
    *   **Accuracy Score**
    *   **Confusion Matrix**
    *   **Classification Report** (Precision, Recall, F1-Score)

## Results

The performance of the models was compared, and the observations were:
*   **Best Performers**: **SVM** and **Logistic Regression** achieved the highest accuracy (~94-95%).
*   **Decision Tree**: Performed reasonably well (~89%).
*   **Naive Bayes**: Achieved the lowest accuracy (~75%) and struggled with neutral tweets.

**Best Classifier**: Support Vector Machine (SVM) (Accuracy: ~95.01%)

## Requirements

To run this notebook, you need the following Python libraries installed:

*   `pandas`
*   `numpy`
*   `matplotlib`
*   `seaborn`
*   `scikit-learn`
*   `wordcloud`

## Usage

1.  Ensure you have the required libraries installed.
2.  Open the Jupyter Notebook `Implementation using ML (2).ipynb`.
3.  Run the cells sequentially to execute the pipeline.
4.  The final section consists of a prediction block where you can input custom tweets to test the best performing models.
