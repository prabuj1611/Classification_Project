# **Classification Project: Song Recommendation & Income Prediction**

*This project demonstrates the application of supervised learning algorithms—K-Nearest Neighbors and Naive Bayes—to two real-world classification problems:*

- *Predicting music preferences*

- *Categorizing income levels*

**I. K-Nearest Neighbors – Will George Like This Song?**

Objective: Use song attributes (danceability, energy, valence, etc.) to predict whether a user (George) would like a given song.

**Key Steps:**

- Loaded and explored spotify_2023.csv and spotify.csv.

- Selected a known or preferred song and extracted its features.

- Cleaned, normalized, and matched variable formats across datasets.

- Conducted t-tests for variable selection.

- Trained a KNN classifier with k=7, then tuned k using validation accuracy.

- Identified the nearest neighbors and evaluated model predictions.


**Tools & Techniques:**

- Pandas, NumPy, Scikit-learn, Matplotlib

- StandardScaler(), KNeighborsClassifier(), and cross-validation

- t-tests for feature significance


# **II.Naive Bayes – Income Classification**

**Objective:**

Predict income categories (High, Medium, Low) using demographic and transaction features from a credit card dataset.

**Key Steps:**

- Loaded and prepared AER_credit_card_data.csv.

- Binned income and numeric variables using equal-frequency binning.

- Converted categorical and numerical predictors into factors.

- Partitioned the data into training and validation sets (60/40 split).

- Visualized variables using proportional barplots to identify weak predictors.

- Trained a Naive Bayes classifier and evaluated it using confusion matrices.

- Extracted top 100 predicted “High income” cases for business use-case demonstration.

- Performed record-level prediction with associated probability outputs.


**Tools & Techniques:**

- Pandas, Scikit-learn (GaussianNB), Seaborn

- Confusion matrix analysis

- Business interpretation of model results

**Key Takeaways**

- KNN can offer intuitive prediction for preference-based problems like music, but is sensitive to scale and irrelevant features.

- Naive Bayes is fast and interpretable for categorical classification tasks, especially after careful binning and variable selection.

- Visualization and feature selection significantly improve model interpretability and accuracy.

- Business application of predictions (e.g., identifying high-income prospects) provides real-world value.