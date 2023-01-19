# Assignment 18: Loan Analysis

The purpose of this analysis was to assess the abilities of supervised machine learning in deciding if someone's
loan application would be considered Low or High risk. Over and undersampling were used in conjunction with
logistic regression to parse the loan data CSV to generate classification reports and accuracy scores, to determine which model would be most effective for our purposes.

###For the Purpose of this analysis###

* 0 Refers to Low-Risk Loan Opportunities
* 1 Refers to High-Risk Loan Opportunities

## Results

The results of the Tests were as follows:
!["OverSample"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/1Oversampling.PNG)
* Oversampling
	* Balanced Acc. Score: .66
	* Precision Score: .99
	* Recall Score: .60

----
!["SMOTE"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/2SMOTE.PNG)
* SMOTE
	* Balanced Acc. Score: .65
	* Precision Score: .99
	* Recall Score: .70

----
!["UnderSample"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/3ClusterUndersampling.PNG)
* Undersampling
	* Balanced Acc. Score: .54
	* Precision Score: .99
	* Recall Score: .40

----
!["SMOTEEEN"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/4SMOTEEEN.PNG)
* SMOTEEEN (Over/Under)
	* Balanced Acc. Score: .65
	* Precision Score: .99
	* Recall Score: .57

----
!["BalancedForest"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/5BalancedForest.PNG)
* BalancedForest
	* Balanced Acc. Score: .77
	* Precision Score: .99
	* Recall Score: .89

----
!["EasyEnsemble"](https://github.com/Jelsik/Credit_Risk_Analysis/blob/main/picsforSUPLEARN/6EasyEnsemble.PNG)
* EasyEnsemble
	* Balanced Acc. Score: .92
	* Precision Score: .99
	* Recall Score: .90


## Summary:

The initial models all contain a high precision, but their recall scores lag somewhat behind, leading to an
accuracy score general in the 50s to 60s. Considering the facts involved with these predictions relating to
potential financial loss to the institution, these accuracy numbers do not fill me with confidence. The dataset
used may contain too many rows to consider, throwing the algorithm off with erroneous data, or the fact that
the actual data set only contains.

When moving on to ensemble models, the results improve. Balanced forest brings accuracy into the 70s,
and the EasyEnsemble group brings an accuracy score of a respectable 91.5%. This model also has a good F1
score with high points in precision and recall. If a model was to be used to predict loan risk, this would
be the one.
