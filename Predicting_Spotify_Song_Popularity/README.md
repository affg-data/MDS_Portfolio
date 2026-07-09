# Predicting Spotify Song Popularity Using Logistic Regression

## Overview

Can a song's popularity be predicted using its audio characteristics?

This project develops a **logistic regression classification model** to predict whether a Spotify track is likely to be **popular** or **not popular** based on audio features and playlist metadata.

The project follows a complete machine learning workflow, including exploratory data analysis, feature engineering, model development, and performance evaluation.

---

## Objective

The goal of this project is to determine whether song popularity can be predicted from measurable musical characteristics and to identify which features contribute most to the prediction.

---

## Dataset

The analysis uses the **Spotify Songs** dataset, which contains information on thousands of tracks, including:

- Danceability
- Energy
- Loudness
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo
- Duration
- Playlist genre
- Playlist subgenre
- Musical key
- Mode

Song popularity was converted into a **binary classification problem** by categorizing tracks as either **popular** or **not popular**.

---

## Project Workflow

The notebook follows these major steps:

1. Data preparation
2. Exploratory Data Analysis (EDA)
3. Feature engineering
4. Logistic regression model development
5. Model evaluation
6. Prediction and interpretation

---

## Exploratory Data Analysis

The EDA includes:

- Dataset overview
- Missing value analysis
- Class balance visualization
- Distribution of numerical variables
- Correlation analysis
- Feature relationships
- Boxplots and scatterplots

---

## Machine Learning Model

**Model**

- Logistic Regression

**Evaluation**

- Confusion Matrix
- ROC Curve
- ROC AUC
- Precision
- Recall
- Classification Accuracy

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Statsmodels
- Jupyter Notebook

---

## Repository Structure

```text
Predicting_Spotify_Song_Popularity/
│
├── notebook/
├── figures/
└── README.md
```

---

## Key Takeaways

The project demonstrates a complete binary classification workflow, from data exploration and preprocessing through model development and evaluation.

Beyond predicting song popularity, the analysis illustrates how audio features and playlist characteristics can be used to better understand patterns associated with successful tracks.

---

## About This Project

*This project was completed as part of the Master of Data Science program at the University of Pittsburgh. It demonstrates the application of logistic regression to a real-world music dataset while following a reproducible machine learning workflow.*
