
# Admission Prediction in Foreign Universities

This project aims to predict the chances of admission for students applying to foreign universities. The model takes several features such as GRE scores, TOEFL scores, university rankings, letters of recommendation, SOPs, CGPA, and research papers to predict the likelihood of admission.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Libraries Used](#libraries-used)
4. [Data Pre-Processing](#data-pre-processing)
5. [Data Visualization](#data-visualization)
6. [Model Building](#model-building)
7. [Model Evaluation](#model-evaluation)
8. [Results](#results)
9. [Conclusion](#conclusion)

## Project Overview

The primary goal of this project is to build a machine learning model that predicts whether a student has a chance of getting admitted to a foreign university based on several key academic and extracurricular features. We tested multiple machine learning algorithms, with Random Forest being the most successful in predicting admissions.

## Dataset

The dataset used in this project is sourced from Kaggle and contains data from students who applied to universities across the world. It includes the following features:

- **GRE Score**
- **TOEFL Score**
- **University Rating**
- **SOP (Statement of Purpose)**
- **LOR (Letter of Recommendation)**
- **CGPA (Cumulative Grade Point Average)**
- **Research Papers Published**

The target variable is the **Chance of Admit**, which is the probability of admission to a foreign university.

### Dataset Summary
- Total Rows: 500
- Total Columns: 9
- Columns: 8 features and 1 label column ("Chance of Admit")

## Libraries Used

The following libraries were used in this project:

- **Pandas** for data manipulation and analysis
- **NumPy** for numerical computations
- **Matplotlib** and **Seaborn** for data visualization
- **Scikit-learn** for machine learning model building and evaluation

## Data Pre-Processing

- The dataset was cleaned to handle any missing values (though there were none).
- We used the `describe()` method to gather summary statistics and ensure there were no outliers.
- Data types of features were checked and converted appropriately.
- The dataset was split into training (75%) and testing (25%) sets.

## Data Visualization

We used several data visualization techniques such as:

- **Heatmap**: To visualize the correlation matrix and identify important features.
- **Boxplots** and **Histograms**: To analyze the distribution of different features.

## Model Building

The following machine learning models were tested:

- Linear Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Lasso Regression
- Support Vector Regression (SVR)

### Random Forest Model
The Random Forest model was selected as the best performer. It is an ensemble method that combines the predictions of several decision trees to improve accuracy and reduce overfitting.

### Hyperparameter Tuning
We used GridSearchCV for hyperparameter tuning, which helped us find the best combination of parameters for each algorithm.

## Model Evaluation

We evaluated the model using **Mean Absolute Percentage Error (MAPE)**, a common metric for regression tasks. The Random Forest model achieved the highest accuracy.

## Results

The Random Forest model successfully predicted the chances of admission based on key academic and extracurricular features. The most important predictors of admission were the GRE score, TOEFL score, and CGPA.

## Conclusion

This project successfully developed a predictive model that can help students make informed decisions about their chances of getting admitted to foreign universities. By analyzing key factors, we can predict the likelihood of admission with high accuracy.

### Future Work

- Incorporate more features (e.g., extracurricular activities, recommendation quality, etc.).
- Explore additional machine learning algorithms for potential improvements.
