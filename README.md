# Diabetes EDA and Prediction

This project performs **Exploratory Data Analysis (EDA)** and **Diabetes Prediction** using a diabetes dataset.

## Project Overview

The project has two main parts:

1. **EDA** – Explore the dataset, clean the data, and identify useful patterns.
2. **Machine Learning** – Build a simple Logistic Regression model to predict diabetes outcomes.

## Dataset

The dataset contains **768 records and 9 columns**.

Main columns:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome

`Outcome` is the target variable:

- `0` = No diabetes
- `1` = Diabetes

## EDA

The analysis includes:

- Loading and understanding the dataset
- Checking dataset shape and data types
- Statistical summary
- Checking missing values
- Detecting zero values that may represent missing measurements
- Replacing invalid zero values with missing values
- Filling missing values using the median
- Checking duplicate rows
- Data visualization and distribution analysis
- Examining relationships between variables and diabetes outcome

## Machine Learning

A **Logistic Regression** model is used for diabetes classification.

Steps:

1. Load the cleaned dataset
2. Separate features (`X`) and target (`y`)
3. Split the data into training and testing sets
4. Train the Logistic Regression model
5. Make predictions on the test data
6. Evaluate the model

The dataset is split into:

- Training data: 80%
- Testing data: 20%

The model achieved approximately **75.32% accuracy** on the test data.

Evaluation also includes:

- Accuracy
- Classification Report
- Confusion Matrix

## Prediction Function

The prediction notebook includes a simple function that allows users to enter patient information such as:

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

The model then returns a predicted result of **Diabetic** or **Not Diabetic**.

## Project Files

```text
├── analysis.ipynb
├── prediction.ipynb
├── diabetes.csv
├── diabetes_cleaned.csv
└── README.md
```

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## How to Run

1. Clone this repository.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open the notebooks in Jupyter Notebook or JupyterLab.
4. Run the EDA notebook first.
5. Run the prediction notebook using the cleaned dataset.


