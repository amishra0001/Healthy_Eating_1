# Healthy_Eating_1
Healthy Eating Meal Data Analysis
Project Overview
*******************************************************************************************************************************************************
This project provides a comprehensive statistical analysis of a healthy eating meal dataset (Healthy_Eating.csv) to identify the key nutritional drivers of customer satisfaction (Rating) and establish data-driven strategies for menu optimization.

The analysis moves beyond simple averages, using Multiple Linear Regression and ANOVA to translate raw nutritional data into actionable, high-impact business recommendations.

Key Strategic Conclusions

The statistical modeling yielded two high-impact findings that guide future recipe development:

Protein-First Strategy is Paramount: Protein and Fiber are confirmed as the strongest positive and statistically significant predictors of a higher customer rating. Focus on increasing these two macro-nutrients to directly maximize user satisfaction.

Cuisine-Specific Calorie Benchmarking: The analysis showed that calorie content differs significantly across cuisine types (e.g., Indian vs. Mexican). This mandates abandoning a single centralized calorie average and establishing cuisine-specific targets for competitive meal design.

Methodology and Analysis Pipeline

The project follows a rigorous three-stage process, fully encapsulated in the complete_healthy_eating_analysis.py script:
1. Data Cleansing and Preparation
Missing Data Imputation: Handled missing values in all numerical columns by imputing the median value.

Outlier Removal: Outliers in key variables (calories, protein_g, fat_g) were removed using the Interquartile Range (IQR) method to ensure robust statistical modeling.

Data Standardization: Categorical data (cuisine, diet_type) was cleaned and standardized.

2. Statistical Analysis
Multiple Linear Regression: Used to quantify the impact (coefficient) and significance (P-value) of different nutrients (protein_g, fat_g, sugar_g, fiber_g) on the final Rating.

ANOVA (Analysis of Variance): Used to test the hypothesis that the mean calorie content is different across the major cuisine types.

3. Data Visualization
Three primary visualizations were generated to summarize the findings:

Distribution of overall Meal Ratings.

Comparison of average nutritional content (Calories, Protein, Fat) by Diet Type.

Box plot showing the distribution of Calories across major Cuisine Types (visual support for the ANOVA test).

Project Structure and Files

File Name

Type

Description

Healthy_Eating.csv

Data

The raw dataset containing meal information, nutritional values, and customer ratings.

complete_healthy_eating_analysis.py

Python Script

The core script for the entire project. It handles data loading, cleansing, execution of all statistical models, plotting of all visualizations, and prints the final strategic conclusion.

project_summary.md

Report

A detailed summary document outlining the project's objectives, methodology, and key strategic findings.

README.md

Documentation

This file.

How to Run the Analysis
Requirements: This analysis requires Python 3.x and the following libraries:

a.pandas
b.numpy
c.matplotlib
4.seaborn
5.scipy
6.statsmodels

Execution: Ensured the Healthy_Eating.csv file is in the same directory as the Python script.
I run the main analysis script from my terminal:
python complete_healthy_eating_analysis.py
Output: The script will output the following to the console:

Data cleansing logs and descriptive statistics.
ANOVA and Regression results (R-squared, coefficients, P-values).

The final strategic conclusion.
Three pop-up windows displaying the generated data visualizations.
