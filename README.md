Topic: - Statistical Investigation of Chronic Kidney Disease Risk 
Factors and Prediction

Assignment: Complex Engineering Project (CEP)

Course: STA281.10 - Statistical Methods and Probability 


# CKD-Project-Tehreek-e-Muhandis


| SL | Student Name              | ID          |
|----|--------------------------|--------------|
| 1  | MD. RAYHAN KAMAL         | 2024100000250|
| 2  | SAIFUL SIDDIKY LABIB     | 2024100000469|
| 3  | ISTIAK AHAMED            | 2024100000273|
| 4  | ABDUL AHAD EMON          | 2024100000490|
| 5  | MD SHAH NAOHAJ KHAN      | 2024100000487|
| 6  | ABDUL AHAD               | 2024100000140|



Chronic Kidney Disease (CKD) Prediction and Statistical Analysis
Project Overview

Chronic Kidney Disease (CKD) is a significant global healthcare challenge that gradually reduces kidney function and may lead to kidney failure if not detected and treated early. Early diagnosis through medical indicators can improve patient outcomes and reduce healthcare costs.

This project investigates the major risk factors associated with CKD and evaluates whether CKD occurrence can be statistically predicted using healthcare data. Statistical methods and machine learning techniques are applied to analyze patient records and identify meaningful relationships between clinical variables and CKD diagnosis.

The project combines healthcare analytics, statistical reasoning, predictive modeling, and computational analysis using Python and Google Colab.

OBJECTIVES:


| OBJECTIVE NO    |   CRITERIA                                                                    |
|-----------------|-------------------------------------------------------------------------------|
|    1            | Identify significant risk factors associated with Chronic Kidney Disease.     |
|    2            | Perform exploratory data analysis using descriptive statistics.               |
|    3            | Apply probability concepts and Bayes' theorem in healthcare analytics.        |
|    4            | Analyze probability distributions of medical indicators.                      |
|    5            | Estimate population parameters using confidence intervals.                    |
|    6            | Conduct hypothesis testing to evaluate statistical significance.              |
|    7            | Examine relationships among variables through correlation analysis.           |
|    8            | Build a Logistic Regression model for CKD prediction.                         |
|    9            | Interpret findings from both statistical and medical perspectives.            |


DATASET: PROVIDED DATASETS.

DATASET VARIABLES:

| Variable                | Improved Description                                                                                                      |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Age**                 | Age of the patient in years at the time of clinical assessment.                                                           |
| **BloodPressure**       | Patient's blood pressure measurement, typically expressed in mmHg, indicating cardiovascular health status.               |
| **SpecificGravity**     | Urine specific gravity, reflecting the concentration of dissolved substances in urine and kidney concentrating ability.   |
| **Albumin**             | Urinary albumin level, indicating the presence and severity of protein leakage through the kidneys.                       |
| **Sugar**               | Urinary glucose level, indicating the presence of sugar in urine and potential abnormalities in glucose metabolism.       |
| **BloodGlucoseRandom**  | Random blood glucose concentration measured irrespective of fasting status, used to assess blood sugar control.           |
| **BloodUrea**           | Blood urea concentration, a biochemical marker used to evaluate kidney function and nitrogen waste excretion.             |
| **SerumCreatinine**     | Concentration of creatinine in the blood, commonly used to assess kidney filtration efficiency and renal function.        |
| **Sodium**              | Serum sodium concentration, an essential electrolyte involved in fluid balance, nerve function, and cellular activity.    |
| **Potassium**           | Serum potassium concentration, an important electrolyte required for proper muscle, nerve, and cardiac function.          |
| **Hemoglobin**          | Hemoglobin concentration in blood, indicating the oxygen-carrying capacity of red blood cells and anemia status.          |
| **PackedCellVolume**    | Percentage of blood volume occupied by red blood cells (hematocrit), used to evaluate anemia and hydration status.        |
| **WhiteBloodCellCount** | Total number of white blood cells in the blood, reflecting immune system activity and possible infection or inflammation. |
| **RedBloodCellCount**   | Total number of red blood cells in the blood, used to assess oxygen transport capacity and hematological health.          |
| **Hypertension**        | Presence or absence of diagnosed high blood pressure.                                                                     |
| **DiabetesMellitus**    | Presence or absence of diabetes mellitus, a chronic metabolic disorder characterized by elevated blood glucose levels.    |


