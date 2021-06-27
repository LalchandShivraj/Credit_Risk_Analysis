# Credit_Risk_Analysis
![credit_risk_header](https://user-images.githubusercontent.com/78666055/123553409-ff8d4e80-d748-11eb-9d13-bfaae2c0736b.png)

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. So, machine learning will have to be employed to solve this challenge.
Jill requested the use of imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

### Task at hand:
Use the credit card credit dataset from LendingClub, a peer-to-peer lending service company. Oversample the data using RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. After also using the combinatorial approach of the SMOTEENN algorithm, compare the two machine learning models: BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk.

# Results

### Naive Random Oversampling
The performance of this algorithm, low accuracy and low percentage precision on high risk loans is not a fovourable choice.
* Balanced Accuracy Score: 66% 
* Precision (High and Low risk respectively): 1% and 100% 
* Recall (High and Low risk respectively): 74% and 58% 

![naive_random_oversampling](https://user-images.githubusercontent.com/78666055/123552210-26488680-d743-11eb-9d4a-49c31cde06bf.png)

### SMOTE Oversampling
The performance of this algorithm, low accuracy and low percentage precision on high risk loans is not a fovourable choice.
* Balanced Accuracy Score: 65% 
* Precision (High and Low risk respectively): 1% and 100% 
* Recall (High and Low risk respectively): 62% and 68% 

![smote_oversampling](https://user-images.githubusercontent.com/78666055/123552219-2cd6fe00-d743-11eb-9412-30aa355e069f.png)

### ClusterCentroid Undersampling
The performance of this algorithm, low accuracy and low percentage precision on high risk loans is not a fovourable choice.
* Balanced Accuracy Score: 54%
* Precision (High and Low risk respectively): 1% and 100%
* Recall (High and Low risk respectively): 69% and 40%
![clustercentroid_undersampling](https://user-images.githubusercontent.com/78666055/123552222-33657580-d743-11eb-9613-b5b44624020c.png)

### SMOTEENN Combination (Over and Under) Sampling
The performance of this algorithm, low accuracy and low percentage precision on high risk loans is not a fovourable choice.
* Balanced Accuracy Score: 54%
* Precision (High and Low risk respectively): 1% and 100%
* Recall (High and Low risk respectively): 70% and 57%
![smoteenn_combination_sampling](https://user-images.githubusercontent.com/78666055/123552230-3e200a80-d743-11eb-8037-5dd1e272a4a8.png)

### Balanced Random Forest Classifier
The performance of this algorithm, good accuracy percentage precision on high risk loans certainly is better than the preceding algorithms.
* Balanced Accuracy Score: 79%
* Precision (High and Low risk respectively): 3% and 100%
* Recall (High and Low risk respectively): 70% and 87%
![balanced_random_forest_classifier](https://user-images.githubusercontent.com/78666055/123552242-4aa46300-d743-11eb-804a-74d05c78e9b3.png)

### Easy Ensemble AdaBoost Classifier
The performance of this algorithm, high accuracy and better percentage precision on high risk loans than other algorithms, make this the best option.
* Balanced Accuracy Score: 93%
* Precision (High and Low risk respectively): 9% and 100%
* Recall (High and Low risk respectively): 92% and 94%
![easy_ensemble_adaboost_classifier](https://user-images.githubusercontent.com/78666055/123552248-52640780-d743-11eb-87a5-562613cff492.png)

# Summary
The first four algorithms (Naive Random Sampling, SMOTE Oversampling, ClusterCentroid Undersampling and SMOTEENN Conbination Sampling) did not produce favourable results. The Balanced Random Forest Classifier did show improvement over the four mentioned, however, the Easy Ensemble AdaBoost Classifier would be the best choice, given it's accuracy, precision and recall values overall.
