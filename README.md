# Twitter Sentiment Analysis

## Overview
This project performs **sentiment analysis on Twitter data** using **Natural Language Processing (NLP)** and **Machine Learning**. The goal is to classify tweets as **positive or negative** based on their textual content. Sentiment analysis is widely used in **social media monitoring, customer feedback analysis, and opinion mining**.

## Objectives
- Perform **text preprocessing** on raw tweet data  
- Convert text into numerical features using **TF-IDF vectorization**  
- Train a **machine learning model** to classify tweet sentiments  
- Evaluate model performance using classification metrics  

## Dataset
The project uses the **Sentiment140 dataset**, which contains **1.6 million labeled tweets**.

| Column | Description |
|------|------|
| target | Sentiment label (0 = Negative, 4 = Positive) |
| ids | Tweet ID |
| date | Tweet date |
| flag | Query flag |
| user | Twitter username |
| text | Tweet content |

Dataset Source: **Kaggle – Sentiment140**

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- NLTK  
- Scikit-learn  

## Project Workflow
**1. Data Collection**  
Downloaded the dataset from Kaggle and loaded it using Pandas.

**2. Data Preprocessing**
- Lowercasing text  
- Removing URLs and special characters  
- Removing stopwords  
- Stemming using Porter Stemmer  

Example:

Original tweet  
`I love this phone! It's amazing 😍`

Processed tweet  
`love phone amaz`

**3. Feature Engineering**  
Used **TF-IDF (Term Frequency – Inverse Document Frequency)** to convert text into numerical vectors.

**4. Model Training**  
The dataset was split into **training and testing sets**, and a machine learning model was trained to predict tweet sentiment.

**5. Model Evaluation**
- Accuracy  
- Confusion Matrix  
- Precision  
- Recall  
- F1 Score  

## Results
The trained model successfully classifies tweets into **positive and negative sentiments**, demonstrating the effectiveness of **NLP and machine learning techniques for social media sentiment analysis**.

## Example Predictions
| Tweet | Predicted Sentiment |
|------|------|
| I love this product | Positive |
| Worst experience ever | Negative |

## Project Structure
