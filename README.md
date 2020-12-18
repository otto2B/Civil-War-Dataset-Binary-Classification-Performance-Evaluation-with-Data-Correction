<img src="img.jpeg">

**1. Introduction**

Civil wars are devastating and to prevent or at least contain them, accurately predicting their onset is crucial. In this paper, the authors focus on analysing the civil war onset predictive performance by comparing the performance of Random Forests (RFs), machine learning method applied in political science to increase predictive accuracy, with three logistic regression approaches, namely standard logistic regression, Firth’s penalized logistic regression and L1-regularized logistic regression models. The models were trained using cross-validation, which allows examining the predictive power of statistical models without collecting new data.

The evaluation of RFs and logistic regression of correctly predicting true instances of civil war onset through Receiver Operating Characteristic (ROC) curves showed that RFs performed excellently, while logistic regressors ranged from average to good. Moreover, RFs outperformed the other methods, in terms of both higher average F1-score and lower standard deviation. All in all, it was concluded from the results that statistical learning methods such as RFs have superior predictive accuracy in class imbalanced Civil War Dataset and can understand its causes. Accordingly RFs can be applied in the political science field, as they are easy to interpret, robust to outliers and allow correcting for class-imbalanced data.

In this extension, we explore methods to overcome the unbalance in the data classes. First, we apply data correction methods such as boosting and sampling on the same dataset used in the paper expecting to improve the logistic regression model’s accuracy. Then we explore other classifiers aiming to get the best possible predictive results on the corrected data. Cross validation is applied here as it produces unbiased and accurate error rates. In assessing the predictive performance, we use the following metrics; F1 score, Receiver Operating Characteristic Curve and AUC score.

**2. Results**

First, we started replicating what the authors did in the paper *Comparing Random Forest with Logistic Regression for
Predicting Class-Imbalanced Civil War Onset Data*. In addition, we used oversampling to test and as we will see in the table at the end, it gave better performances in terms of F1 score.

<img src="images/final/LR_replicationn.png">

In a second time, we decided to change an aspect of their paper, which was that the models they compared did not have the same features. It was thus not accurate to compare them. We decided to use all the features we could to train our models.

<img src="images/LR_RF_separate_figures_replication_all_features.png">

What came out of this first change is that, without any surprise, the regression stays less performant than the random forest. Though it performed better when using the data correction methods we used, that is to say oversampling and adaboost. We did not use undersampling because of the lack of sample in the minority class.

Oversampling generates new data points for the minority to have the same amount than the majority class.We decided to use the Synthetic minority oversampling technique (SMOTE) that generates new samples between existing data points based on local density and their border with the other class. It is an informed oversampling method that is less prone to overfitting than a random oversampling method.

Boostings methods are algorithms that convert weak learners into strong learners in order to improve the prediction power. It will first identify the weak learners and combine them into one strong learner. 

We then tried several models in order to find one that could surpass the final model of the paper.

<img src="images/final/KNN.png">

<img src="images/final/linear_SVM.png">

<img src="images/final/gradient_boost_all_features.png">

To draw a first conclusion, the only model that performed better was gradient boosting, as we can see on the ROC curves.


**3. Conclusion**
  

