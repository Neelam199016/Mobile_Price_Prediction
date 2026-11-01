Mobile Price Prediction Using Machine Learning

1. Introduction

Mobile phones have become an essential part of our daily lives. Different mobile brands offer smartphones with various features, specifications, and price ranges.Choosing a mobile phone can be difficult because prices depend on several factors, such as RAM, internal storage, battery capacity, camera quality, processor, and mobile brand.This project aims to develop a machine learning model that predicts the price of a mobile phone based on its specifications. The project uses Python, data analysis, data visualization, and machine learning algorithms to estimate mobile prices.Two machine learning algorithms, Linear Regression and Random Forest Regression, are used and compared to identify the better-performing model.

2. Problem Statement

Selecting a suitable mobile phone within a specific budget is challenging because smartphones have different specifications and prices.The price of a mobile phone depends on several features, including brand, model, RAM, internal storage, battery capacity, camera specifications, and processor.The main problem addressed by this project is to build a machine learning model that can predict the approximate price of a mobile phone using its technical specifications.The model will help users understand how mobile phone features influence prices and estimate the price of a smartphone before purchasing it.

3. Objectives

The main objectives of this project are:
To collect and understand mobile phone specification data.
To clean and preprocess the dataset.
To perform exploratory data analysis (EDA) using Python.
To visualize the relationship between mobile phone features and prices.
To apply Linear Regression and Random Forest Regression algorithms.
To evaluate and compare the performance of both machine learning models.
To identify the better-performing model for mobile price prediction.
To save the trained machine learning model for future predictions.

## 4. Dataset Description

The dataset used in this project is named `Processed_Flipdata.xlsx`.
It contains information about 541 mobile phones and their technical specifications. The dataset has 11 columns after removing the unnecessary index column.
The important features included in the dataset are:

**Model:** Mobile phone model name.
**Colour:** Available colour of the mobile phone.
**Memory:** Internal storage capacity.
**RAM:** Random Access Memory.
**Battery:** Battery capacity.
**Rear Camera:** Rear camera specification.
**Front Camera:** Front camera specification.
**AI Lens:** AI lens information.
**Mobile Height:** Height of the mobile phone.
**Processor:** Mobile phone processor.
**Prize:** Target variable representing the mobile phone price.

The target variable is `Prize`, which is used to train the machine learning models.
The dataset contains 541 records and has no missing values after the initial data inspection.

## 5. Data Cleaning and Preprocessing

Data cleaning and preprocessing are important steps in preparing the dataset for machine learning.

The following operations were performed:
**Removing unnecessary column:** The `Unnamed: 0` column was removed because it was not useful for prediction.
**Checking missing values:** The dataset was checked for missing values. No missing values were found.
**Checking duplicate records:** Duplicate records were checked during data inspection.
**Converting camera specifications:** The `Rear Camera` and `Front Camera` columns were converted from text values (such as MP) into numerical values.
**Separating features and target:** The input features were stored in `X`, and the target column `Prize` was stored in `y`.
**Encoding categorical data:** Categorical features such as Model, Colour, and Processor were converted into numerical values using One-Hot Encoding.
After preprocessing, the encoded feature dataset contained 541 rows and 592 columns.

## 6. Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) was performed to understand the dataset and identify patterns and relationships between mobile phone specifications and prices.
Python libraries such as Pandas, Matplotlib, and Seaborn were used for data analysis and visualization.

The following graphs were created:
1. Price Distribution – Shows the distribution of mobile phone prices.
2. Price Boxplot – Helps identify the spread of prices and possible outliers.
3. Top Mobile Models – Displays the most frequently occurring mobile models.
4. Average Price by RAM – Shows how average mobile prices vary with RAM capacity.
5. Average Price by Storage – Compares average prices across storage capacities.
6. Average Price by Battery – Shows the relationship between battery capacity and average price.
7. Average Price by Processor – Compares average prices for different processors.
8. Correlation Heatmap – Displays the correlation between numerical features.

