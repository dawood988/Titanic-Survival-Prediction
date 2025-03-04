# Titanic Survival Prediction

This repository contains a machine learning project focused on predicting the survival of passengers on the Titanic. Using the Titanic dataset, multiple approaches are applied to preprocess the data, build models, and evaluate performance.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Model Building](#model-building)
- [Performance Evaluation](#performance-evaluation)
- [Installation & Usage](#installation--usage)
- [Contributors](#contributors)

## Project Overview

The goal of this project is to build a machine learning model that predicts whether a passenger on the Titanic survived based on various attributes such as age, gender, ticket class, and fare. The project explores different approaches to handling missing data and evaluates multiple logistic regression models.

## Dataset

The dataset contains information on Titanic passengers, including:

- **Survived** (0 = No, 1 = Yes) - Target Variable
- **Pclass** (Ticket class: 1st, 2nd, or 3rd)
- **Sex** (Male/Female)
- **Age** (Passenger’s age)
- **SibSp** (Number of siblings/spouses aboard)
- **Parch** (Number of parents/children aboard)
- **Fare** (Ticket fare)
- **Cabin** (Cabin number - Often missing)
- **Embarked** (Port of Embarkation)

## Data Preprocessing

- **Handling missing values**: Dropping or imputing missing values using various strategies (mean, median, regression, etc.).
- **Encoding categorical variables**: Converting categorical data (e.g., 'Sex') into numerical format using Label Encoding.
- **Removing unnecessary features**: Dropping irrelevant columns such as 'Name', 'Ticket', and 'Cabin'.
- **Splitting dataset**: Separating the dataset into features (**X**) and target (**y**).

## Exploratory Data Analysis (EDA)

- **Statistical summaries** of the dataset.
- **Correlation analysis** between different variables.
- **Visualization of survival distribution** based on key features such as age, sex, and class.

## Feature Engineering

- **Handling missing data** using different techniques:
  - Removing missing values.
  - Filling missing values with mean/median.
  - Using SimpleImputer.
  - Applying a regression model to predict missing values.

## Model Building

Several Logistic Regression models are trained using different approaches for handling missing data:

1. **Model 1**: Built without the 'Age' column (dropped missing values).
2. **Model 2**: Built after removing rows with missing data.
3. **Model 3**: Built after filling missing values with mean imputation.
4. **Model 4**: Built using SimpleImputer with the median strategy.
5. **Model 5**: Built after filling missing values using a regression model.

## Performance Evaluation

Models are evaluated based on:

- **Accuracy Score**
- **Confusion Matrix**
- **Visualization of Confusion Matrix using Seaborn**

## Installation & Usage

### Prerequisites

Ensure you have Python installed along with the following dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Running the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/titanic-survival-prediction.git
   cd titanic-survival-prediction
   ```
2. Run the Jupyter Notebook or Python script:
   ```bash
   jupyter notebook
   # Open the notebook and run the cells
   ```

## Contributors

- **Dawood M D** - Data Analysis, Model Implementation, Documentation

Feel free to contribute by submitting issues or pull requests! 🚢

al-Prediction
