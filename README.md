# CodeAlpha_Unemployment-Analysis-with-Python

## Project Overview
This project combines data analysis and machine learning to study unemployment trends in India. It features data preprocessing, exploratory data analysis (EDA), and the implementation of a Linear Regression model to predict unemployment rates based on socio-economic indicators. The project also visualizes model performance and feature importance for interpretability.

## Dataset Description
File Name: Unemployment in India.csv

Key Columns:

Date: Date of data collection.

Estimated Unemployment Rate (%): Target variable (unemployment rate in percentage).

Estimated Labour Participation Rate (%): Labor force participation rate in percentage.

Estimated Employed: Number of employed individuals.

Region: Geographical region of data collection.

Area: Specifies whether the data is from a rural or urban area.

## Libraries Used
Pandas: Data manipulation and analysis.

Seaborn and Matplotlib: Data visualization.

Scikit-learn: Data preprocessing and machine learning.

Joblib: Saving and loading the trained model.

## Project Workflow

1. Data Preprocessing
   
   Removed rows with missing values.
   
   Standardized region names to lowercase and removed whitespaces.
   
   Dropped the irrelevant Frequency column.
   
   Label-encoded the Area column (Rural/Urban).
   
   One-hot encoded the Region column for categorical data.

2. Exploratory Data Analysis (EDA)
   
   Visualizations and insights:

    Line Plot: Trends of unemployment rates over time.
   
    Bar Chart: Average unemployment rates by region.
   
    Boxplot: Rural vs Urban unemployment comparison.
   
    Scatterplot: Relationship between labor participation rates and unemployment rates.

3. Machine Learning
   
    a. Model Training:
 
    Features: Estimated Labour Participation Rate (%) and Estimated Employed.
    
    Target: Estimated Unemployment Rate (%).
    
    Split data into training (80%) and testing (20%) sets.
    
    Trained a Linear Regression model on the training set.

    b. Model Evaluation:
 
    Metrics:
    
    R-squared: Measures how well the model explains variability in the target.
    
    Root Mean Squared Error (RMSE): Indicates prediction error magnitude.
    
    Visualization:
    
    Actual vs Predicted Scatter Plot: Compares predicted values to actual values.
    
    Residual Plot: Highlights residual patterns to check model assumptions.

   c. Feature Importance

   Analyzed regression coefficients to determine the importance of features.

   d. Prediction on New Test Cases

   Predicted unemployment rates for new inputs (e.g., Labour Participation Rate and Employed).

   e. Time Series Comparison

   Visualized the actual vs predicted unemployment rates over time.


5. Saving Outputs
   
   Cleaned data saved to Cleaned_Unemployment_Data.csv.
   
   Trained model saved as unemployment_model.pkl for future use.

## Visualizations

Unemployment Trends: Line plot over time.

Region-Wise Averages: Bar chart of average unemployment rates.

Rural vs Urban Comparison: Boxplot analysis.

Actual vs Predicted: Scatter plot and residual analysis.

Feature Importance: Bar chart of regression coefficients.

Time Series Prediction: Line plot for actual vs predicted trends.

## How to Run

Prerequisites:

 Python (3.8 or higher)
 
 Libraries: pandas, seaborn, matplotlib, scikit-learn, joblib
 
 Steps:

   Place Unemployment in India.csv in the same directory.
   
   Run the script using any Python IDE or Jupyter Notebook.
   
   View generated plots and output files.

## Key Insights

 1.Regional and temporal patterns significantly impact unemployment trends.
 
 2.Labour participation rate is strongly correlated with unemployment rate.
 
 3.Rural and urban areas exhibit unique unemployment dynamics.
 
 4.Linear regression provides reasonable predictions with explainable feature importance.


