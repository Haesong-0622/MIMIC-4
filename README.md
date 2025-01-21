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

#### Study population
-------------------------------
![image](https://github.com/user-attachments/assets/14e15cdb-a70b-459a-939f-64ade572583c)
-------------------------------

#### Preprocessing
-------------------------------
![image](https://github.com/user-attachments/assets/ea7536ae-2fab-4959-8d57-8299d8d8f276)
1. Among the data, patient, medication, nursCharting, comorvbidity, and lab data are combined.
2. categorical variables after removal continuous variables only leave it
3. 0.01% of data the above missing values remove data you have
4. 0.01% of data missing values below the data I have is replace with nearby values
5. When analyzing the correlation less relevant remove Variables
-------------------------------

#### Why is it 0.01 percent?
-------------------------------
1. Statistical Reliability:
(Addressing missing values in routine health information system data: an evaluation of imputation methods using data from the Democratic Republic of the Congo during the COVID-19 pandemic)
2. Difficulty with alternative methods:
(Missing value imputation in high-dimensional phenomic data: imputable or not, and how?)
3. Data Quality Considerations:
(Addressing missing values in routine health information system data: an evaluation of imputation methods using data from the Democratic Republic of the Congo during the COVID-19 pandemic)
-------------------------------

#### result
-------------------------------
1. Linear Regression : train(0.907) , test(0.834)
2. Random Forest : train(1.0) , test(0.673)
-------------------------------

#### Discussion
-------------------------------
1. As the mimic-iv data is huge, we believe that a small number of patients is a failure factor when we reduce the number of patients.
2. I think the model performance came out poorly because the pre-processing process was simplified.
-------------------------------


