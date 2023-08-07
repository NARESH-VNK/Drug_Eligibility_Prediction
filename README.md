
# DRUG ELIGIBILITY PREDICTION

## Objective 

- This project aims to develop a predictive model that determines whether a patient will be eligible for the "Target Drug" in the next 30 days. 
- The model will help physicians make informed decisions on treatment options by identifying eligible patients in advance.



## Dataset Information

- The dataset provided for this project contains electronic health records of patients diagnosed with a specific disease. 
- Each row represents a healthcare record/medical event for a patient, including the timestamp, patient ID, and the type of incident (e.g., drug prescriptions, symptoms, tests). 
- The main columns in the dataset are:

```bash
1. Patient-Uid: Unique alphanumeric identifier for a patient.
2. Date: Date when the patient encountered the event
3. Incident: The type of event (e.g., drug prescriptions, symptoms).

```

The dataset is stored in Parquet format, and it includes two files:

```bash
1. Train.parquet: Dataset used for training the predictive model
2. Test.parquet: Dataset used for testing the trained model

```


## Requirements

To run this project, you need the following software and libraries:

```bash
Python
Pandas
NumPy
Scikit-learn
Matplotlib & Seaborn
```




## Process Flow

### Problem 1 - Predictive Model for "Target Drug" Eligibility
- The objective is to develop a predictive model that can predict whether a patient will be eligible for "Target Drug" in the next 30 days. Eligibility is determined when a patient takes their first prescription of "Target Drug." 

The steps to solve this problem are:

- Create a positive set comprising patients who have taken "Target Drug" and a negative set with patients who have not.
- Perform feature engineering, considering frequency-based and time-based.
- Evaluate the model on the validation set and optimize to reduce false positives and false negatives.
- Generate predictions for patients in the test dataset and which is in the form of Final_submission.csv.

## Problem 2 - Analysis of "Target Drug" Dropoff Rate

- The goal is to study dropoff for "Target Drug," which occurs when patients stop taking the treatment before the ideal treatment duration (1 year).

The steps to solve this problem are:

- Analyze the dropoff rate, defined as the number of patients dropping off each month.
- Identify events that lead to patients stopping "Target Drug" treatment.

## Problem 3 - Analysis of "Target Drug" Prescription Patterns
- The objective is to analyze the patterns in which "Target Drug" is prescribed to patients.

 The steps to solve this problem are:

- Calculate the Prescription count to extract dominant patterns in the prescription data.
- Visualize the prescription patterns over time (X-axis: month, Y-axis: number of prescriptions) using Barchart.
## Lessons Learned

- The Learning outcomes of this project help me to understand the importance of problem framing, data preprocessing, and model selection while addressing real-world challenges with healthcare data.

- It shows the Each and every data is very much important in consideration while handling in health care industry.  
-  It emphasizes clear understanding, highlighting the potential impact of data science in the medical domain.


## Output

- After training and evaluating the model, the final predictions for the test dataset has been saved in the format specified in final_submission.csv.
