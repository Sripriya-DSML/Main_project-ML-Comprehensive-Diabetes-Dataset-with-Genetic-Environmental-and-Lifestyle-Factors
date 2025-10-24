# Main_project-ML-Comprehensive-Diabetes-Dataset-with-Genetic-Environmental-and-Lifestyle-Factors
PROJECT TITLE

Comprehensive Diabetes Dataset with Genetic, Environmental, and Lifestyle Factors

PROBLEM STATEMENT

Diabetes mellitus includes multiple subtypes, each with distinct causes and progression patterns. Understanding how genetic, environmental, and lifestyle factors interact is essential for personalized healthcare. This project analyses a comprehensive dataset covering Steroid-Induced Diabetes, Neonatal Diabetes Mellitus (NDM), Prediabetes, Type 1 Diabetes, and Wolfram Syndrome to identify unique and shared risk factors. The challenge is to determine which factor combinations contribute to each subtype, enabling better diagnosis, targeted interventions, and effective disease management.

PROJECT OVERVIEW

This project uses a comprehensive dataset encompassing multiple diabetes subtypes, including Steroid‑Induced Diabetes, Neonatal Diabetes Mellitus (NDM), Prediabetes, Type 1 Diabetes, and Wolfram Syndrome. The dataset includes medical, genetic, environmental, and lifestyle attributes to provide a holistic view of each patient’s profile. The aim is to help researchers and healthcare professionals understand how these factors interact and contribute to the development and progression of different diabetes subtypes, enabling insights for personalized treatment, risk assessment, and improved disease management.

GOALS

1.Risk Prediction:

Predict likelihood of developing specific diabetes subtypes using genetic, environmental, lifestyle, and medical data

2.Feature Analysis & Interpretation:

Identify key factors and their interactions influencing each subtype.

3.Subtype Classification:

Build a model to distinguish among the different diabetes types using available data (e.g. classify a new patient into Type 1 vs NDM vs Steroid‑Induced, etc.).

4.Public Health Insights:

Inform preventive strategies to reduce risk, especially in genetically susceptible populations.


Domain:

Healthcare Analytics / Machine Learning for Disease Prediction

Objective:

1.Predictive Modelling: Develop a model to identify individuals at high risk of developing diabetes, supporting early intervention and personalized healthcare.

2.Classification: Classify individuals as diabetic or non-diabetic based on genetic, environmental, and lifestyle factors.

Type of problem:

Classification (predict diabetes type / diabetes status)

Target feature

Target feature 1 - Diabetes_Subtype

Target Classes / Values

Class Value Description

0: "Steroid-Induced Diabetes",

1: "Neonatal Diabetes Mellitus (NDM)",

2: "Prediabetic",

3: "Type 1 Diabetes",

4: "Wolfram Syndrome",

5: "LADA",

6: "Type 2 Diabetes",

7: "Wolcott-Rallison Syndrome",

8: "Secondary Diabetes",

9: "Type 3c Diabetes (Pancreatogenic Diabetes)",

10: "Gestational Diabetes",

11: "Cystic Fibrosis‑Related Diabetes (CFRD)",

12: "MODY"

Input feature

feature1,feature 2....feature N All the other columns (except target)

1.Genetic Markers

2.Autoantibodies

3.Family History

4.Environmental Factors

5.Insulin Levels

6.Age

7.BMI (Body Mass Index)

8.Physical Activity

9.Dietary Habits

10.Blood Pressure

11.Cholesterol Levels

12.Waist Circumference

13.Blood Glucose Levels

14.Ethnicity

15.Socioeconomic Factors

16.Smoking Status

17.Alcohol Consumption

18.Glucose Tolerance Test

19.History of PCOS (Polycystic Ovary Syndrome)

20.Previous Gestational Diabetes

21.Pregnancy History

22.Weight Gain During Pregnancy

23.Pancreatic Health

24.Pulmonary Function

25.Cystic Fibrosis Diagnosis

26.Steroid Use History

27.Genetic Testing

28.Neurological Assessments

29.Liver Function Tests

30.Digestive Enzyme Levels

