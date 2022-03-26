# Credit_Risk_Analysis

## Overview of the analysis: Explain the purpose of this analysis.


The objective of the analysis is to evaluate the performance of machine learning methods to accuralely predict credit risk. Once this analysis is performed have enough information to make a written recommendation on whether they should be used to predict credit risk.


## Results

### **- Oversampling Results: 63,66%**

The result of this test is above 50% but not sufficient. The report shows a good recall score but with low precision score resulting on a low f1 score. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Undersampling%20.png?raw=true"/>

### **- SMOTE Oversampling Results: 63.02%**


The report shows very low precision with low recall for high-risk predicting. Low risk predicting has high precision and low recall. Overall f1 score is moderate. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/SMOTE%20Oversampling%20.png?raw=true"/>


### **- Undersampling**
The accuracy score is low for undersampling.



recall and precision are low for both low and high-risk predictability.

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Undersampling%20.png?raw=true"/>




### **- Combination (Over and Under) Sampling**
The accuracy score is moderate for combined over and under-sampling.



the recall is moderate and precision is low for high-risk predicting. precision is high and recall is low for low-risk predicting. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Combine%20Under%20-%20Oversampling%20.png?raw=true"/>

### **- Ensemble Learners: Balanced Forest Classifier**
With a balanced random forest classifier of ensemble learning algorithm, the accuracy score is moderate. 


The precision is moderate and recall is low for high-risk predicting. The precision and recall are 100% for low-risk predicting. Overall F1 score is very high. 

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Balanced%20Random%20Forest%20Classifier.png?raw=true"/>

### **-- Easy Ensemble AdaBoost Classifier**

With Easy Ensemble AdaBoost Classifier algorithm, the accuracy score is high.  



In the report, the precision is very low for high-risk predicting but high on sensitivity/recall. The low-risk predictability is high on precision and recall/sensitivity. Overall F1 score is high. F1 score for high-risk predicting is very low.

<p align = "center">
<img src ="https://github.com/GDIAZ1106/Module_17_Credit_Risk_Analysis/blob/ec19dcdbc625b4e8114c8732109ffc86d130c274/Resources/Easy%20Assemble%20Adabost%20Classifier.png?raw=true"/>




## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

In our case, when we are trying to screen candidates for a loan, we do not want too many high-risk candidates labeled as low risk for our model. In other words, we want fewer false negatives. Therefore a high precision predicting algorithm is more important. We will lose low-risk candidates in the process but that will be better than letting too many high-risk candidates through.  

Out of all the algorithms performed, none showed a promising robust result to confidently predict our results. Most of the models show very low precision scores and only the Easy Ensemble AdaBoost Classifier showed a high accuracy score of 0.92. Some reasons that might be causing this are due to weak data and weak learners in the data. We just don't have enough high-risk applicant data to make our models predict better. 

The highest precision score resulted in an ensemble balanced forest classifier with 0.73 and is moderate but not high. The F1 score for this model was very high due to the high precision and sensitivity of low risk predicting pushing this score to 1.0. This means that the ensemble balanced forest classifier detected all the low-risk applicants correctly but was not sensitive or very precise at finding the high-risk applicants. The accuracy score of this model was not strong but higher than fifty percent at 0.62. Overall this is a good model to use but does not show strong reliability. 

There are deeper trade-offs to take into consideration in this case. a low and high risk is vague and may have variance within its definition. An individual high-risk applicant could have a criminal record while the other high-risk applicant is high in debt. In this example, risks could be interpreted differently. For discussions like these, perhaps letting some high-risk applicants is a sacrifice the loan lending company can afford to take to profit higher in the long term. Then the ensemble AdaBoost classifier is more exceptional to use because it has very high sensitivity numbers with a high accuracy score. 
