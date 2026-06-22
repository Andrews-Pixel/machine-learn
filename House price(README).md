# 🏠 House Price Prediction — Linear Regression
A machine learning project that predicts **California housing prices** using Linear Regression, with Ridge and Lasso regularization comparisons. Built with scikit-learn, pandas, and seaborn.


## 📌 Project Overview
This project walks through a complete ML pipeline — from raw data exploration and outlier detection to model training, evaluation, and visualization — to predict median house prices based on features like income, house age, room count, population, and geographic coordinates.


## 📂 Dataset
Source:California Housing Dataset (`lr_dataset.csv`)
Target Variable:`House_price`
Features Used:


| Feature | Description |
|---|---|
| `MedInc` | Median income in block group |
| `HouseAge` | Median house age in block group |
| `AveRooms` | Average number of rooms per household |
| `AveBedrms` | Average number of bedrooms per household |
| `Population` | Block group population |
| `AveOccup` | Average number of household members |
| `Latitude` | Block group latitude |
| `Longitude` | Block group longitude |


## 🔧 Tech Stack
Built with **Python 3.x**.
**pandas** and **NumPy** for data manipulation.
**scikit-learn** for model training and evaluation.
**Matplotlib** and **Seaborn** for data visualization.

## 🔄 Project Workflow
Data Loading → EDA → Outlier Detection (IQR) → Correlation Analysis
       → Train/Test Split → Model Training → Evaluation → Visualization

### 1. Exploratory Data Analysis (EDA)
- Inspected shape, data types, null values, and summary statistics
- Selected relevant features for modeling

### 2. Outlier Detection
- Applied **IQR (Interquartile Range)** method to detect outliers
- Computed Q1, Q3, lower and upper bounds across all features

### 3. Correlation Analysis
- Generated a **correlation matrix** to understand feature relationships
- Visualized using a **Seaborn heatmap** with `viridis` colormap

### 4. Model Training
- Split data: **80% training / 20% testing**
- Trained a **Linear Regression** model using scikit-learn
- Also applied **Ridge** and **Lasso** regularization (alpha=1.0) for comparison

### 5. Model Evaluation

| Metric | Description |
|---|---|
| **MSE** | Mean Squared Error |
| **RMSE** | Root Mean Squared Error |
| **R² Score** | Coefficient of Determination |
| **Adjusted R²** | Penalizes for number of features |

### 6. Results Visualization
- Plotted **Actual vs Predicted** values as a line chart to assess model fit


## 📊 Model Comparison
| Model | Regularization | Notes |
| Linear Regression | None | Baseline model |
| Ridge Regression | L2 (α=1.0) | Reduces coefficient magnitude |
| Lasso Regression | L1 (α=1.0) | Can zero out coefficients |



### Prerequisites
pip install pandas numpy matplotlib seaborn scikit-learn


## 📁 Project Structure
📦 house-price-linear-regression
 ┣ 📓 House_price_linear-Regression_.ipynb
 ┣ 📄 lr_dataset.csv


## 👤 Author

**Andrews Martin**
- 💼 LinkedIn: [andrewsmartin30](https://linkedin.com/in/andrewsmartin30)
