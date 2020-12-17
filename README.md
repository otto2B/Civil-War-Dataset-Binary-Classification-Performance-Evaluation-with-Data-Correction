![alt text](https://miro.medium.com/max/1200/1*N5wTuuEAq8GU4zlomwWLiQ.jpeg)


Abstract

The paper Comparing Random Forest with Logistic Regression for Predicting Class-Imbalanced Civil War Onset Data shows that Random Forests have a significantly higher predictive accuracy than logistic regression models. While the authors focus on comparing the performance of statistical methods, namely Random Forests and three logistic regression versions in predicting civil war onset in out-of-sample data, we will focus on improving the predictive performance of civil war onset.

In this extension, we will explore methods to overcome the unbalance in the data classes. First, we will apply data correction methods such as boosting or sampling on the same dataset used in the article, expecting to improve the logistic regression model’s accuracy. Then we will explore other classifiers aiming to get the best possible predictive results on the corrected data. Cross validation is applied here as it produces unbiased and accurate error rates. In assessing the predictive performance, we use the metrics, Confusion matrix, F1 score, Receiver Operating Characteristic Curve and AUC score.

Research Questions

a) How correcting imbalanced datasets through boosting, sampling, and cost-sensitive methods can help improve the predictive performance of a classifier?

b) How different classifiers (e.g SVM, Naive Bayes, KNN) perform on corrected imbalanced datasets?

Proposed dataset

The main dataset we will use is the provided Civil War Data (CWD) dataset (SambnisImp.csv). It measures from 1945 to 2000 whether a civil war occured in a given country, in a given year. We will then use sampling methods on the dataset to try to overcome the dataset unbalance.

Methods

a) Imbalanced data correction

i) Boosting techniques (AdaBoost/Gradient Boosting)
ii) Sampling methods (Oversampling/Undersampling)
iii) Cost-Sensitive Learning (upweighting/down-weighting)
b) Classifiers to test

i) Logistic Regression
ii) KNN
iii) Naive Bayes
iv) SVM
c) Cross validation

d) Assessment Metrics

i) Confusion matrix
ii) F1 score
iii) Receiver operating characteristic curve
iv) AUC score

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/otto2B/p4_presentation_test/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/otto2B/p4_presentation_test/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
