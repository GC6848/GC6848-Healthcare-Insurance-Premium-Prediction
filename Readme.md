# Project: Healthcare Insurance Premium Prediction

## Executive Summary
This study seeks to develop a model capable of predicting health insurance premium. Through the study, I have created a regression model with RMSE testing at $4,350 and adjusted r squared testing at 87%.


## Background

Health insurance is a contract, represented by a policy, designed to help offset the costs of medical treatment by covering a portion of the professional and hospital fees incurred on the policyholders, who are most likely to be insureds. According to the U.S government’s health insurance exchange website HealthCare.gov, health insurance coverage comes in several forms aimed at meeting the varying needs of policyholders. These are:
- Exclusive Provider Organization (EPO): services in this plan are covered only if the doctors, specialists, or hospitals are in the plan’s network – except in cases of emergency.
- Health Maintenance Organization (HMO): coverage in this plan is limited to care from doctors who work for or are contracted with the HMO. Generally, policies do not cover out-of-network care except in an emergency. Likewise, plans may require that a policyholder to live or work in its service area to be eligible for coverage. Typically, HMOs provide integrated care and focus on prevention and wellness.
- Point of Service (POS): payment in this plan is lesser if policyholders access doctors, hospitals, and other healthcare providers belonging to the plan’s network. Nonetheless, insured is required to get a referral from their primary care doctor for them to see a specialist.
- Preferred Provider Organization (PPO): payment in this plan is lesser for healthcare if policyholders choose to get treatment from providers in the plan’s network. However, policyholders can pay additional cost to access doctors, hospitals, and providers outside of the network without a referral 

Under the healthcare law, insurance companies can only account for five factors when determining premiums. These are:
- Age: health insurance premiums are higher for older people than for younger ones.
- Location: health insurance rates may vary due to competition, state, local regulations, and cost of living.
- Tobacco use: tobacco users pay higher health insurance premium compared to those who do not smoke.
- Individual vs. family enrollment: plan that also covers a spouse and dependents are more costly than plan that does not cover spouse and dependents.
- Plan category: plan categories Bronze, Silver, Gold, and Platinum have an effect on premium prices.

According to the latest marketplace benchmark premiums from the Kaiser Family Foundation, health insurance premiums across the US cost an average of $438 monthly per person and this can be a steep price to pay for some American families ([source](https://www.insurancebusinessmag.com/us/news/healthcare/a-guide-to-finding-the-best-affordable-health-insurance-plan-422601.aspx#:~:text=Health%20insurance%20premiums%20across%20the,pay%20for%20some%20American%20families.)).


## Problem Statement

Health insurance premium is expensive in the United States. Many Americans are concerned about health insurance costs. Almost 40 percent of Americans would discard their health insurance altogether and chose to go uninsured instead of paying high premiums if the health insurance premium exceeded what they considered reasonable ([source](https://healthpayerintelligence.com/news/health-insurance-is-expensive-but-americans-intend-to-keep-their-plans-in-2023)). Hence, in this project, I am tasked to develop a model to help Americans to predict health insurance premium.

The model is expected to predict if health insurance premium, accurately. Metric used to assess model's prediction is RMSE. This metric will be compared against a baseline model prediction of health insurance premium at $12,114. Model is expected to achieve at least 70% in adjusted r squared testing score.


## Datasets

The datasets used for this analysis are obtained from [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance):

| Dataset | Description |
|---|---|
| insurance_claims.csv | Contains data relating to age of primary beneficiary, insurance contractor gender, body mass index (ideally 18.5 to 24.9), number of children covered by health insurance / number of dependents covered by health insurance, smoking status, beneficiary's residential area in the US, northeast, southeast, southwest, northwest; and individual medical costs billed by health insurance. |


#### Overview of technical analysis: 

(1) Problem_Statement <br>
(2) Understanding Data <br>
(3) Preprocessing <br>
(4) Modelling <br>
(5) Conclusion <br>
(6) Recommendations


### Conclusion
Random Forest Regressor is chosen as the final model as Random Forest Regressor <br>
(1) is not overfitting;   
(2) has highest adjusted r squared testing at 87%; and
(3) has lowest RMSE testing at \$4,350 and third lowest RMSE training at \\$3,740, that is lower than that of baseline model.


### Recommendations
These are the limitations observed: <br>
(1) dataset is small with 7 columns and 1,338 rows; <br>
(2) results generalizability limited to United States; <br>
(3) no information on the source of data, whether it is from one insurance company, a few companies or more; and <br>
(4) Random Forest Regressor model is prone to overfitting because it can keep branching until it memorizes the training data.

For future improvement, it is recommended to <br>
(1) continuous training and improving model with more data. 