31.Urine Test

32.Birth Weight

33.Early Onset Symptoms

Outcome:

Diabetes Subtype Prediction Report

Patient / Sample Input Features

Feature	Value
Risk Score	92.1
Age	45
Blood Pressure	130
Blood Glucose Levels	210
Weight Gain During Pregnancy	8.5
Cholesterol Levels	220
Waist Circumference	95
Digestive Enzyme Levels	60
Age Group	3
BMI	29.3
Pulmonary Function	88
Insulin Levels	14.2
Birth Weight	3.5
Neurological Assessments	75
Pancreatic Health	65
BMI Category	2
Genetic Marker 1	1
Family History	Yes
Air Pollution Index	75
Diet Score	6
Physical Activity	Low
Fasting Glucose	120 mg/dL
Insulin Level	10 µIU/mL
…	…
Sample Output

Predicted Diabetes Subtype Probabilities

Diabetes Subtype	Probability
Prediabetes	0.65
Type 1 Diabetes	0.15
Steroid-Induced Diabetes	0.05
Wolfram Syndrome	0.02
NDM (Neonatal Diabetes Mellitus)	0.13
Predicted Subtype: Prediabetes
Top Contributing Features

Feature	Contribution / Interpretation
Genetic Marker 1	  Presence increases genetic risk for Prediabetes.
BMI	Higher          BMI is strongly associated with Prediabetes risk.
Diet Score        	Moderate diet score contributes to increased risk.

Interpretation:

	Genetic Factors: Presence of Genetic_Marker_1 significantly increases Prediabetes risk.

	Lifestyle & Clinical Factors: High BMI and moderate diet score further elevate risk.

	Model Insight: Effectively captures complex interactions between genetic, clinical, and lifestyle variables, which may be missed by linear models.

Sample Final Decision

Chosen Model

•	Reason for Selection: High accuracy, interpretability, and strong performance in multiclass diabetes subtype prediction.

•	Final Prediction: Wolcott-Rallison Syndrome (55.95%)

•	Although Prediabetes had the highest single-class probability (0.65), the final prediction incorporates overall model confidence, clinical relevance, and ensemble decision logic to ensure a data-driven and clinically meaningful outcome.

Information about the dataset


	Shape of the dataset:70000,34


	Number of columns:34


	Number of rows:70000


	Number of duplicate rows: 0


	Checking the nulls values:0

What are the algorithms you are going to use?

	For classification tasks like diabetes prediction,algorithm

	Logistic Regression: A fundamental algorithm for binary classification.

	Decision Tree Classifier: Decision Tree Classifier: Provides clear decision-making logic.

	Random Forest Classifier: Random Forest Classifier: An ensemble method that reduces overfitting.

	Gradient Boosting Machines (GBM): Gradient Boosting Machines (GBM): Builds models sequentially to correct errors. Support Vector Machine (SVM): Effective in high-dimensional spaces.

	K-Nearest Neighbors:K-Nearest Neighbors: (Classifies based on proximity to neighbors.KNN)

	Naive Bayes: Assumes independence among features.

📈 Model Evaluation Metrics

	Accuracy: Proportion of correct predictions.

	Precision:Proportion of positive predictions that are actually correct.

	Recall (Sensitivity): Proportion of actual positives correctly identified.

	F1-Score:Harmonic mean of precision and recall.

	Area Under ROC Curve (AUC-ROC):Performance measurement for classification problems at various thresholds settings.

Perform Hyperparameter Tuning

Utilize techniques like Grid Search or Randomized Search to find the best hyperparameters:
	Grid Search: Exhaustively tests all combinations in the hyperparameter grid.

	Randomized Search: Samples a fixed number of hyperparameter combinations from the grid, offering a balance between exploration and computational efficiency.

	->This dataset going to use Randomized Search CV

Evaluate Model Performance

	After tuning, assess the model’s performance using metrics like Accuracy, Precision, Recall, F1-Score, and AUC-ROC
	
“Final Sample Input & Output Prediction — Hyperparameter Tuning with RandomizedSearchCV and Combined Classifier Models”
