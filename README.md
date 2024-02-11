# Home Credit: Credit Risk Model Stability
The goal of this repository is to predict which clients are more likely to default on their loans

## Description
 The absence of a credit history might mean a lot of things, including young age or a preference for cash. 
 Without traditional data, someone with little to no credit history is likely to be denied. Consumer finance providers must accurately determine which clients can repay a loan and which cannot and data is key. If data science could help better predict one’s repayment capabilities, loans might become more accessible to those who may benefit from them the most.

Currently, consumer finance providers use various statistical and machine learning methods to predict loan risk. These models are generally called scorecards. In the real world, clients' behaviors change constantly, so every scorecard must be updated regularly, which takes time. The scorecard's stability in the future is critical, as a sudden drop in performance means that loans will be issued to worse clients on average. The core of the issue is that loan providers aren't able to spot potential problems any sooner than the first due dates of those loans are observable. Given the time it takes to redevelop, validate, and implement the scorecard, stability is highly desirable. There is a trade-off between the stability of the model and its performance, and a balance must be reached before deployment.
Founded in 1997, competition host Home Credit is an international consumer finance provider focusing on responsible lending primarily to people with little or no credit history. Home Credit broadens financial inclusion for the unbanked population by creating a positive and safe borrowing experience.


## Evaluation
www.kaggle.com/competitions/home-credit-credit-risk-model-stability/overview/evaluation

## Scoring
1. Innovation (40%): Analyzes credit stability over time, specifically focusing on the competition evaluation metric beyond just feature selection. e.g. High average gini, non-decreasing performance over time, small oscillations
2. Quality (20%): Any tables, figures, and/or code samples are high quality (e.g. information-dense, easy-to-understand, and informative)
3. Clarity (20%): The overall composition is articulate, concise, accurate, and easy-to-understand.
4. Generalization (20%): The implementation of stability as a metric can be applied to non-competition datasets.


## Dataset Description
In this competition, you will be predicting default of clients based on internal and external information that are available for each client. Scoring is performed using custom metric that not only evaluates the AUC of predictions but also considers the stability of predictions model across the data range of the test set. To better understand this metric, please refer to the Evaluation tab.

### Table Description
This dataset contains a large number of tables as a result of utilizing diverse data sources and the varying levels of data aggregation used while preparing the dataset. Note: All files listed below are found in both .csv and .parquet formats.

### Base tables
Base tables store the basic information about the observation and case_id. This is a unique identification of every observation and you need to use it to join the other tables to base tables.

### Train FIles:

train_base.csv
Test Files:

