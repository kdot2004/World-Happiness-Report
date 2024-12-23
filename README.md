# World-Happiness-Report Project
This project analyzes the factors contributing to the happiness of countries using data from the World Happiness Report. It employs machine learning techniques to uncover key insights and build predictive models.


### Introduction
The World Happiness Report ranks countries based on various socioeconomic factors. This project aims to:

- Identify features most strongly associated with happiness.
- Build predictive models to classify countries as "happy" or "unhappy."
- Provide actionable insights for policymakers to improve happiness levels globally

### Dataset Description
Source: World Happiness Report
Rows: 156 countries
Features:

- Happiness Score: Target variable (scale 0-10).
- GDP Per Capita
- Social Support
- Healthy Life Expectancy
- Freedom to Make Life Choices
- Generosity
- Perceptions of Corruption 

### Methodology
Data Preprocessing:
Dropped non-essential columns like "Country or Region."
Exploratory Data Analysis (EDA):
Correlation heatmaps.
Scatter plots for feature-target relationships.
Feature Engineering:
Created a binary column, is_happy, based on a happiness score threshold of 6.
Modeling:

- Linear and Logistic Regression.
- Decision Tree and Random Forest.
- Evaluated model performance using metrics like rmse, accuracy, precision, recall, and F1-score.

### Key Findings
Top Predictors of Happiness:

- GDP Per Capita, Social Support, and Healthy Life Expectancy are consistently significant.
- Freedom to make life choices and Perceptions of Corruption are still significant but not as much compared to the top 3 features. 
- Generosity: Weak predictor with minimal influence.
- Model Performance: Logistic Regression achieved an accuracy of 87.5%, with a precision and recall of 75%. Linear Regression achieved a RMSE of 0.64. Decision tree achieved an accuracy of 81.25%. Random Forest achieved an accuracy of 87.5%

### Limitations

- Limited to the dataset's features; external factors like culture and history are not considered.
- Possible overfitting due to the small dataset size.
- The subjectivity of happiness varies widely between individuals and cultures, making it difficult to generalize findings across all populations.
- Potential surveyor bias 
