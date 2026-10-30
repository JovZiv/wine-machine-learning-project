# 🍷 Wine Machine Learning Project


## Project Overview

This project explores the relationship between wine prices and professional ratings using data analysis and machine learning.

The main objective was to investigate whether more expensive wines tend to receive higher ratings and whether machine learning models can predict wine ratings based on selected features.


## 🎯 Research Question

**Do higher-priced wines tend to receive higher professional ratings?**

## 📊 Dataset

The project uses the Wine Enthusiast dataset (`wine-price.csv`).

The target variable was `points`, representing the professional wine rating.


## ⚙️ Methodology

The project followed these main steps:

1. **Data Cleaning:** Removed records with missing prices and duplicate rows.
2. **Exploratory Data Analysis (EDA):** Investigated price distributions, ratings and the relationship between price and points.
3. **Data Preparation:** Handled missing categorical values using the mode and converted categorical features into numerical format using One-Hot Encoding.
4. **Train-Test Split:** Divided the dataset into 80% training data and 20% testing data.
5. **Model Training:** Trained and compared different machine learning model configurations.
6. **Model Evaluation:** Evaluated performance using Mean Absolute Error (MAE) and R².
7. **Hyperparameter Tuning:** Used GridSearchCV and cross-validation to optimise the Random Forest model.


## 🤖 Machine Learning Models

Two algorithms were explored across three model configurations:

| Algorithm         | Features                | MAE   | R²    |
| ----------------- | ----------------------- | ----- | ----- |
| Linear Regression | Price                   | 2.239 | 0.191 |
| Linear Regression | Price, Variety, Country | 2.138 | 0.258 |
| Random Forest     | Price, Variety, Country | 1.848 | 0.428 |

**Random Forest achieved the best performance**, with an average prediction error of approximately 1.85 rating points and an R² of 0.428.


## 🔍 Key Findings

- Wine ratings generally increased across higher price ranges.
- The Pearson correlation between price and ratings was approximately 0.416, indicating a moderate positive relationship.
- Price was the most important feature in the Random Forest model, accounting for approximately 86.82% of feature importance.
- Variety and country also contributed to the model's predictions.


## 💡 Conclusion

The analysis suggests that higher-priced wines tend to receive higher professional ratings. However, price alone does not explain wine ratings completely.

The Random Forest model performed better than Linear Regression, showing that more complex relationships between features can help improve predictions.

**Importantly, correlation does not imply causation, and a higher price does not necessarily mean a better wine.**


## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Machine Learning


## 📄 Project Presentation

[View the Wine Machine Learning Project Presentation (PDF)](https://drive.google.com/file/d/1KospnSs6nDIdQHul-Y_fxkckQ4C-Bisl/view?usp=sharing)


## 🚀 Future Improvements

- Explore additional features that could influence wine ratings.
- Test other machine learning algorithms.
- Experiment with further hyperparameter tuning.
- Evaluate whether additional features can improve prediction performance.

  
