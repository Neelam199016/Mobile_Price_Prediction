# 📱 Mobile Price Prediction Using Machine Learning

![Python](https://img.shields.io/badge/Python-3.14-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-green)
![Status](https://img.shields.io/badge/Project-Completed-success)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 1. Project Overview
Mobile Price Prediction is a machine learning project developed to predict the approximate price of a smartphone based on its technical specifications.
The project uses Python, data analysis, data visualization, and machine learning regression algorithms to estimate mobile phone prices.

## 🎯 2. Project Objectives
- Understand and analyze mobile phone data.
- Clean and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Visualize relationships between mobile features and prices.
- Train machine learning regression models.
- Compare model performance.
- Save the best-performing trained model.

## 📊 3. Dataset Description
The dataset contains **541 mobile phone records** and 11 columns after removing an unnecessary index column.

### Features
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

## 🛠️ 4. Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib
- OpenPyXL

## 🔄 5. Project Workflow
1. Data loading
2. Data cleaning and preprocessing
3. Exploratory Data Analysis
4. Data visualization
5. Feature encoding
6. Model training
7. Model evaluation
8. Model comparison
9. Model saving

## 🤖 6. Machine Learning Algorithms
### Linear Regression
A supervised machine learning algorithm used as a baseline for predicting mobile phone prices.

### Random Forest Regression
An ensemble learning algorithm that combines multiple decision trees to make predictions.

## 📈 7. Model Performance
The models were evaluated using MAE, RMSE, and R² Score.
| Evaluation Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | 2204.64 | 1781.42 |
| RMSE | 6341.00 | 4570.94 |
| R² Score | 70.83% | 84.84% |

### Best Model
**Random Forest Regression** performed better on the test dataset, achieving an R² score of approximately **84.84%**.

## 📉 8. Exploratory Data Analysis
Ten visualizations were created:
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

All graphs are available in the `images` folder.

## 💾 9. Project Files
| File | Description |
|---|---|
| `mobile_price_prediction.ipynb` | Main Jupyter Notebook |
| `Processed_Flipdata.xlsx` | Dataset |
| `Project_Report.md` | Detailed project report |
| `random_forest_model.pkl` | Trained Random Forest model |
| `model_comparison.xlsx` | Model comparison results |
| `Mobile_Price_Prediction_Presentation.pptx` | Project presentation |
| `images/` | Project visualizations |

## ▶️ 10. How to Run the Project
### Step 1: Clone the repository
```bash
git clone https://github.com/Neelam199016/Mobile_Price_Prediction.git
```

### Step 2: Open the project folder
```bash
cd Mobile_Price_Prediction
```

### Step 3: Install the required libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter ipykernel joblib
```

### Step 4: Open Jupyter Notebook
```bash
jupyter notebook
```
Open `mobile_price_prediction.ipynb` and run the cells in order.

## 🏁 11. Conclusion
This project demonstrates the practical application of machine learning for predicting smartphone prices based on their specifications.
Two regression algorithms were implemented and compared. Random Forest Regression achieved better results, with an R² score of approximately 84.84%.
The trained model was saved for future use.

## 🚀 12. Future Scope
- Add more mobile phone records.
- Experiment with additional machine learning algorithms.
- Perform hyperparameter tuning.
- Develop a web application for price prediction.
- Update the dataset regularly.

## 👩‍💻 Author  **Neelam**

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
