# Diwali Sales Analysis
## Project Overview

This project performs Exploratory Data Analysis (EDA) on a Diwali Sales Dataset to understand customer purchasing behavior during the Diwali festival season.

The analysis helps businesses identify customer demographics, product categories, and purchasing trends so they can improve marketing strategies and increase sales.

## Objectives
The main objectives of this project are: 

 • Analyze customer purchasing behavior during Diwali
 
 • Identify which age group, gender, and state contribute most to sales
 
 • Determine the top selling product categories
 
 • Understand the relationship between occupation and spending
 
 • Generate insights useful for business decision making

## Dataset Description
The dataset contains customer transaction information such as:

• User_ID

• Customer Name

• Gender

• Age Group

• State

• Marital Status

• Occupation

• Product Category

• Product ID

• Orders

• Amount (Purchase Value)

## Technologies Used
This project uses the following tools and libraries:

• Python

• Pandas

• NumPy

• Matplotlib

• Seaborn

• Jupyter Notebook

# Project Workflow
## 1. Data Import
Load the dataset and required libraries.

  import pandas as pd
  
  import numpy as np
  
  import matplotlib.pyplot as plt
  
  import seaborn as sns
  
  df = pd.read_csv("Diwali Sales Data.csv", encoding='unicode_escape')
  
## 2. Data Cleaning
Data preprocessing steps performed:

• Removing null values

• Dropping unnecessary columns

• Converting data types

• Handling missing values
  
  df.drop(['Status','unnamed1'], axis=1, inplace=True)
  df.dropna(inplace=True)
  
## 3. Exploratory Data Analysis (EDA)
EDA was performed to understand patterns such as:

• Gender-wise purchasing behavior

• Age group vs spending

• State-wise sales distribution

• Product category analysis

• Occupation vs purchase amount

Example visualization:
  sns.countplot(x='Gender', data=df)

  
## Key Insights
Some important findings from the analysis:

• Married women aged 26–35 years are the highest buyers.

• Customers from Uttar Pradesh, Maharashtra, and Karnataka contribute the most to sales.

• IT, Healthcare, and Aviation professionals spend more during Diwali.

• Food, Clothing, and Electronics are the top selling product categories.

# Project Structure
Diwali-Sales-Analysis
│

├── Diwali_Sales_Analysis.ipynb

├── Diwali Sales Data.csv

├── README.md


# How to Run This Project
1. Clone the Repository

git clone https://github.com/RitikDevrani/Python_Diwali_Sales_Analysis.git

3. Navigate to the Project Folder

cd Diwali-Sales-Analysis

4. Install Required Libraries

pip install pandas numpy matplotlib seaborn

6. Run Jupyter Notebook

 jupyter notebook

Open Diwali_Sales_Analysis.ipynb and run the cells.

# Future Improvements
Possible future enhancements:

• Build Machine Learning models to predict customer purchase behavior

• Create a Power BI dashboard for interactive visualization

• Deploy a web dashboard using Streamlit


# Author
Ritik Devrani

Diploma in Computer Science

BCA (IGNOU)
