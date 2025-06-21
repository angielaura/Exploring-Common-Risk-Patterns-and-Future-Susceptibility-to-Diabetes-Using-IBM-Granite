# Exploring-Common-Risk-Patterns-and-Future-Susceptibility-to-Diabetes-Using-IBM-Granite
A capstone project made for IBM Data Classification and Summarization using IBM Granite

## Project Overview
This project aims to analyze the common risk patterns associated with diabetes and identify individuals who may bet at high risk of developing the disease in the future. The objectives are :
- To uncover consistent characteristics and trends found in past diabetic patients.
- To detect non-diabetic individuals who exhibit early indicators or risk factors of future diabetes.
- To determine which variables have the most significant impact on the likelihood of someone developing diabetes.

## Raw Dataset Link
The dataset was obtained from Kaggle and is uploaded by Mohamed Mustafa with the title of Diabetes Prediction Dataset.
Below is the link :
https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

## Insights and Findings
I have found the main characteristics of diabetic patients, below is the summaries :
- Age is over 80 years old.
- High BMI (>30).
- Blood glucose level is above 250mg/dL.
- Presence of hypertension and heart disease.
- Higher risk as a smoker.
  
While the general trends of the individuals who is at risk of developing diabetes in the future are down below :
- Age is over 40 years old.
- High BMI value (>27).
- Elevated HbA1c levels (>5.7)
- Particularly has the glucose level of 140mg/dL.
- Has a history of smoking
- The presence of hypertension in older individuals (>60 years old)

And finally, individuals whom developed diabetes tend to scored higher in some features, namely Age, BMI, HbA1c Levels, and Blood Glucose.

Conclusion :
These findings underscore the multifactorial nature of type 2 diabetes, with obesity, age, and comorbid conditions such as hypertension and heart disease playing crucial roles. Several shared patterns also point toward higher future risks, notably advanced age, elevated BMI, pre-diabetic biomarkers (such as high HbA1c and glucose levels), and the occasional presence of hypertension or a history of smoking. Individuals would benefit from lifestyle interventions focusing on healthy weight management, regular physical activity, and glucose monitoring to mitigate their diabetes risk. Further research or larger sample sizes would be beneficial to solidify these observations and explore potential causal relationships.

## AI Support Explanation
In this project, I utilized the IBM Granite model (granite-3.3-8b-instruct) to assist in analyzing tabular health data and identifying patterns related to diabetes risk. Although the create_pandas_dataframe_agent from Langchain could not be fully utilized due to runtime and memory constraints, I successfully employed llm.invoke() to prompt Granite for summarizing risk characteristics and high-risk profiles based on descriptive patient data. The model helped extract key insights, such as common traits among diabetic and at-risk individuals, which guided the manual visualization and comparison of features. While IBM Granite could not directly generate charts or manipulate dataframes, it played a significant role in guiding the analytical direction and interpretation of results.
