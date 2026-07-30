# 🚗 Car Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.0-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-green?logo=pandas)
![License](https://img.shields.io/badge/License-MIT-yellow)

> A machine learning project to predict the selling price of cars based on various features such as present price, year, kilometers driven, and fuel type.

---

## 🎥 Video Presentation

Watch the video below for a complete walkthrough of the project, from data exploration to model evaluation!

Tape below to open it on youtube

**[![Watch the Video](https://img.youtube.com/vi/ejSVxkmKHUM/maxresdefault.jpg)](https://www.youtube.com/watch?v=ejSVxkmKHUM)**


*(Note: If you are hosting the video on YouTube, you can also embed a thumbnail by replacing the link above with an image link that redirects to your video).*

---

## 📖 About the Project

The objective of this project is to build a predictive model that estimates the selling price of a car. The selling price is determined by several factors, including the car's present price, the year it was purchased, the total kilometers driven, the fuel type, and the type of seller. 

By applying **Linear Regression**, this project demonstrates how to clean data, engineer features, train a machine learning model, and evaluate its performance using real-world automotive data.

---

## 📊 The Dataset

The dataset used for this project contains **301 records** and **9 features**:

| Feature | Description |
| :--- | :--- |
| `Car_Name` | Name of the car model |
| `Year` | Year the car was bought |
| `Selling_Price` | **Target Variable** - The final price the car was sold for |
| `Present_Price` | The current market price of the car |
| `Driven_kms` | Total kilometers driven by the car |
| `Fuel_Type` | Type of fuel (Petrol, Diesel, CNG) |
| `Selling_type` | Type of seller (Dealer, Individual) |
| `Transmission` | Gear transmission type (Manual, Automatic) |
| `Owner` | Number of previous owners (0, 1, or 2) |

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** & **NumPy**: For data manipulation and analysis.
- **Matplotlib** & **Seaborn**: For data visualization and plotting scatter graphs.
- **Scikit-Learn**: For machine learning modeling, data splitting, and evaluation metrics.

---

## 🚀 Project Workflow

### 1. Data Exploration (EDA)
- Checked for missing values using `isnull().sum()` (No missing values found).
- Analyzed the dataset structure using `info()`.
- Explored the distribution of categorical variables using `value_counts()`.

### 2. Data Preprocessing
Machine learning models require numerical input. Categorical variables were encoded into numerical values:
- **Fuel Type:** Petrol $\rightarrow$ 0, Diesel $\rightarrow$ 1, CNG $\rightarrow$ 2
- **Selling Type:** Dealer $\rightarrow$ 0, Individual $\rightarrow$ 1
- **Transmission:** Manual $\rightarrow$ 0, Automatic $\rightarrow$ 1

### 3. Data Splitting
- Dropped the `Car_Name` column as it is not useful for numerical prediction.
- Defined `X` (features) and `y` (target: `Selling_Price`).
- Split the data into Training (80%) and Testing (20%) sets using `train_test_split`.

### 4. Model Training & Evaluation
- Implemented a **Linear Regression** algorithm using Scikit-Learn.
- Evaluated the model's performance using the **R-squared ($R^2$) score**.

---

## 📈 Results

The model showed strong predictive performance with minimal overfitting:

- **Training Data $R^2$ Score:** `0.8836` (88.36%)
- **Test Data $R^2$ Score:** `0.8466` (84.66%)

**Visualization:**
Scatter plots were generated to compare *Actual Values* vs *Predicted Values* for both the training and testing datasets. The data points closely follow the linear trend, confirming the model's high accuracy and reliability.

---

## 💻 How to Run This Project

1. Clone this repository:
   ```bash
   git clone https://github.com/ennaguiyoussef/codealpha_tasks.git
   cd car_price_prediction