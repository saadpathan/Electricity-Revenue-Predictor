# Electricity-Revenue-Predictor

Necessary links for this Machine Learning project~

Dataset : https://drive.google.com/file/d/1tx1NP1a5fyfzPHHLqsCi6GNGRFdVeFtW/view?usp=drive_link

Dataset Source: https://catalog.data.gov/dataset/electric-utilities-revenue-units-sold-and-customers-by-year

Google Colab : https://colab.research.google.com/drive/1_xVQPAmAPG0M0y_8899Nsq38yl_-avH5#scrollTo=jNuJjisPX7DI

## Overview

This repository contains a Jupyter Notebook that demonstrates a comprehensive machine learning project. The project aims to to develop a machine learning model capable of accurately forecasting electricity revenues based on the provided features. This model is valuable for utility companies, energy firms, and policymakers who need to optimize electricity consumption, reduce costs, and minimize the environmental impact of energy usage. This notebook includes data preprocessing, exploratory data analysis (EDA), model training, evaluation, and deployment steps. 

## Problem Statement

The goal is to develop a machine learning model capable of accurately forecasting electricity revenues based on the provided features. This model is valuable for utility companies, energy firms, and policymakers who need to optimize electricity consumption, reduce costs, and minimize the environmental impact of energy usage.

Specifically, the model should reliably predict electricity revenues by considering various factors influencing energy consumption, such as consumer types and the number of consumers. This can help utility companies, building managers, and energy firms identify patterns and trends in energy consumption, enabling them to make informed energy decisions. Policymakers can also use this data to create regulations and incentives that promote energy efficiency and sustainability.

## Project Structure

Electricity is essential for economic and social development, enabling nations to achieve higher living standards.

In today's world, effective planning and operation of electricity production, revenue generation from production, and energy consumption are imperative. Understanding how energy generates revenue and is utilized by consumers is crucial for better management. This presents an opportunity to develop a supervised machine learning model to forecast future electricity revenues.


1. Initial Phase: We brainstormed the problem and potential approaches to solve it using machine learning concepts. Then, we designed the workflow of our project.


2. Data Mining: We extracted a dataset from Data.gov, covering data from 2015 to 2022. The dataset includes revenue, units sold, and the average number of customers, categorized by customer class for each electric utility operating in Iowa, USA.


3. Data Preprocessing: We understood the data and identified some null values in the dataset, receiving a detailed description of the characteristics involved.


4. Feature Discussion: We discussed and renamed features for better readability and understanding, facilitating a smoother data environment.


5. Exploratory Data Analysis (EDA) and Visualization: EDA and visualization provided concise knowledge of the link between features and the label (the dependent variable). The heatmap was used to understand the association between independent variables, helping to choose important features. Selecting the right elements to improve accuracy was challenging.

6. Feature Selection: We decided to use PCA for feature selection, ultimately choosing PC1 as the feature for our project.

7. Model Training and Assessment: We employed Linear Regression, Random Forest Regression, Neural Network Regression, Decision Tree, and XGBoost techniques. After comparing numerous metrics, we determined that the Random Forest Regressor produced the best results.

8. Model Explainability: We used a bar chart to compare the performance of all five models, assisting in selecting the best one. The Random Forest Regressor emerged as the best model for our dataset.

9. Conclusion: We summarized our project, from model selection and evaluation to finding the most suitable model for our dataset. We also highlighted key findings from each model with their respective values.

## Dataset Information

RY - Reporting Year

ToU - Type of Utility

U - Utility

ORoRS - Operating Revenues of Residential Sales

ORoCIS - Operating Revenues of Commercial & Industrial Sales

ORoSR - Operating Revenues of Sales for Resale

ORoAOS - Operating Revenues of All Other Sales

ASforR - Amount Sold for Residential in MWh

ASforCI - Amount Sold for Commercial & Industrial in MWh

ASforSR - Amount Sold for Sales for Resale in MWh

ASforAO - Amount Sold for All Other in MWh

ANoCR - Average No. of Customers in Residential

ANoCCI - Average No. of Customers in Commercial & Industrial

ANoCSR - Average No. of Customers in Sales for Resale

ANoCAO - Average No. of Customers in All Other

## Requirements

The project requires the following libraries:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`
- `missingno`
- `datetime`
- `scipy.stats`
- `warnings`
- `scipy.stats`
- `statsmodels.api`
- `pickle`

You can install the necessary libraries using:
```bash
pip install -r requirements.txt
```

## Usage

To run this project, clone the repository and open the `.ipynb` file in Jupyter Notebook or Jupyter Lab. On the other hand you can follow the google colab link to access this project. Follow the steps outlined in the notebook to understand the data preprocessing, modeling, and evaluation processes.

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
jupyter notebook your-notebook-file.ipynb
```

## Results





- **Best Model**: Random Forest Regression Model with Mean Squared Error (MSE): 5297160256238.563 and Root Mean Squared Error (RMSE): 2301556.051074699 and R-squared (R2): 0.9978659726302849.

- **Key Insights**: The Random Forest Regressor model is recommended for this project, as it exhibited the best performance in terms of predictive accuracy and model fit. It provided the lowest MSE and highest R-squared value among all models, indicating superior predictive capability. However, depending on specific project requirements, the XGBoost Regression model could also be considered as it demonstrated strong performance as well. The decision tree model, while showing promise, might require additional regularization techniques to mitigate overfitting. The neural network and linear regression models did not perform as well and are less suitable for this dataset.

## Contributing

Contributions are welcome! Please feel free to open issues or submit pull requests.






