# Chris's Portfolio

## Project 1
## Predictive Hotel Review Analysis Alteryx Data Competitetion Overview 
- Collaborated in developing a predictive model using Excel and Python's scikit-learn to forecast Las Vegas hotel review scores for amenity optimization.
- Developed Tableau visualizations to illustrate amenity trends among top- and bottom-rated hotels, reinforcing model insights.
- Employed Excel and Python to scrape over 1,000 hotel reviews, ensuring a robust dataset for analysis.
- Competed in an Alteryx-hosted challenge with over 70 participants, demonstrating advanced analytical skills.
- Applied regression analysis techniques to accurately predict dependent variable outcomes based on independent variables.
  
  ## Code and Resources
- Conducted regression analysis using Python to derive actionable insights.
- Utilized Excel for data cleaning to support efficient Alteryx workflows.
- Developed and maintained interactive Tableau dashboards for comprehensive data visualization.
![image](https://github.com/user-attachments/assets/06eedf4d-1400-4664-95a7-adb6f8122fb1)
## The Equation for Pyhton
![image](https://github.com/user-attachments/assets/4705a82a-1737-4bf7-a496-79eaf305f119)
![image](https://github.com/user-attachments/assets/0b54b751-55f8-4719-81b7-4fdc0f442bc5)

## Our Analysis 
Utilized Alteryx to develop workflows that provided data-driven insights into team performance, enabling role-based analysis to measure effectiveness and optimize operations.
![image](https://github.com/user-attachments/assets/785c4063-ca65-406d-9a9c-9c1b159bcf25)
Based On Linear Regression we did on python we discovery what amenties should hotels priotzie in order to ensure the highest review.
![image](https://github.com/user-attachments/assets/bd00ec4f-814a-4e24-afcb-46907919cbbf)
While we were data cleaning we narrow down to Hotel name, # amenities, Average score, Spa, Casino, Free Interent, and top 3 Amenities.
After Analysis we noticed with the top 5 hotels that were doing well was having around 5 amentites compare to the other amounts of amentites they had.
![image](https://github.com/user-attachments/assets/92192a28-eed8-4bd9-906c-c7887fbddb8d)

We also saw that hotels with higher reviews and scores had specfic amenties such as Casino, Free Internet, Spa. Others that had these and extras places were a plus such as Tennis Court and Pool.

##  Hotels should prioritize these amenities (in order):
- Free Internet
- Casino
- Spa
- Pool
- Tennis Court
- Gym (negative effect)




### What was our Objective: How can hotels predict a Tripadvisor review, and what amenities should hotels prioritize in order to ensure the highest review?
### Answer: Hotels offering five key amenities—prioritizing free internet, a spa, and a casino—tended to receive higher reviews on TripAdvisor. To predict higher review counts and ratings, these specific amenities were identified as essential, with hotels like Wynn, The Venetian, and Encore scoring the highest.
![image](https://github.com/user-attachments/assets/29297c93-5330-4677-b857-7cd99f085a67)







## Project 2 
### Alzheimer’s Diagnosis Predictive Modeling Overview 
- Led a team in utilizing Excel for data analysis and predictive modeling, applying Multiple Linear Regression (MLR) and Regression Trees to identify key factors for early Alzheimer’s diagnosis. 
- Developed Regression Trees using XLMiner to visually highlight critical variables for early detection.
- Identifying which variables are the most significant when diagnosing a patient with alzheimer's.

DataSet:
- [Alzheimer’s Disease Data from Kaggle](https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset)
- 33 Variables and 2150 Records
- Decision variable: Diagnosis
- Classification

## Preprocessing Data
### Step 1:
Check missing values pattern by heatmap and delete columns rows if needed. There were no missing values in our data set. We did delete one column, Which was “DoctorInCharge,” since all values were listed as “Confidential.”

### Step 2:
Check the distribution of continuous variables by histogram and boxplot. 
Histograms and Boxplots didn’t show any notable outliers for any continuous variable
![image](https://github.com/user-attachments/assets/8e5597af-ccda-46c6-ad14-6a6fac3a7c09)


### Step 3 
Check the frequency table for categorical variables.
Frequencies were good for all categorical variables.

### Step 4
Create dummy variables for categorical variables.
Since we did not combine any of our categories, we did not need to create dummy variables.
![image](https://github.com/user-attachments/assets/2d80d5b0-9f61-4256-b20a-802e393ddfc3)

We than go on excel to see if the table is very clean and there are no high correlations above 0.8 or below -0.8 So nothing to delete.
![image](https://github.com/user-attachments/assets/1b63529b-37bd-47e3-9143-a7f05a180154)

### Step 5
Generate pairwise correlation table and do collinearity check.
This table displays correlation between the variables and potential relations of interest.
Worth noting that Mini-Mental State Examination (MMSE), Functional Assessment And Activities of Daily Living  (ADL) had a slightly high negative correlation.
While Memory Complaints and Behavioral Problems had a slightly higher positive correlation

## Classifcations
### Logistic Regression 
Using Backwards Elimination, Stepwise Selection and Forward Selection
### kNN
Finding the best k and what variables we used by grouping data points based on similarity
### Classification and Regression Trees(CART)
Explains how our outcome variables value can be predicted based on other values


### Logistic Regression Analysis 
 Forward Selection Best Subset
![image](https://github.com/user-attachments/assets/a34e55fa-d47d-46e4-a86d-a98b6cce2b01)
### Forward Selection Coefficient Analysis
- The odds of being diagnosed with Alzheimer's disease for those who reported memory complaints is 13.54 times as the odds of being diagnosed with Alzheimer's disease for those who did not reported memory complaints (p value < 0.001).
- The odds of being diagnosed with Alzheimer's disease for those who reported behavioral problems is 11.8 times as the odds of being diagnosed with Alzheimer’s disease for those who did not report behavioral problems
![image](https://github.com/user-attachments/assets/6b40e8a4-848e-4ba6-9337-4db91339f57e)

Forward Selection Cutoff Ratio Analysis
![image](https://github.com/user-attachments/assets/089670ca-f314-4d02-b6f4-ec869640ce9e)
Relationship: As cutoff ratio increases, specificity increases and sensitivity (target class) decreases. Therefore a lower cutoff ratio of 0.3 is the most ideal since if we want high accuracy in Alzheimer's diagnosis. However cutoff ratio 0.5 gives us the lowest overall ER. 

### Backwards Elimination Best Subset
![image](https://github.com/user-attachments/assets/92888fab-3c6d-4728-8515-cb130eb37019)

### Backwards Elimination Coefficient Analysis
- The odds of being diagnosed with Alzheimer's disease decreases by approx. 37% for every point increase in their functional assessment (score ranges 0-10, lower score indicates greater impairment).
- Our outstanding variables have low p values < .05 which means there significant
![image](https://github.com/user-attachments/assets/4011e355-6a28-47aa-8f0c-e7c962c37fc3)

### Backwards Elimination Cutoff Ratio Analysis
Relationship: As cutoff increases specificity increases, and sensitivity decreases. A low cutoff ratio of 0.3 is the most ideal if we want high accuracy in Alzheimer's diagnosis. However if we are looking at smallest overall ER then cutoff ratio of 0.5 is ideal option.
![image](https://github.com/user-attachments/assets/6457f81d-83dc-4c0f-ac7b-38868d7e6898)


