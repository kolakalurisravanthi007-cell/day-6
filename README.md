# day-6
exploratory data analysis assignment 

ASSIGNMENT DETAILS

Course: Python with Data Analysis
Topic: Exploratory Data Analysis (EDA)
Dataset: WineQT.csv
Student Name: kolakaluri sravanthi 
Assignment No: 2
Date:27 May 2026

INTRODUCTION

Exploratory Data Analysis (EDA) is the process of analyzing datasets to understand their structure, patterns, relationships, and anomalies before applying machine learning models.
EDA helps in:
->Understanding data distribution
->Finding missing values
->Detecting outliers
->Identifying relationships between variables
->Improving data quality

 OBJECTIVE
 
The objectives of this assignment are:
1.To explore WineQT dataset
2.To understand data structure and features
3.To perform data cleaning
4.To analyze data using visualizations
5.To identify relationships between variables

 DATASET INFORMATION
 
->Dataset Name: WineQT.csv
->Total Rows: 1143
->Total Columns: 13
->Type: Structured dataset
->Target Variable: Quality

 LIBRARIES USED
 
->Pandas → Data handling
->NumPy → Numerical operations
->Matplotlib → Data visualization
->Seaborn → Statistical plots
-Warnings → Ignore unnecessary alerts

 PROGRAM - DATA LOADING
 
Python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import warnings as wr

wr.filterwarnings('ignore')

df = pd.read_csv("WineQT.csv")

print(df.head())

 DATA INSPECTION
 
Used functions:
->df.shape → size of dataset
->df.info() → data types & null values
->df.describe() → statistical summary
->df.columns → column names

 DATA CLEANING
 
->Checked missing values using df.isnull().sum()
->Checked duplicates using df.duplicated().sum()
->Ensured dataset is clean before analysis

 UNIVARIATE ANALYSIS
 
Used:
->Bar plot (Quality distribution)
-.Histogram (Feature distribution)
->Swarm plot (Outliers detection)
 Observation:
->Most wines belong to medium quality range
->Some features show skewed distribution

 BIVARIATE ANALYSIS 
 
Used:
-.Pairplot
->Violin plot (Alcohol vs Quality)
->Box plot
 Observation:
->Alcohol content influences wine quality
->Higher alcohol → better quality trend

 MULTIVARIATE ANALYSIS
 
Used:
Correlation Heatmap
 Observation:
->Positive correlation: variables move together
->Negative correlation: variables move opposite
->Some features strongly impact wine quality

 KEY FINDINGS
 
->Dataset has no major missing values
->Alcohol is an important feature for quality
->Some outliers exist in data
->Correlation helps identify important features

 ADVANTAGES OF EDA
 
1.Helps understand dataset easily
2.Improves model performance
3.Detects errors and missing data
4.Provides visual insights

 CONCLUSION
 
EDA is an essential step in data analysis. It helps in understanding the dataset before applying machine learning models. WineQT dataset shows clear patterns in wine quality based on different chemical properties.
