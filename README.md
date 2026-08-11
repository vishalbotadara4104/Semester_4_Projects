# Airline Ticket Price Analysis and Prediction

## Project Overview

This project focuses on analyzing airline ticket prices and identifying the major factors that influence pricing. The study combines Exploratory Data Analysis, statistical analysis, regression techniques, and machine learning models to understand pricing patterns and predict airline ticket prices.

The project uses airline flight data containing information about airlines, routes, travel class, duration, stops, departure time, arrival time, days left before departure, and ticket price.

## Objectives

- Analyze the distribution, trends, and patterns in airline ticket prices.
- Study the impact of airline, travel class, routes, duration, stops, and booking time on ticket prices.
- Examine relationships and differences between important variables using statistical analysis.
- Apply Quantile Regression to study factors affecting low, median, and high ticket prices.
- Develop a Gamma Regression model for skewed airline ticket price data.
- Build and compare machine learning models to improve ticket price prediction.

## Dataset

Source: Kaggle Airline Flights Dataset

Dataset Size: More than 300,000 flight records

Target Variable: Price

Main Features:

- Airline
- Flight
- Source City
- Departure Time
- Stops
- Arrival Time
- Destination City
- Class
- Duration
- Days Left
- Price

## Methodology

### 1. Data Preprocessing

- Loaded and inspected the dataset
- Checked data types and missing values
- Removed duplicate records
- Handled missing values
- Converted variables into suitable formats
- Encoded categorical variables
- Converted duration into numerical format
- Created relevant features
- Applied scaling and transformation where required

### 2. Exploratory Data Analysis

- Descriptive statistics
- Distribution analysis
- Histogram
- Boxplot
- Bar plots
- Scatter plots
- Correlation analysis
- Correlation heatmap
- Outlier detection
- Feature relationship analysis

### 3. Statistical Analysis

- Kolmogorov-Smirnov Test
- Mann-Whitney U Test
- Kruskal-Wallis Test
- Spearman Rank Correlation

These methods were used to understand the distribution of ticket prices, compare pricing across groups, and identify relationships between important variables. The dataset was found to be non-normal, supporting the use of non-parametric methods. :contentReference[oaicite:1]{index=1}

### 4. Statistical Modelling

Quantile Regression was used to study the effects of different variables across the 25th, 50th, and 75th price quantiles.

Gamma Regression was applied because airline ticket prices are positive, right-skewed, and show increasing variance with the mean.

### 5. Machine Learning Models

- Linear Regression
- Ridge Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

The models were evaluated using R2 Score, MAE, RMSE, and MAPE.

## Model Results

| Model | R2 Score | MAE | RMSE | MAPE |
|---|---:|---:|---:|---:|
| Linear Regression | 0.9118 | 4,550 | 6,741 | 46.23% |
| Ridge Regression | 0.9118 | 4,550 | 6,741 | 46.23% |
| Decision Tree | 0.9603 | 2,516 | 4,521 | 17.06% |
| Gradient Boosting | 0.9627 | 2,560 | 4,380 | 18.12% |
| Random Forest | 0.9765 | 1,783 | 3,476 | 12.32% |

Random Forest achieved the best overall performance with an R2 score of 0.9765, MAE of 1,783, RMSE of 3,476, and MAPE of 12.32%. It was selected as the final model for ticket price prediction. :contentReference[oaicite:2]{index=2}

## Statistical Model Results

### Quantile Regression

The Quantile Regression model achieved a median Pseudo R2 of approximately 0.7373. The training and testing MAE were approximately ₹4,242 and ₹4,221 respectively, showing similar performance across both datasets. The model also maintained the expected order of the predicted quantiles without quantile crossing. :contentReference[oaicite:3]{index=3}

### Gamma Regression

The Gamma Regression model achieved:

- Pseudo R2: 0.9041
- MAE: ₹4,691
- RMSE: ₹7,882

The model was suitable for the right-skewed and positive ticket price data. :contentReference[oaicite:4]{index=4}

## Key Insights

- Airline ticket prices are right-skewed and contain outliers.
- Travel class has a major influence on ticket prices.
- Airline, route, duration, stops, and days left before departure are important pricing factors.
- Ticket prices generally increase as the departure date approaches.
- Longer flights tend to have higher prices.
- Pricing behaviour differs across low, median, and high price segments.
- Nonlinear tree-based models performed better than linear models.
- Random Forest provided the best prediction performance among the tested machine learning models. :contentReference[oaicite:5]{index=5}

## Conclusion

The project demonstrates how statistical analysis and machine learning can be combined to understand and predict airline ticket prices. Exploratory analysis helped identify important pricing patterns, while statistical models provided deeper insights into different price segments.

Among the machine learning models, Random Forest achieved the best performance and was selected as the final prediction model. The results show that airline ticket pricing involves complex and nonlinear relationships that can be effectively captured using ensemble machine learning methods. :contentReference[oaicite:6]{index=6}

## Future Improvements

- Include seasonal trends and holiday information.
- Add fuel prices, weather, and competition-related factors.
- Use larger and more diverse datasets.
- Apply hyperparameter tuning and cross-validation.
- Update the model regularly with recent ticket pricing data.
- Deploy the prediction model through a web or mobile application. :contentReference[oaicite:7]{index=7}

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

## Project Files

- ML_Models.ipynb
- Project_Work_Quantile Regression Model.ipynb
- Gamma_model.ipynb
- airlines_flights_data.csv
- Project Report

## Author

Vishal Botadara

M.Sc. Applied Statistics

Sardar Patel University
