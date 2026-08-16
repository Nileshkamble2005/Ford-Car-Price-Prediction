# 🚗 Ford Car Price Prediction

A Machine Learning regression project that predicts the selling price of Ford cars using historical car data and features such as model, year, mileage, transmission, fuel type, tax, MPG, and engine size.

## 📌 Project Overview

The goal of this project is to build a Machine Learning model that can predict the price of a Ford car based on its characteristics.

The project follows a complete Machine Learning workflow:

**Data Loading → Data Understanding → Exploratory Data Analysis → Data Preprocessing → Feature Encoding → Feature Scaling → Train-Test Split → Model Training → Prediction → Evaluation**

## 🎯 Problem Statement

Car prices depend on several factors such as the manufacturing year, mileage, engine size, fuel type, and transmission.

This project uses historical Ford car data to train a regression model that predicts the expected selling price of a car.

## 📊 Dataset

The dataset contains:

* **17,966 records**
* **9 columns**

### Features

| Feature        | Description              |
| -------------- | ------------------------ |
| `model`        | Ford car model           |
| `year`         | Manufacturing year       |
| `price`        | Selling price of the car |
| `transmission` | Transmission type        |
| `mileage`      | Mileage of the car       |
| `fuelType`     | Fuel type                |
| `tax`          | Vehicle tax              |
| `mpg`          | Miles per gallon         |
| `engineSize`   | Engine size              |

### Target Variable

`price`

Since price is a continuous numerical variable, this is a **Supervised Machine Learning Regression** problem.

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and relationships between different features and car prices.

The analysis includes:

* Price distribution
* Statistical analysis
* Correlation analysis
* Price vs. mileage
* Price vs. year
* Feature relationships
* Categorical feature analysis

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Checked the dataset shape and information.
3. Checked for missing values.
4. Performed statistical analysis.
5. Separated input features and target variable.
6. Encoded categorical features.
7. Scaled numerical features.
8. Split the dataset into training and testing data.

### Categorical Features

The dataset contains categorical variables:

* `model`
* `transmission`
* `fuelType`

Different encoding approaches were explored.

The **One-Hot Encoding** approach performed better than Label Encoding for this project.

## 🤖 Machine Learning Model

### Linear Regression

The main Machine Learning algorithm used in this project is **Linear Regression**.

The model learns the relationship between the car features and its price.

```text
Car Features
     ↓
Data Preprocessing
     ↓
One-Hot Encoding
     ↓
Feature Scaling
     ↓
Linear Regression
     ↓
Predicted Car Price
```

## 📈 Model Performance

The One-Hot Encoding + Linear Regression approach achieved:

| Evaluation Metric |      Score |
| ----------------- | ---------: |
| R² Score          | **0.8397** |
| Adjusted R²       | **0.8387** |

The R² score of approximately **0.84** indicates that the model explains a substantial portion of the variation in car prices on the test dataset.

### Model Comparison

| Approach                             |   R² Score |
| ------------------------------------ | ---------: |
| One-Hot Encoding + Linear Regression | **0.8397** |
| Label Encoding + Linear Regression   | **0.7310** |

Based on the results, **One-Hot Encoding + Linear Regression** performed better.

## 📁 Project Structure

```text
Ford-Car-Price-Prediction/
│
├── ford_carprice_prediction.ipynb
├── ford.csv
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Nileshkamble2005/Ford-Car-Price-Prediction.git
```

### 2. Navigate to the project folder

```bash
cd Ford-Car-Price-Prediction
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

## ▶️ How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
ford_carprice_prediction.ipynb
```

Run the notebook cells sequentially to reproduce the data analysis, preprocessing, model training, predictions, and evaluation.

## 💡 Key Learning Outcomes

This project provided practical experience with:

* Data loading and data understanding
* Data cleaning
* Exploratory Data Analysis
* Data visualization
* Feature engineering
* Categorical encoding
* Feature scaling
* Train-test splitting
* Regression modeling
* Model evaluation
* Comparing preprocessing approaches

## 🚀 Future Improvements

The project can be improved by:

* Testing additional regression algorithms
* Applying hyperparameter tuning
* Using cross-validation
* Performing advanced feature engineering
* Evaluating MAE and RMSE
* Deploying the model using Streamlit or Flask
* Creating an interactive car price prediction application

## 👨‍💻 Author

**Nilesh Kamble**

B.Tech – Artificial Intelligence & Data Science

GitHub: [Nileshkamble2005](https://github.com/Nileshkamble2005)

## ⭐ Repository

If you find this project useful, consider giving the repository a ⭐.

**Project Repository:**
https://github.com/Nileshkamble2005/Ford-Car-Price-Prediction
