# Data Introduction:
The dataset of interest is based on medical and demographic data from patients, along with their diabetes status (positive or negative). The data includes features such as age, gender, body mass index (BMI), hypertension, heart disease, smoking history, HbA1c level, and blood glucose level.

# Programming Languages/plugins used:
Python, scipy, pandas, seaborn, statsmodels.formula.api, numpy, confusion_matrix, and roc_curve. 

# Motivation:
Motivations for our research are primarily for the following:
- Explore the relationship between variables like age, gender, body mass index (BMI), hypertension, heart disease, smoking history, blood glucose level on HbA1c level, and whether a patient would have diabetes or not.
- Predict whether a patient has diabetes status based on patient characteristics.
By navigating different patient characteristics, health officials can identify individuals who are more at risk of developing diabetes status and prevent issues from worsening.

# Research Questions:
- Is there a relationship between the smoking history of an individual and their HbA1c level after controlling their age, and whether that person has heart disease and hypertension?
- Is there a linear relationship between the log-odds of getting diabetes and bmi, hemoglobin levels, and blood glucose levels in the data?
The first question can be used to identify how smoking history and HbA1c level interact with each other after controlling age, and whether that person has heart disease and hypertension. The second question can be helpful to know what the relationship between getting diabetes and bmi, hemoglobin levels, and blood glucose levels are. The information gained from asking these questions can help identify individuals at risk of diabetes.

# Summarization:
Based on the linear regression model we fit, we're 95% confident that the population slope for how the person who currently smokes affects the chances of that person having diabetes is contained in the interval (0.005, 0.060). Alongside that, based on the logistic model with a relatively high AUC and pseudo R^2 value, we have evidence to suggest that the explanatory variables used (hemoglobin levels, bmi, and blood glucose levels) provide a good model to assess the likelihood of an individual developing diabetes. Using a low predictive probability threshold reduces the chance of an individual getting a false negative. Minimizing a low false negative rate is important to ensure the safety of individuals and make sure that they get treatment if necessary.

# Limitations:
There are several limitations to our analysis, results, and interpretations. Firstly, our dataset is limited in the different patient characteristics that may influence the likelihood of an individual having diabetes. Therefore, we cannot confidently state that the characteristics chosen for this research are the sole predictors in identifying diabetes. Furthermore, in this research, we only identify whether a patient has or does not have diabetes. There is no indication of what type of diabetes a patient has, which may be influenced by other factors. For those looking for treatment and prevention described in the introduction, different measures may be taken depending on the type of diabetes.

# Future Work:
For future analyses, it may be beneficial to explore the other variables that were not tested in this specific. For instance, patient sex was not used in our analyses but can offer the potential to be an important factor.
