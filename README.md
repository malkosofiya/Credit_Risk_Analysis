# Credit_Risk_Analysis

## Overview of the analysis

The purpose of this analysis is to use machine learning techniques to predict credit risk. To achive this goal a several different approaches were used to train and evaluate data models. Firstly, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and then undersampled the data using the ClusterCentroids algorithm. Afterwards, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm was deployed.  Finally, two machine learning models were compared that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier. 

## Results

* Naive Random Oversampling

Overall, this model may not be the best one for credit risk predictions because the model's accuracy, 66.5%, is relitavly low, and the precision for high risk loaners, 1%, is really low as well. 

<img width="822" alt="Screen Shot 2022-12-05 at 9 38 30 PM" src="https://user-images.githubusercontent.com/110862261/205807166-87b18452-161e-49c4-9f74-940cd0d197c0.png">

* SMOTE Oversampling

This model provided similar results to Naive Random Oversampling with accuracy of 66.4% and precision for high risk loaners of 1%. 

<img width="821" alt="Screen Shot 2022-12-05 at 9 47 56 PM" src="https://user-images.githubusercontent.com/110862261/205808269-f680d9ac-6fc8-4e99-afe7-07ed654796fc.png">

* Undersampling 

Balanced accuracy score was alliged with previous models at 66,4%. The recall is also low for the low risk loaners, which is indicative of a large number of false possitives.Taking in account both precision and recall scores are not good enough to state that the model will be good at classifying credit risks.

<img width="818" alt="Screen Shot 2022-12-05 at 9 55 02 PM" src="https://user-images.githubusercontent.com/110862261/205809221-42047aeb-ae51-4fb0-92e8-b06c3ce7c3ab.png">

* Combination (Over and Under) Sampling

Overall, this module performed worth that the previous models. It is not good at predict credit risk due to the model's accuracy, 54,5%, and F1 score being low.

<img width="826" alt="Screen Shot 2022-12-05 at 10 01 10 PM" src="https://user-images.githubusercontent.com/110862261/205810087-979ff45e-1515-48da-a143-da1087f73848.png">

* Balanced Random Forest Classifier

Balanced accuracy score increased to 78.8% as well as precision for high risk loaners to 4%. The recall remained similar to the other models at 67% for high risk loans and 91% for low risk loans.

<img width="791" alt="Screen Shot 2022-12-05 at 10 04 19 PM" src="https://user-images.githubusercontent.com/110862261/205810996-21a592a5-6af2-4a1e-9ef1-a56e33f77f10.png">

* Easy Ensemble AdaBoost Classifier

Overall, the model performed better than the others with an accuracy of 92.5% and a high-risk prediction of 7%. The f1 score is alo higher when compared at an average of 97%.

<img width="791" alt="Screen Shot 2022-12-05 at 10 04 19 PM" src="https://user-images.githubusercontent.com/110862261/205811663-bf4afbc2-8b47-4730-83da-26a7ee4fe23e.png">
