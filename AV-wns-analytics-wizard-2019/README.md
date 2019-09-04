# Analytics Vidya - WNS Analytics Wizard 2019
Repository for the WNS Analytics Wizard 2019 Challenge based on Ad-click prediction on the basis of History logs, Item data and Train data for last three months.

The Challenge is from the page:
https://datahack.analyticsvidhya.com/contest/wns-analytics-wizard-2019

XGBoost provided best accuracy ~60% on test data. 
Here is a brief of the approach followed:<br />
a) Imputing/managing NANs(is any), Removing the duplicates. EDA using value_counts and pair plots for feature analysis.<br />
b) Dummies for categorical variables - No scaling.<br />
c) Correlation of independent features with target as well as within independent features.<br />
d) SMOTE for upscaling as the original data is biased(95:5 ratio on target variable). Only done on train data after splitting original data using the train_test_split.<br />
e) Standard Scaling for continuous independent features. Fit_transform on train and validation set, transform only on test set.<br />
f) Ensemble models and DNNs for modelling.<br />
g) Accuracy using ROC and Confusion Matrix.<br />


