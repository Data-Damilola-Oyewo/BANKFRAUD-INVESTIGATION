# BANKFRAUD-INVESTIGATION
MACHINE LEARNING PREDICTION MODEL OF BANK FRAUD

Background
Blossom Bank also known as BB PLC is a multinational financial services group, that offers retail and investment banking, pension management, asset management and payments services, headquartered in London, UK.
Problem
There are occasional cases of fraudulent transactions in online payment which is staining the reputation of the bank. 

SOLUTION
Obviously, the financial institution is experiencing occasional fraudulent transactions and they intend to prevent such occurrences. The development of this machine learning model, when deployed into the bank application will assist to predict a transaction that will end as a fraudulent activities, and appropriate care such as Flags can then be raised to monitor such transactions.

The solution being proffered will enhance customer trust and confidence in the bank. This will result in the improved profitability of the organization as more customers will troop into the company.

The following activities were taken in sequence in developing the model
 
Step1: Loaded the dataset using pandas library
Step 2: Checked the dataset information 
Step 3: Confirmed the presence or absence of null values in the datasets
Step 4: Exploratory data analysis was performed on the data to understand the data more
These include the following: 
a.	Univariate graphs were explored using matplotlib and seaborn libraries
b.	Bivariate graphs were explored using matplotlib and seaborn libraries
c.	Multivariate graphs were explored using matplotlib and seaborn libraries
Step 5:  Observed the data correlation among columns
Step 6 : Encoding Type data (Categorical value) into numeric data
Step 7: Feature engineering was performed, resulting in dropping of irrelevant data
Step 8: Splitting data (Making train dataset to be 80% and test data to be 20%)
Step 9: Building the Model, RandomForestClassifier, Support Vector Machine, GradientBoostingClassifier, and NaiveBayes classifiers were used to model the data
Step 10: Evaluating our model by checking for Precision, Recall, F1 score and Confusion Matrix



CHALLENGES FACED
It took me some time to discover the extent of damage being caused by the 0.01% of the fraudulent transactions which I was determined to dig into. It is shocking to realize that 87% of the amount transacted was actually fraudulent.

OUTPUT
RandomForestClassifier, Support Vector Machine, GradientBoostingClassifier, and NaiveBayes were modelled in search for the fraudulent transactions.

	Random Forest Classifier	Support Vector Machine	Gradient Boosting Classifier	Naïve Bayes
RECALL	9%	0	9%	0%
PRECISION	100%   	0	100%	33.3%
F1 SCORE	17%	0	17%	1%
CONFUSION 
MATRIX	TP=
209474	FN=0
FP= 
219	TN=
22
	TP=
209474	FN =0
FP= 
241	TN=
0
	TP=
209474	FN= 0
FP = 219	TN=
22
	TP=
209472	FN=
2
FP = 240	TN=
1


I observed Accuracy metrics is not necessary here because it is an in balanced data set. Non-Fraudulent transactions is 99.9% whereas Fraudulent is around 0.1%. Recall, Precision and F1 are best for evaluation. The values are shown in the table above.
Random Forest Classifier and Gradient Boosting Classifier with exactly the same metrics value outperformed the remaining two classifiers. 
It is important to take cognizance of the True-Positive, which were the correctly predicted fraudulent transaction. The percentage of success alludes to the robustness of the RandomForest and Gradient Boosting Classifier. 
Attention must be paid however to the False-Negatives, which represent a portion that were predicted to be non-fraudulent, but which were in actual fact fraudulent transactions. Interestingly, the model had no occurrence of such.

