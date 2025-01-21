#### Introduction to the Study
-------------------------------
Using various biological datasets, we intend to develop an algorithm (model) that can predict potadium concentrations after 6 hours.
-------------------------------

#### the purpose of the study
-------------------------------
It is to improve patient safety by accurately predicting potassium levels after 6 hours, 
and to improve treatment outcomes in the clinical field by providing timely treatment. 
This is to develop a tool to help medical staff become aware of and respond appropriately to risks from potassium imbalances.
-------------------------------

#### Reason for Research Selection
-------------------------------
Potassium is an important electrolyte that plays an essential role in maintaining nerve and muscle function and heart rhythm.

Recent studies have pointed out that an imbalance in potassium concentration can cause serious cardiovascular problems, which is a common risk factor in patients with chronic diseases such as acute renal failure, diabetes, and heart failure.

Given such risks, early detection of changes in potassium concentration and proper management are critical to increasing patient survival rates, so we have developed algorithms to predict potassium concentration.
-------------------------------

#### INPUT
-------------------------------
MIMIC-iv (ver 3.0)
Total number of patients, number of visits: 47073 patients, 80215 visits (based on MIMIC-iv)
-------------------------------

#### OUTPUT
-------------------------------
Using mimic-iv data, predict the concentration of potassium in the patient's blood after 6 hours
-------------------------------

#### Model Learning
-------------------------------
Algorithms : Linear Regression, Random Forest
Train and Test Split : 7:3
-------------------------------

#### Model Verification
-------------------------------
Evaluation indicators : AUC, Classification Matrix, RMSE
-------------------------------
