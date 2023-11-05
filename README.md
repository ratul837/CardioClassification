# CardioClassification
The goal of this project was to use machine learning techniques to predict the 10-year risk of future coronary heart disease (CHD) in patientsusing data from an 
ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The dataset provided informationon over 4,000 patients and included 15 attributes, 
each representing a potential risk factor for CHD. These attributes included demographic,behavioral, and medical risk factors. To prepare the data for analysis, extensive
preprocessing was performed to clean and transform the data. This included handling missingvalues using median, mode, as well as identifying and removing outliers using the
Interquartile Range (IQR) method. Skewed continuousvariables were also transformed using log and square root transformations to reduce skewness and improve model performanceFeature.

Feature selection was performed using variance inflation factor to remove multicollinearity and a new feature called pulse pressure was createdto capture the relationship between 
systolic and diastolic blood pressure. Redundant columns were also removed to simplify the dataset. Themost important features for predicting CHD risk were identified as 'age', 'sex', 
'education', 'cigs_per_day', 'bp_meds', 'prevalent _stroke','prevalent_hyp', 'diabetes', 'total_cholesterol', 'bmi, 'heart _rate', 'glucose', and 'pulse_pressure'.

To handle the imbalanced nature of the dataset, the SMOTE combined with Tomek links undersampling technique was used to balance theclass distribution and improve model performance. The data
was also scaled using standard scalar method to ensure that all features were onthe same scale. Several machine learning models were evaluated on their performance on the primary evaluation
metric of recall. After careful analysis, theNeural Network (tuned) was chosen as the final prediction model because it had the highest recall score among the models evaluated. By selecting a 
model with a high recall score, the goal was to correctly identify as many patients with CHD risk as possible, even if it meant havingsome false positives.

Overall, this project demonstrated the potential of machine learning techniques to accurately predict CHD risk in patients using data from a cardiovascular study. By carefully preprocessing and 
transforming the data, selecting relevant features, and choosing an appropriate model based on its performance on a relevant evaluation metric, it was possible to achieve a positive business impact
by accurately predicting CHD risk in patients.
