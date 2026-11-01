# 📱 Mobile Price Prediction Using Machine Learning

## 1. Project Overview
Mobile Price Prediction is a machine learning project that predicts the approximate price of a smartphone based on its technical specifications.
The project uses Python, data analysis, data visualization, and regression algorithms to estimate mobile phone prices.

## 2. Project Objectives
- Analyze mobile phone specifications and prices.
- Clean and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Visualize relationships between mobile features and prices.
- Build machine learning regression models.
- Compare model performance.
- Save the best-performing trained model.

## 3. Dataset Description
The dataset contains **541 mobile phone records** and 11 columns after removing an unnecessary index column.
Important features include:
- Model
- Colour
- Memory
- RAM
- Battery
- Rear Camera
- Front Camera
- AI Lens
- Mobile Height
- Processor
- Prize (Target Variable)

## 4. Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib

## 5. Project Workflow
1. Data loading
2. Data cleaning and preprocessing
3. Exploratory Data Analysis
4. Data visualization
5. Feature encoding
6. Model training
7. Model evaluation
8. Model comparison
9. Model saving

## 6. Machine Learning Algorithms
Two regression algorithms were implemented:

### Linear Regression
Used as a baseline model for predicting mobile phone prices.

### Random Forest Regression
An ensemble learning algorithm that combines multiple decision trees to improve prediction performance.

## 7. Model Performance
| Evaluation Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | 2204.64 | 1781.42 |
| RMSE | 6341.00 | 4570.94 |
| R² Score | 70.83% | 84.84% |

**Result:** Random Forest Regression performed better than Linear Regression on the test dataset.

## 8. Project Visualizations
The following visualizations were created and saved in the `images` folder:
1. Price Distribution
2. Price Boxplot
3. Top Mobile Models
4. Average Price by RAM
5. Average Price by Storage
6. Average Price by Battery
7. Average Price by Processor
8. Correlation Heatmap
9. Feature Importance
10. Actual vs Predicted Prices

## 9. Saved Model and Outputs
- `random_forest_model.pkl` – Trained Random Forest model.
- `model_comparison.xlsx` – Model evaluation results.
- `Project_Report.md` – Detailed project report.
- `Mobile_Price_Prediction_Presentation.pptx` – Project presentation.

## 10. How to Run the Project
1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Create and activate a Python virtual environment.
4. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter ipykernel joblib
```

5. Open `mobile_price_prediction.ipynb` in VS Code.
6. Select the Python virtual environment as the notebook kernel.
7. Run the notebook cells in order.

## 11. Conclusion
This project demonstrates the practical application of machine learning in predicting smartphone prices.
Random Forest Regression achieved an R² score of approximately 84.84%, making it the better-performing model in this experiment.

## 12. Future Scope
- Add more mobile phone datasets.
- Experiment with additional machine learning algorithms.
- Perform hyperparameter tuning.
- Develop a web application for mobile price prediction.
- Update the dataset regularly.

**Project:** Mobile Price Prediction Using Machine Learning

**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
