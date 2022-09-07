# Credit_Risk_Analysis
## 1. Overview of the analysis
The purpose of this analysis was to use different methods to train and evaluate models with unbalanced classes. I resampled data using oversampling (RandomOverSampler and SMOTE), undersampling (ClusterCentroids), and a mix of both (SMOTEENN). Then, I compared two models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias to predict credit risk. 

## 2. Results

<img width="722" alt="Screen Shot 2022-09-06 at 7 54 57 PM" src="https://user-images.githubusercontent.com/105089651/188762304-df54c157-09e8-439b-9fac-aee146b6fa63.png">

* The first machine learning model I used was naive random oversampling. The balanced accuracy score was 0.6479 which is not very impressive. This is the percentage of correct predictions. The precision for this model was 0.99, which is very good. Precision is how reliable a positive classification is. Next, the recall or sensitivity was 0.67, rather low. Recall is the percentage of actual positive results that were predicted correctly. 

<img width="649" alt="Screen Shot 2022-09-06 at 8 17 12 PM" src="https://user-images.githubusercontent.com/105089651/188762308-41966ab2-8f24-4554-ba90-681c229839a3.png">

* The second machine learning model was SMOTE oversampling. This model had a balanced accuracy score of 0.6418, which is lower than the previous model. The precision was 0.99 and the recall was 0.65, also lower than before. 

<img width="640" alt="Screen Shot 2022-09-06 at 8 17 48 PM" src="https://user-images.githubusercontent.com/105089651/188762315-eb29c8d1-1fa0-4c34-a0c4-09d27afef993.png">

* The third model was undersampling using the cluster centroids algorithm. The balanced accuracy score was 0.5293, much lower than the first two models. The precision was 0.99 and recall was only 0.45. This model is clearly worse than the oversampling models. 

<img width="642" alt="Screen Shot 2022-09-06 at 8 18 14 PM" src="https://user-images.githubusercontent.com/105089651/188762321-d83ffe53-96b9-4929-98e9-3b6f0d88d04a.png">

* The next machine learning model was a combination of under- and over-sampling using the SMOTEENN algorithm. The balanced accuracy score was still unimpressive being 0.6467. The precision, 0.99, was high like the others, but the recall, being 0.59, was rather low. 

<img width="639" alt="Screen Shot 2022-09-06 at 8 18 46 PM" src="https://user-images.githubusercontent.com/105089651/188762328-fe7f1d01-c5b4-4cc5-a1f8-72a7cb6d7467.png">

* The last two machine learning models involve ensemble algorithms. The first I used was a Balanced Random Forest Classifier. This model had a balanced accuracy score of 0.7874, much higher than the previous models. The precision was 0.99 and recall 0.88. It is apparent that this model is the best overall so far. 

<img width="647" alt="Screen Shot 2022-09-06 at 8 19 14 PM" src="https://user-images.githubusercontent.com/105089651/188762301-b9513f0d-cdb9-4d66-95bc-3f435fa87edb.png">

* The last model was the Easy Ensemble AdaBoost Classifier. This model appeared best overall with a balanced accuracy score of 0.925. The precision was 0.99 and recall was 0.94.

## 3. Summary

The results displayed that the best machine learning models were the ensemble algorithm types, while undersampling was the worst based on balanced accuracy scores, precision, and recall. I would recommend using the last model: Easy Ensemble AdaBoost Classifier, since it had the highest scores, especially with an f1 score of 0.97. It is clearly the most accurate model. 

<img width="642" alt="Screen Shot 2022-09-06 at 8 31 33 PM" src="https://user-images.githubusercontent.com/105089651/188763170-5f1c9fae-853d-4faa-b67f-4d6e088fc286.png">
