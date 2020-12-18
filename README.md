<img src="img.jpeg">

**1. Introduction**

Civil wars are devastating and to prevent or at least contain them, accurately predicting their onset is crucial. In this paper, the authors focus on analysing the civil war onset predictive performance by comparing the performance of Random Forests (RFs), machine learning method applied in political science to increase predictive accuracy, with three logistic regression approaches, namely standard logistic regression, Firth’s penalized logistic regression and L1-regularized logistic regression models. The models were trained using cross-validation, which allows examining the predictive power of statistical models without collecting new data.

The evaluation of RFs and logistic regression of correctly predicting true instances of civil war onset through Receiver Operating Characteristic (ROC) curves showed that RFs performed excellently, while logistic regressors ranged from average to good. Moreover, RFs outperformed the other methods, in terms of both higher average F1-score and lower standard deviation. All in all, it was concluded from the results that statistical learning methods such as RFs have superior predictive accuracy in class imbalanced Civil War Dataset and can understand its causes. Accordingly RFs can be applied in the political science field, as they are easy to interpret, robust to outliers and allow correcting for class-imbalanced data.

In this extension, we explore methods to overcome the unbalance in the data classes. First, we apply data correction methods such as boosting and sampling on the same dataset used in the paper expecting to improve the logistic regression model’s accuracy. Then we explore other classifiers aiming to get the best possible predictive results on the corrected data. Cross validation is applied here as it produces unbiased and accurate error rates. In assessing the predictive performance, we use the following metrics; F1 score, Receiver Operating Characteristic Curve and AUC score.

**2. Results**

First, we started replicating what the authors did in the paper 
<img src="images/final/LR_replication.png">

<img src="images/LR_RF_separate_figures_replication_all_features.png">

<img src="images/final/KNN.png">

<img src="images/final/linear_SVM.png">

<img src="images/final/gradient_boost_all_features.png">


**3. Conclusion**
  