test_base.csv (Note, the hidden test_base.csv contains approximately 90% of the numbers of case_id values of train_base.csv
static_0
Properties: depth=0, internal data source
Train Files:

train_static_0_0.csv
train_static_0_1.csv
Test Files:

test_static_0_0.csv
test_static_0_1.csv
test_static_0_2.csv
static_cb_0
Properties: depth=0, external data source
Train Files:

train_static_cb_0.csv
Test Files:
test_static_cb_0.csv
applprev_1
Properties: depth=1, internal data source
Train Files:

train_applprev_1_0.csv
train_applprev_1_1.csv
Test Files:

test_applprev_1_0.csv
test_applprev_1_1.csv
test_applprev_1_2.csv
other_1
Properties: depth=1, internal data source
Train Files:

train_other_1.csv
Test Files:

test_other_1.csv
tax_registry_a_1
Properties: depth=1, external data source, Tax registry provider A
Train Files:

train_tax_registry_a_1.csv
Test Files:

test_tax_registry_a_1.csv
tax_registry_b_1
Properties: depth=1, external data source, Tax registry provider B
Train Files:

train_tax_registry_b_1.csv
Test FIles:

test_tax_registry_b_1.csv
tax_registry_c_1
Properties: depth=1, external data source, Tax registry provider C
Train Files:

train_tax_registry_c_1.csv
Test Files:

test_tax_registry_c_1.csv
credit_bureau_a_1
Properties: depth=1, external data source, Credit bureau provider A
Train Files:

train_credit_bureau_a_1_0.csv
train_credit_bureau_a_1_1.csv
train_credit_bureau_a_1_2.csv
train_credit_bureau_a_1_3.csv
Test Files:

test_credit_bureau_a_1_0.csv
test_credit_bureau_a_1_1.csv
test_credit_bureau_a_1_2.csv
test_credit_bureau_a_1_3.csv
credit_bureau_b_1
Properties: depth=1, external data source, Credit bureau provider B
Train Files:

train_credit_bureau_b_1.csv
Test files:

test_credit_bureau_b_1.csv
deposit_1
Properties: depth=1, internal data source
Train Files:

train_deposit_1.csv
Test Files:

test_deposit_1.csv
person_1
Properties: depth=1, internal data source
Train Files:

train_person_1.csv
Test Files:

test_person_1.csv
debitcard_1
Properties: depth=1, internal data source
Train Files:

train_debitcard_1.csv
Test Files:

test_debitcard_1.csv
applprev_2
Properties: depth=2, internal data source
Train Files:

train_applprev_2.csv
Test Files:

test_applprev_2.csv
person_2
Properties: depth=2, internal data source
Train Files:

train_person_2.csv
Test Files:

test_person_2.csv
credit_bureau_a_2
Properties: depth=2, external data source, Credit bureau provider A
Train Files:

train_credit_bureau_a_2_0.csv
train_credit_bureau_a_2_1.csv
train_credit_bureau_a_2_2.csv
train_credit_bureau_a_2_3.csv
train_credit_bureau_a_2_4.csv
train_credit_bureau_a_2_5.csv
train_credit_bureau_a_2_6.csv
train_credit_bureau_a_2_7.csv
train_credit_bureau_a_2_8.csv
train_credit_bureau_a_2_9.csv
train_credit_bureau_a_2_10.csv
Test Files:

test_credit_bureau_a_2_0.csv
test_credit_bureau_a_2_1.csv
test_credit_bureau_a_2_2.csv
test_credit_bureau_a_2_3.csv
test_credit_bureau_a_2_4.csv
test_credit_bureau_a_2_5.csv
test_credit_bureau_a_2_6.csv
test_credit_bureau_a_2_7.csv
test_credit_bureau_a_2_8.csv
test_credit_bureau_a_2_9.csv
test_credit_bureau_a_2_10.csv
test_credit_bureau_a_2_11.csv
credit_bureau_b_2
Properties: depth=2, external data source, Credit bureau provider B
Train Files:

train_credit_bureau_b_2.csv
Test Files:

test_credit_bureau_b_2.csv
Please be aware that the same naming conventions apply to the test files. It's worth noting that some external data providers might not be available for future (test) evaluations, which is anticipated. Each group of tables can comprise one or more individual tables. If a group contains more than one table, they are divided based on WEEK_NUM. This division was implemented to restrict the maximum size of the tables.
Depth values:

depth=0 - These are static features directly tied to a specific case_id.
depth=1 - Each case_id has an associated historical record, indexed by num_group1.
depth=2 - Each case_id has an associated historical record, indexed by both num_group1 and num_group2.
You can read more about Credit bureau (CB) here https://en.wikipedia.org/wiki/Credit_bureau.

### Columns
#### Special columns:

case_id - This is the unique identifier for each credit case. You'll need this ID to join relevant tables to the base table.
date_decision - This refers to the date when a decision was made regarding the approval of the loan.
WEEK_NUM - This is the week number used for aggregation. In the test sample, WEEK_NUM continues sequentially from the last training value of WEEK_NUM.
MONTH - This column represents the month and is intended for aggregation purposes.
target - This is the target value, determined after a certain period based on whether or not the client defaulted on the specific credit case (loan).
num_group1 - This is an indexing column used for the historical records of case_id in both depth=1 and depth=2 tables.
num_group2 - This is the second indexing column for depth=2 tables' historical records of case_id. The order of num_group1 and num_group2 is important and will be clarified in feature definitions.
All other raw columns in the tables serve as predictors. Their definitions can be found in the file feature_definitions.csv. For depth=0 tables, predictors can be directly used as features. However, for tables with depth>0, you may need to employ aggregation functions that will condense the historical records associated with each case_id into a single feature. In case num_group1 or num_group2 stands for person index (this is clear with predictor definitions) the zero index has special meaning. When num_groupN=0 it is the applicant (the person who applied for a loan).

Various predictors were transformed, therefore we have the following notation for similar groups of transformations

P - Transform DPD (Days past due)
M - Masking categories
A - Transform amount
D - Transform date
T - Unspecified Transform
L - Unspecified Transform
Please note that transformations within a group are denoted by a capital letter at the end of the predictor name (e.g., maxdbddpdtollast6m_4187119P). We hope that this will simplify the manipulation with predictors.

### Edits:

pmts_month_158T is for active contract
pmts_month_706T is for closed contract
