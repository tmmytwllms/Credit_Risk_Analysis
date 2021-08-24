# Credit_Risk_Analysis

## Overview 
<br/>
<br/>

The purpose of this analysis was to use supervised machine learning to determine a loan applicant's credit risk. Several machine learning models were trained and tested on the dataset to determine an optimal model for predicting credit risk. These models included resampling models, SMOTEENN, and ensemble classifiers. 
<br/>
<br/>

## Results

### 1. Naive Random Oversampling
- This model had an accuracy of 65%.
- This model had a near-perfect precision of 100% for detecting the low risk applicants. This tradeoff equates to it having very low precision in detecting high risk applicants.
- Recall is 59% for low risk applicants and 72% for high risk applicants.
<br/>

![naive_random_oversampling](https://user-images.githubusercontent.com/82389466/130539062-c3c35183-0074-4f11-bbc1-52203b56d800.png)
<br/>

### 2. SMOTE Oversampling
- This model had an accuracy of 66%.
- This model had a near-perfect precision of 100% for detecting low risk applicants. Again, this is a tradeoff for the precision of 1% for high risk applicants.
- Recall is 63% for high risk applicants, and 69% for low risk applicants.
<br/>

![Smote_oversampling](https://user-images.githubusercontent.com/82389466/130539808-87480cb7-ac12-4e86-ab07-279deff2f939.png)
<br/>

### 3. Undersampling
- This model had an accuracy of 52%.
- This model had another near-perfect precision for low risk applicants, and again a very low 1% precision for high risk applicants.
- Recall is 69% and 40% for high and low risk applicants, respectively.
<br/>

![undersampling](https://user-images.githubusercontent.com/82389466/130540000-e362da41-8a77-485e-9367-eb4c10bd095d.png)
<br/>

### 4. Over and Undersampling Combination
- This model had an accuracy of 66%.
- This model had another near-perfect precision for low risk applicants, and again a very low 1% precision for high risk applicants.
- Recall is 58% and 75% for high and low risk applicants, respectively.
<br/>

![under_over](https://user-images.githubusercontent.com/82389466/130540113-9975e350-51b4-4f03-b7b7-794f50ecf8a7.png)
<br/>

### 5. Balanced Random Forest Classifier
- This model had an accuracy of 78%.
- This model had another near-perfect precision for low risk applicants, and a slightly higher but  very low 3% precision for high risk applicants.
- Recall is 70% and 80% for high and low risk applicants, respecitively. 
<br/>

![balanced_random_forest](https://user-images.githubusercontent.com/82389466/130540201-b7594b44-0891-46ef-8aeb-4c1ec5c0678c.png)
<br/>

### 6. Easy Ensemble AdaBoost Classifier
- This model had an accuracy of 93%.
- This model had another near-perfect precision for low risk applicants, and a slightly higher still but very low 9% precision for high risk applicants.
- This model had a recall of 92% and 94% for high and low risk applicants, respectively.
<br/>

![easy_ensemble_adaboost](https://user-images.githubusercontent.com/82389466/130540325-99e669b3-2ecf-412b-84cb-8a59ae7bf431.png)
<br/>

## Summary
To summarize, we can see that as we start with simpler supervised machine learning models, such as oversampling or undersampling alone, we see lower accuracy and recall percentages. As we move to more complex machine learning models, we beging to see more accurate results as the data tests and retests itself to improve upon its mistakes. 

I would reccommend unsing the Easy Ensemble AdaBoost Classifier, as it saw the highest accuracy and recall. This model would be best for determining low risk applicants, but similarly to the other models, fails to reliably identify high risk applicants.
