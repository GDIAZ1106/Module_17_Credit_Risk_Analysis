# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.


The objective of the analysis is to evaluate the performance of machine learning methods to accuralely predict credit risk. Once this analysis is performed have enough information to make a written recommendation on whether they should be used to predict credit risk.


## Results

### **- Oversampling Results: 63,66%**

The result of this test is above 50% but not sufficient. The report shows a good recall score but with low precision score resulting on a low f1 score. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/712ac0153b5b72a8e8b6943efd2ab31a92278e14/Resources/Naive%20Random%20Oversampling%20.png?raw=true"/>

### **- SMOTE Oversampling Results: 63.02%**
The report shows very low precision with low recall for high-risk predicting. Low risk predicting has high precision and low recall. Overall f1 score is low. Results are pretty similar than the previous method. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/SMOTE%20Oversampling%20.png?raw=true"/>


### **- Undersampling Results: 51,03%**
The accuracy score is low for undersampling recall and precision are low for both low and high-risk predictability.

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/49ae163bbfa06c9eef5c76782f8bdda3f7914445/Resources/Undersampling%20.png?raw=true"/>


### **- Combination (Over and Under) Sampling Results: 63,75%**
The accuracy score is similar to the other methods. The recall is moderate and precision is low for high-risk predicting. precision is high and recall is low for low-risk predicting. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Combine%20Under%20-%20Oversampling%20.png?raw=true"/>

### **- Ensemble Learners: Balanced Forest Classifier Result: 67,20% **
With a balanced random forest classifier of ensemble learning algorithm, the accuracy score is moderate, but higher than the rest of the methods.
The precision is moderate and recall is low for high-risk predicting. The precision and recall are 100% for low-risk predicting. Overall F1 score is very high. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Balanced%20Random%20Forest%20Classifier.png?raw=true"/>

### **-- Easy Ensemble AdaBoost Classifier Result: 92.54%**

With Easy Ensemble AdaBoost Classifier algorithm, the accuracy score is high.  
In the report, the precision is very low for high-risk predicting but high on sensitivity/recall. The low-risk predictability is high on precision and recall/sensitivity. Overall F1 score is high. F1 score for high-risk predicting is very low.

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Easy%20Assemble%20Adabost%20Classifier.png?raw=true"/>




## Summary: 

The best option to use in this type of activities a models with a high accuracy result but with the focus on having a high precision level. The idea is to avoid high risk candidtates as not risky, when in fact there is a high change of a default, in other words, we are trying to avoid false negative.


From all the algorithms performed, none showed a promising robust result to confidently predict our results except for the Easy Ensemble AdaBoost Classifier showed a high accuracy score of 0.92. On the other hand this method offer a low recall on the high risk candidates which is the most important risk that we should avoid (false negatives). I would say that the only method that can be used is the Easy Ensemble Balance Forest Classifier since offer a higher recal of 73%.

I would be recommendable also to try to increase the size of the database in order to have a bigger universe of high-risk candidates that could help the methods to increase the recall. 

