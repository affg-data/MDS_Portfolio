# Predicting Spotify Song Popularity

Predicting whether a song will become popular is a challenging machine learning problem because popularity is influenced by many musical and non-musical factors. This project explores whether Spotify audio features and playlist metadata can be used to classify songs as **popular** or **not popular** using logistic regression.

The analysis follows a complete binary classification workflow, including exploratory data analysis, feature engineering, model development, model comparison, and performance evaluation.

---

## Project Objective

The objective of this project is to develop and evaluate logistic regression models that predict song popularity based on measurable audio characteristics and playlist information.

Key questions explored include:

- Which audio features are associated with popular songs?
- Can logistic regression effectively classify song popularity?
- Which combination of predictors provides the best predictive performance?

---

## Dataset

The project uses the **Spotify Songs** dataset from TidyTuesday, containing thousands of tracks with audio characteristics, playlist information, and popularity scores.

### Features include

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
- Musical Key
- Mode
- Playlist Genre
- Playlist Subgenre

Song popularity was transformed into a **binary target variable** by classifying tracks as either **Popular** or **Not Popular**.

---

## Project Workflow

The notebook follows a complete machine learning pipeline:

1. Data cleaning and preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature engineering
4. Logistic regression model development
5. Model comparison
6. Model evaluation
7. Prediction and interpretation

---

## Exploratory Data Analysis

The EDA examines both the structure of the dataset and relationships among variables through:

- Dataset overview
- Missing value analysis
- Class balance
- Distribution of continuous variables
- Correlation analysis
- Feature relationships
- Boxplots and scatterplots

### Correlation Matrix

<p align="center">
  <img src="figures/correlation_heatmap.png" width="700">
</p>

The correlation heatmap highlights relationships among continuous audio features and identifies variables that are positively or negatively associated with song popularity.

---

## Model Development

Several logistic regression models were developed using different combinations of predictor variables, ranging from simple baseline models to more comprehensive specifications that incorporate both continuous and categorical features.

Model performance was compared using classification metrics and ROC analysis to identify the strongest-performing model.

---

## Model Evaluation

The final logistic regression model was evaluated using a confusion matrix and Receiver Operating Characteristic (ROC) curve.

### Confusion Matrix

<p align="center">
  <img src="figures/model_4_confusion_matrix.png" width="700">
</p>

The confusion matrix summarizes the classification results by comparing predicted and actual song popularity labels, illustrating both correct classifications and prediction errors.

---

### ROC Curve

<p align="center">
  <img src="figures/roc_curve.png" width="700">
</p>

The ROC curve evaluates the model's ability to distinguish between popular and non-popular songs across different classification thresholds. The final model achieved an **Area Under the Curve (AUC) of 0.648**, indicating moderate predictive performance above random guessing.

---

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

---

## Repository Structure

```text
Predicting_Spotify_Song_Popularity/
│
├── notebook/
│   └── Predicting_Spotify_Song_Popularity.ipynb
│
├── figures/
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── class_balance.png
│
├── raw_data/
│   └── spotify_songs.csv
│
└──README.md
```

---

## Key Takeaways

- Audio characteristics contain useful information for predicting song popularity.
- Logistic regression provides an interpretable baseline for binary music classification.
- Combining multiple predictor types improves classification performance over simpler models.
- While the final model demonstrates meaningful predictive ability (AUC = **0.648**), song popularity is influenced by additional factors beyond audio features alone, including marketing, artist recognition, and listener behavior.

---

*This project was completed as part of the Master of Data Science program at the University of Pittsburgh. It demonstrates the application of logistic regression to a real-world music dataset while following a complete machine learning workflow from exploratory data analysis through model evaluation.*