# Methodology

## 1. Data Preprocessing

Before conducting the statistical analysis, the dataset is preprocessed to ensure data quality and consistency. The preprocessing steps include:

* Handling missing values using appropriate imputation techniques.
* Removing duplicate records and correcting inconsistencies.
* Encoding categorical variables into numerical formats suitable for analysis.
* Normalizing or standardizing numerical features where necessary.

---

## 2. Descriptive Statistical Analysis

Descriptive statistics are used to summarize the characteristics of the dataset and provide an overview of the patient population. The following measures are calculated:

* Mean
* Median
* Mode
* Standard Deviation
* Variance
* Range

These statistics help identify central tendencies, variability, and potential outliers in the data.

---

## 3. Probability Analysis

Probability theory is applied to evaluate the likelihood of Chronic Kidney Disease (CKD) occurrence and its association with various risk factors. The analysis includes:

* Probability of CKD occurrence
* Conditional probabilities
* Joint probabilities between medical attributes and CKD status

---

## 4. Bayes’ Theorem

Bayes’ theorem is used to estimate the probability of a patient having Chronic Kidney Disease (CKD) given the presence of specific risk factors or medical conditions.

P(CKD∣RiskFactor)={P(RiskFactor)P(RiskFactor∣CKD)×P(CKD)​}/P(RiskFactor)

Where:

* **P(CKD | RiskFactor)** = Probability of CKD given the risk factor.
* **P(RiskFactor | CKD)** = Probability of observing the risk factor among CKD patients.
* **P(CKD)** = Prior probability of CKD.
* **P(RiskFactor)** = Overall probability of the risk factor in the population.

This theorem helps assess the impact of specific medical conditions on CKD risk.

---

## 5. Probability Distribution Analysis

Probability distributions are examined to understand the patterns and variability of important clinical indicators, including:

* Age distribution
* Blood pressure distribution
* Serum creatinine distribution
* Hemoglobin distribution

Distribution analysis assists in identifying trends, skewness, and deviations from normality.

---

## 6. Confidence Interval Estimation

Confidence intervals are calculated to estimate population parameters and quantify the uncertainty associated with sample-based estimates. These intervals provide a range within which the true population values are expected to lie with a specified level of confidence.

---

## 7. Hypothesis Testing

Statistical hypothesis tests are conducted to determine whether significant relationships exist between CKD and various risk factors. The analyses include:

* Assessing the effect of hypertension on CKD occurrence.
* Assessing the effect of diabetes mellitus on CKD occurrence.
* Comparing serum creatinine levels between CKD and non-CKD patients.

Appropriate significance tests are applied, and results are interpreted using p-values and confidence levels.

---

## 8. Correlation Analysis

Correlation analysis is performed to evaluate relationships among clinical variables and identify potential predictors of CKD.

### Methods

* Pearson Correlation Coefficient
* Correlation Heatmap Visualization

### Objectives

* Identify strong predictors associated with CKD.
* Explore relationships among medical indicators.
* Detect multicollinearity among variables.

---

## 9. Logistic Regression Model

A Logistic Regression model is developed to predict the presence of Chronic Kidney Disease (CKD) based on patient clinical attributes.

### Model Equation

P(CKD) = 1 / (1 + e^(-(β₀ + β₁X₁ + β₂X₂ + ... + βₙXₙ)))

* **β₀** = Intercept term
* **β₁, β₂, ..., βₙ** = Model coefficients
* **X₁, X₂, ..., Xₙ** = Predictor variables

### Model Evaluation Metrics

The performance of the model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score

These metrics measure the effectiveness of the model in correctly identifying CKD patients and distinguishing them from non-CKD cases.


Expected Outcomes:
The project aims to:
•	Identify major medical indicators linked to CKD.
•	Quantify the relationship between risk factors and disease occurrence.
•	Evaluate the predictive power of healthcare variables.
•	Demonstrate the application of statistical methods in healthcare analytics.
•	Develop a reliable CKD prediction model.


Results Summary:
Key findings may include:
•	Serum creatinine and blood urea are strong indicators of CKD.
•	Hypertension and diabetes significantly increase CKD risk.
•	Hemoglobin levels show negative correlation with CKD occurrence.
•	Logistic regression provides effective prediction performance for CKD classification.


