# Heart Disease in Patients
Syed Zain Ali, Eric Hou, Anna Kovtunenko, Rico Osamulia

## Introduction
### Background Information
Heart disease encompasses various conditions affecting the heart, including coronary heart disease and cardiomyopathy (Centers for Disease Control and Prevention, 2023). It is a widespread health issue globally, claiming an estimated 17.9 million lives annually, with one-third of these deaths occurring prematurely in individuals under 70 years of age (World Health Organization, 2019). Factors such as high blood pressure and elevated cholesterol levels are associated with an increased risk of heart disease (Centers for Disease Control and Prevention, 2023).

Early identification of heart disease in patients is crucial. Therefore, this project aims to evaluate the effectiveness of predicting a patient's likelihood of having heart disease based on two primary factors: ST depression induced by exercise relative to rest and maximum heart rate. The central question addressed is: How accurately can the presence of heart disease be predicted in patients through the classification of these key factors?

For exploratory data analysis (EDA), we conducted forward selection to best understand the variables that would allow for the highest accuracy of predicting heart disease. The combination that had the highest accuracy was of three variables: ST depression, maximum heart rate and serum cholesterol levels. However, we wanted to be able to best visualize a correlation. As creating a visualization with three variables is difficult, we chose the combination of two variables with the highest accuracy which were ST depression and maximum heart rate. Consequently, these two variables were selected for further analysis. Classification was chosen as the algorithm for prediction, as it aims to predict the categorical class label (healthy or presence of heart disease) based on the selected variables. While exploring additional risk factors such as sex and age would have been desirable with more time and resources, the project focused on a select set of variables to maintain manageability.

The presence of heart disease appears to be correlated with low ST depression and high maximum heart rate. Classification was selected as the algorithm for prediction, aiming to predict the categorical class label (healthy or presence of heart disease) based on the selected variables.

We are combining cleveland_dataset_web, switzerland_dataset_web, virginia_dataset_web, and reprocessed_hungarian_dataset_web from the Heart Disease Database to predict if a patient from will have heart disease and have a sample size of 920. The column names for the dataset are as follows:

age - Patient's age
sex - Patient's sex
chest_pain - Chest pain type
rest_bp - Resting blood pressure
cholesterol - Serum cholesterol level (mg/dl)
fasting_blood_sugar - Fasting blood sugar > 120mg/dl (true/false)
rest_ecg - Resting electrocardiographic results
max_hr - Maximum heart rate
exercise_angina - Exercise induced angina (yes/no)
st_depression - ST Depression induced by exercise relative to rest levels
slope_st_segment - Slope of the peak exercise ST segment
num_vessels - Number of major vessels colored by flourosopy
thalassemia - Presence of thalassemia ('fixed', 'reversible', 'normal')
diagnosis - Diagnosis of heart disease ('healthy'/'sick')
