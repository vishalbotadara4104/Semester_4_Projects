# Airline Ticket Price Analysis and Prediction

## Project Overview

This project focuses on analyzing airline ticket prices and developing predictive models using statistical analysis and machine learning techniques. The study explores how factors such as airline, travel class, route, duration, number of stops, and booking time influence ticket prices. Statistical methods and machine learning algorithms are used to understand pricing behavior and improve prediction accuracy.

## Objectives

- Perform Exploratory Data Analysis (EDA) to understand ticket price distribution, trends, and patterns.
- Analyze the impact of airline, travel class, and routes on ticket prices.
- Examine relationships between variables using correlation analysis and hypothesis testing.
- Apply Quantile Regression to study the influence of different factors on low, median, and high ticket prices.
- Develop a Gamma Regression model for predicting airline ticket prices with skewed data.
- Build and compare machine learning models to improve prediction accuracy.

## Dataset

Source: Kaggle Airline Flights Dataset

Dataset Size: More than 300,000 flight records

Target Variable: Ticket Price

Features:
- Airline
- Source City
- Destination City
- Departure Time
- Arrival Time
- Duration
- Stops
- Travel Class
- Days Left Before Departure
- Ticket Price

## Methodology

1. Data Preprocessing
   - Data cleaning
   - Missing value handling
   - Duplicate removal
   - Encoding categorical variables
   - Feature engineering
   - Outlier detection

2. Exploratory Data Analysis
   - Histogram
   - Box Plot
   - Violin Plot
   - Scatter Plot
   - Correlation Heatmap
   - Distribution Analysis

3. Statistical Analysis
   - Kolmogorov-Smirnov Test
   - Mann-Whitney U Test
   - Kruskal-Wallis Test
   - Spearman Rank Correlation

4. Statistical Models
   - Quantile Regression
   - Gamma Regression

5. Machine Learning Models
   - Decision Tree Regression
   - Random Forest Regression
   - XGBoost Regression

6. Model Evaluation
   - R² Score
   - RMSE
   - MAE
   - Residual Analysis

## Results

- Airline ticket prices are positively skewed and do not follow a normal distribution.
- Business class tickets are significantly more expensive than Economy class tickets.
- Premium airlines such as Vistara and Air India have higher average ticket prices.
- Ticket prices generally increase as the departure date approaches.
- Flight duration has a positive relationship with ticket price.
- Airline, travel class, route, and booking time significantly influence ticket pricing.
- Random Forest and XGBoost produced the best prediction performance among the implemented models.

## Key Insights

- Travel class is the most influential factor affecting ticket price.
- Airline type plays a significant role in pricing strategies.
- Early booking usually results in lower ticket prices.
- Longer flight durations are generally associated with higher fares.
- High-demand routes have higher median ticket prices.
- Most flights in the dataset have one stop.
- Airline ticket pricing depends on multiple interacting factors rather than a single variable.

## Conclusion

This project demonstrates that airline ticket pricing is influenced by several operational and market-related factors, including airline, travel class, route, duration, number of stops, and booking time. Statistical analysis confirmed significant differences in pricing across airlines, routes, and travel classes. The combination of Exploratory Data Analysis, hypothesis testing, Gamma Regression, Quantile Regression, and Machine Learning models provides a comprehensive framework for understanding and predicting airline ticket prices. The developed models can support data-driven decision-making and improve airline pricing analysis.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- XGBoost
- Jupyter Notebook

## Author

Vishal Botadara

M.Sc. Applied Statistics

Sardar Patel University
