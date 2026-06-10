# OIBSIP_Data-Science_taskno.3
# Car Price Prediction Using Machine Learning

## 🚗 Project Overview

This project was completed as part of the **Oasis Infobyte Data Science Internship (Task 3)**.

The objective of this project is to build a Machine Learning model capable of predicting the selling price of a used car based on various factors such as present price, fuel type, transmission type, ownership, kilometers driven, and car age.

The project demonstrates the complete Machine Learning workflow including data preprocessing, feature engineering, model training, evaluation, and prediction.

---

## 📊 Dataset Information

Dataset: **Car Price Prediction Dataset**

The dataset contains information about used cars and their selling prices.

### Features

| Feature       | Description                            |
| ------------- | -------------------------------------- |
| Car_Name      | Name of the Car                        |
| Year          | Manufacturing Year                     |
| Selling_Price | Selling Price of Car (Target Variable) |
| Present_Price | Current Market Price                   |
| Driven_kms    | Total Kilometers Driven                |
| Fuel_Type     | Petrol / Diesel / CNG                  |
| Selling_type  | Dealer / Individual                    |
| Transmission  | Manual / Automatic                     |
| Owner         | Number of Previous Owners              |

---

## 🎯 Project Objectives

* Analyze car-related data.
* Perform feature engineering.
* Convert categorical variables into numerical values.
* Train a Machine Learning regression model.
* Predict car selling prices.
* Evaluate model performance using regression metrics.

---

## 🛠 Technologies Used

* Python
* Pandas
* Scikit-Learn
* Jupyter Notebook
* Machine Learning

---

## 🤖 Machine Learning Algorithm

### Random Forest Regressor

Random Forest Regressor is an ensemble learning algorithm that combines multiple decision trees and averages their predictions to improve accuracy and reduce overfitting.

### Why Random Forest?

✅ High Prediction Accuracy

✅ Handles Non-Linear Relationships

✅ Less Overfitting Compared to Single Decision Trees

✅ Works Well on Small and Medium Datasets

---

## 📂 Project Workflow

### Step 1: Import Required Libraries

Libraries used:

* Pandas
* train_test_split
* RandomForestRegressor
* r2_score
* mean_absolute_error

---

### Step 2: Load Dataset

The dataset is loaded into a Pandas DataFrame for analysis and preprocessing.

---

### Step 3: Feature Engineering

A new feature called **Car_Age** is created:

Car_Age = Current Year - Manufacturing Year

This helps the model understand how old the car is.

---

### Step 4: Data Preprocessing

#### Remove Unnecessary Columns

Columns removed:

* Car_Name
* Year

#### Convert Categorical Variables

Text columns such as:

* Fuel Type
* Selling Type
* Transmission

are converted into numerical format using One-Hot Encoding.

---

### Step 5: Define Features and Target

#### Features (X)

* Present Price
* Driven KMs
* Fuel Type
* Selling Type
* Transmission
* Owner
* Car Age

#### Target (y)

* Selling Price

---

### Step 6: Split Dataset

Dataset is divided into:

* Training Data: 80%
* Testing Data: 20%

Random State:

42

---

### Step 7: Train Machine Learning Model

A Random Forest Regressor model is trained using the training dataset.

```python
model.fit(X_train, y_train)
```

---

### Step 8: Make Predictions

The trained model predicts selling prices for unseen cars.

```python
y_pred = model.predict(X_test)
```

---

### Step 9: Evaluate Model Performance

Two evaluation metrics are used:

#### R² Score

Measures prediction quality.

Range:

* 1.0 = Perfect Prediction
* 0.0 = Poor Prediction

#### Mean Absolute Error (MAE)

Measures average prediction error.

Lower MAE indicates better performance.

---

## 📈 Model Performance

Typical Results:

```text
R² Score: 0.95+

Mean Absolute Error: 0.4 - 0.6
```

These results indicate excellent prediction accuracy.

---

## 🚘 Sample Prediction

The model can predict the selling price of a car using its features.

Example Output:

```text
Predicted Selling Price: 3.42 Lakhs
```

---

## 📊 Learning Outcomes

Through this project, I gained practical experience in:

✅ Data Cleaning

✅ Feature Engineering

✅ One-Hot Encoding

✅ Regression Analysis

✅ Random Forest Algorithm

✅ Model Evaluation

✅ Predictive Analytics

✅ Machine Learning Workflow

---

## 🚀 How to Run the Project

### Install Required Libraries

```bash
pip install pandas scikit-learn
```

### Run the Script

```bash
python car_price_prediction.py
```

or open the notebook in Jupyter Notebook and run all cells.

---

## 📩 Internship Details

Internship Provider: Oasis Infobyte

Domain: Data Science

Task: Task 3 – Car Price Prediction Using Machine Learning

---

## 👨‍💻 Author

Nilay Patel

Data Science Intern – Oasis Infobyte

GitHub:
https://github.com/Nilay-Patel-5

---

## ✅ Conclusion

This project successfully predicts used car selling prices using the Random Forest Regression algorithm. Through data preprocessing, feature engineering, and model evaluation, the project demonstrates how Machine Learning can be applied to solve real-world business problems involving price prediction and decision-making.
