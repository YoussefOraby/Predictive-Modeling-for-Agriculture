# Predictive-Modeling-for-Agriculture

This project applies machine learning to help farmers determine the best crop to grow based on soil conditions.

## Problem

Farmers cannot always measure every soil element due to cost and time constraints.  
This project identifies which soil feature is the most predictive for determining the optimal crop.

## Dataset

The dataset contains soil measurements and the recommended crop.

Features:

N  : Nitrogen content in soil  
P  : Phosphorous content in soil  
K  : Potassium content in soil  
pH : Soil acidity level  

Target:

crop : optimal crop for the soil condition

## Method

A multinomial Logistic Regression model is trained separately using each individual feature.

The performance of each feature is evaluated using the weighted F1-score.

The feature with the highest F1-score is selected as the most predictive soil metric.

## Workflow

1 Load dataset  
2 Split data into training and testing sets  
3 Train Logistic Regression using one feature at a time  
4 Evaluate predictions using F1-score  
5 Identify the most predictive feature

## Libraries

pandas  
scikit-learn
