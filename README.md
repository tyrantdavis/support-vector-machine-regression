# Building an SVM Model for Regression

## [Demo](https://nbviewer.org/github/tyrantdavis/support-vector-machine-regression/blob/main/svm-regression.ipynb)

---

### Scenario
Up to this point, training has been done working with housing datasets using various models. These models have enabled the median house value estimations in specific regions based on several factors. However, it has been observed that certain outliers in the dataset could be hindering the accuracy of the predictions. There are multiple strategies to tackle outliers, but one of the most efficient methods is to utilize Support Vector Machines (SVMs). Therefore, you plan to retrain the dataset using SVM regression models to enhance your predictions of housing prices.


**Data Sources:**

- data/cali_house_data.pickle

## Project Goals
The goal is to analyze California housing data particularly around various attributes for the homes observed in the area and their prices while also teaching students about the different elements that can influence these predictions. Additionally, another aim is to evaluate how well a Logistic Regression model performs in classification compared to the predictive abilities of a Support-Vector Machine regression model.

Several questions will be asked:

1. Is the SVM regression model effective in enhancing prediction accuracy?

2. How is the MEDINC feature connected to the target feature, which is price?

3. In what ways does the SVM regression boundary correspond with the data compared to the logistic regression boundary?

4. What is the median house value?





#### Why use a support-vector machine algorithm to predict the classification?
Support Vector Machines (SVMs) are particularly effective for classification problems that involve training datasets containing outliers. In such scenarios, SVMs often demonstrate superior performance compared to logistic regression and various other classification methods.  A support-vector machine demonstrates significant efficacy in data classification, making it a suitable choice for the goals of this project. An instance of data can represent one category while simultaneously not belonging to another.


## Data
A dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 20640 housing records. 


## Conclusions
1. Is the SVM regression model effective in enhancing prediction accuracy?
    - Yes. The cost error decreased to 0.6110 and is even lower than that of the top-performing linear regression models.

2. How is the MEDINC feature connected to the target feature, which is price?
    - Generally, 'target' - the value of a home tends to increase as MEDINC(income) levels rise. 
3. In what ways does the SVM regression boundary correspond with the data compared to the logistic regression boundary? 
    - The linear regression boundary does not effectively address the outliers while the SVM regression boundary takes into account the outliers, utilizing them as support vectors in its decision-making process. This means that these unusual data points play a crucial role in shaping the model's predictions.
4. What is the median house value?
    - The median house value is $179700.00 