These visualizations helped in understanding the dataset and the factors that may influence mobile phone prices.
All eight EDA graphs were saved in the `images` folder.

## 7. Model Building

After completing data cleaning, preprocessing, and exploratory data analysis, machine learning models were developed to predict mobile phone prices.
The dataset was divided into training and testing sets using the `train_test_split()` function.
- Training data: 80% (432 records)
- Testing data: 20% (109 records)
- Random state: 42

Two machine learning algorithms were implemented:
### 7.1 Linear Regression

Linear Regression is a supervised machine learning algorithm used to predict continuous numerical values.
It was applied to estimate mobile phone prices based on the available specifications.

### 7.2 Random Forest Regression
Random Forest Regression is an ensemble learning algorithm that combines multiple decision trees to make predictions.
It was also trained using the processed dataset to predict mobile phone prices.
Both models were trained using the same training and testing data so that their performance could be compared fairly.

## 8. Model Evaluation and Comparison

The performance of both machine learning models was evaluated using three evaluation metrics:
**Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices. Lower values indicate better performance.
**Root Mean Squared Error (RMSE):** Measures prediction errors while giving more weight to larger errors. Lower values indicate better performance.
**R² Score:** Measures how well the model explains variations in the target variable. A value closer to 1 indicates better performance.

### 8.1 Model Performance Results
| Evaluation Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | 2204.64 | 1781.42 |
| RMSE | 6341.00 | 4570.94 |
| R² Score | 0.7083 | 0.8484 |

### 8.2 Comparison
The Random Forest Regression model performed better than Linear Regression on the test dataset.
- Random Forest achieved a lower MAE and RMSE.
- Random Forest achieved a higher R² score of approximately 84.84%.
- Linear Regression achieved an R² score of approximately 70.83%.
Therefore, Random Forest Regression was selected as the better-performing model for this project.

## 9. Feature Importance and Visualization

Feature importance was analyzed using the Random Forest Regression model to understand which mobile phone specifications contribute most to price prediction.
The `feature_importances_` attribute of the trained Random Forest model was used to calculate the importance of each feature.

A bar chart showing the top 10 important features was created and saved as:
`images/09_feature_importance.png`
An Actual vs Predicted Price graph was also created to compare the actual mobile phone prices with the prices predicted by the Random Forest model.

The graph was saved as:
`images/10_actual_vs_predicted.png`
These visualizations help explain the model's behavior and show how closely its predictions match the actual prices.

## 10. Model Saving

After evaluating both machine learning algorithms, the Random Forest Regression model was selected because it achieved better performance.
The trained Random Forest model was saved using the Python `joblib` library.
The saved model filename is:
`random_forest_model.pkl`
The model can be loaded later and used to make predictions without training it again.

The model comparison results were also saved in an Excel file named:
`model_comparison.xlsx`
These files help preserve the trained model and its evaluation results for future use.

## 11. Conclusion

The Mobile Price Prediction project successfully demonstrates how machine learning can be used to estimate mobile phone prices based on their specifications.
The dataset was cleaned and preprocessed, followed by exploratory data analysis and visualization. Two machine learning algorithms, Linear Regression and Random Forest Regression, were implemented and evaluated.
The results showed that Random Forest Regression performed better than Linear Regression, achieving an R² score of approximately 84.84%.
The trained Random Forest model was saved for future use. This project helped demonstrate the practical application of Python, data analysis, data visualization, and machine learning in solving a real-world prediction problem.

## 12. Future Scope

This project can be improved further in several ways:
**More Data:** Add more mobile phone records from different brands and models to improve model performance.
**Additional Algorithms:** Experiment with other machine learning algorithms such as Decision Tree, Gradient Boosting, and XGBoost.
**Hyperparameter Tuning:** Optimize model settings to improve prediction accuracy.
**User Interface:** Develop a simple web application where users can enter mobile specifications and receive an estimated price.
**Regular Updates:** Update the dataset regularly to reflect changes in mobile phone prices and new smartphone models.

These improvements can make the Mobile Price Prediction system more accurate, useful, and practical.