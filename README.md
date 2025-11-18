# Kaggle Titanic Survival Prediction

This project is a complete data science workflow to predict passenger survival on the Titanic, based on Kaggle's famous competition. I achieved a **76.5% accuracy** on the final test set.

---

# Project Goal

The primary goal was to build a machine learning model that could accurately predict whether a passenger survived the Titanic disaster, based on personal data like age, sex, and ticket class.

---

# My Process

My workflow followed the standard data science pipeline, from cleaning the raw data to evaluating the final model.

1. Data Cleaning & Preprocessing
Before any modeling, the data had to be made clean and complete.

Missing Values: Handled missing data in key columns like Age (e.g., filled with mean).

Duplicates: Ensured data integrity by removing any duplicate rows.

Categorical Encoding: Converted all non-numeric columns (Sex, Embarked, Deck) into a numerical format that the model could understand (e.g., male=1, female=0).

2. Feature Engineering & Selection
I created new, more informative features from the existing data.

Feature Extraction: Created a Deck feature by extracting the first letter from the Cabin column.

Feature Selection: Removed irrelevant columns (like PassengerId ,name and Ticket) that would not help the model make a prediction.

3. Model Training & Evaluation
With a clean dataset, I built and tested the models.

Train/Validation Split: I split the train.csv data (which contains the Survived label) into a training set and a validation set. This allowed me to test my model's performance locally before checking the final score.

Model Selection: I trained and compared several different classification models (e.g., Logistic Regression, Random Forest, etc.) to find the best performer.

Feature Scaling: I applied StandardScaler to the training and validation data, which is a crucial step for many models.

Model Evaluation: I used Accuracy as the primary performance metric. I also analyzed the Confusion Matrix, Precision, and Recall to understand how well the model predicted both survival and non-survival.

Cross-Validation: To ensure the model's performance was stable and not just a one-time success, I performed K-Fold Cross-Validation (with 10 folds). This gave a more reliable average accuracy score.

---

# Results & Conclusion

The final model achieved a **76.5% accuracy** on the Kaggle test set. This project was a great introduction to the end-to-end machine learning pipeline, especially the importance of feature engineering, which had the biggest impact on the score.

---

# Tools Used

* **Python**
* **Pandas** (for data manipulation)
* **NumPy** (for numerical operations)
* **Matplotlib / Seaborn** (for visualization)
* **Scikit-learn** (for modeling and evaluation)
* **Google Colab** (for the development environment)
