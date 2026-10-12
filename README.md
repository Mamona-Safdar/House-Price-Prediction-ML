# House-Price-Prediction-ML
# House Price Prediction | Machine Learning

## Project Overview

This project predicts residential house prices using **Random Forest Regression** and the Kaggle House Prices dataset.

The goal is to explore the factors influencing house prices, prepare the data for machine learning, train a regression model, and generate predictions for unseen houses.

## Dataset

**Source:** [Kaggle — House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

- Training data: 1,460 houses
- Test data: 1,459 houses
- Input features: 79
- Target variable: `SalePrice`

## Project Workflow

1. **Data Inspection:** Explored the dataset and identified missing values.
2. **Data Cleaning:** Handled missing numerical and categorical values.
3. **Exploratory Data Analysis:** Investigated house prices, property quality, living area, neighborhoods, and construction years.
4. **Feature Preprocessing:** Applied one-hot encoding to categorical features and log transformation to the target variable.
5. **Model Training:** Trained a Random Forest Regressor using scikit-learn.
6. **Model Improvement:** Adjusted hyperparameters to reduce overfitting.
7. **Model Evaluation:** Used RMSE and 5-fold cross-validation.
8. **Final Predictions:** Generated predictions for 1,459 test houses and exported `submission.csv`.

## Model Performance

| Metric | Result |
|---|---|
| Baseline Validation Log RMSE | 0.14600 |
| Improved Validation Log RMSE | 0.14585 |
| Mean 5-Fold CV Log RMSE | 0.14466 |
| CV Standard Deviation | 0.00961 |

Lower RMSE indicates better prediction accuracy.

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Random Forest Regression
- Git and GitHub

## Project Structure

```text
House-Price-Prediction-ML/
├── House-Price-Prediction-ML.py
├── README.md
└── LICENSE
```

The dataset files (`train.csv`, `test.csv`, and `data_description.txt`) must be downloaded separately from Kaggle and placed alongside the Python script to run it locally.

## How to Run

1. Download the dataset from Kaggle.
2. Install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

3. Place the dataset files in the project folder.
4. Run:

```bash
python House-Price-Prediction-ML.py
```

5. The script generates a `submission.csv` file containing predicted house prices.

## Key Learnings

Through this project, I practiced building an end-to-end machine learning regression workflow, including handling missing data, exploring feature relationships, training models, identifying overfitting, improving hyperparameters, and evaluating model performance with cross-validation.


