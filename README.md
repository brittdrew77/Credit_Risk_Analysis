# Credit_Risk_Analysis
## 1. Overview of the analysis
The purpose of this analysis was to use different methods to train and evaluate models with unbalanced classes. I resampled data using oversampling (RandomOverSampler and SMOTE), undersampling (ClusterCentroids), and a mix of both (SMOTEENN). Then, I compared two models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias to predict credit risk. 

## 2. Results

* The first machine learning model I used was naive random oversampling. The balanced accuracy score was 0.6479 which is not very impressive. This is the percentage of correct predictions. The precision for this model was 0.99, which is very good. Precision is how reliable a positive classification is. Next, the recall or sensitivity was 0.67, rather low. Recall is the percentage of actual positive results that were predicted correctly. 

* The second machine learning model was SMOTE oversampling. This model had a balanced accuracy score of 0.6418, which is lower than the previous model. The precision was 0.99 and the recall was 0.65, also lower than before. 

* The third model was undersampling using the cluster centroids algorithm. The balanced accuracy score was 0.5293, much lower than the first two models. The precision was 0.99 and recall was only 0.45. This model is clearly worse than the oversampling models. 

* The next machine learning model was a combination of under- and over-sampling using the SMOTEENN algorithm. The balanced accuracy score was still unimpressive being 0.6467. The precision, 0.99, was high like the others, but the recall, being 0.59, was rather low. 

* The last two machine learning models involve ensemble algorithms. The first I used was a Balanced Random Forest Classifier. This model had a balanced accuracy score of 0.7874, much higher than the previous models. The precision was 0.99 and recall 0.88. It is apparent that this model is the best overall so far. 

* The last model was the Easy Ensemble AdaBoost Classifier. This model appeared best overall with a balanced accuracy score of 0.925. The precision was 0.99 and recall was 0.94.

## 3. Summary
