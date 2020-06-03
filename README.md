## Kaggle House Pricing - Advanced Regression Challenge

### Rank = 677
(rank as of this commit)

Files:
* HousePricingDataProcessing: Pre-processing of features. 
	* Used [this](https://www.kaggle.com/agodwinp/stacking-house-prices-walkthrough-to-top-5) notebook as a coarse guide and learn what steps can be taken.
	* Saves training and test(for submission) data after feature engineering
* SearchFeatureSelector: Runs a search over bayesian regression using different numbers of important features for fitting
* HousePricingV3: Implements the House pricing regression
	* reads processed data
	* handles categorical data - one hot encoding
	* applies multiple regression techniques
		* linear regression (with and without log on target)
		* Random Forest
		* Lasso
		* NN
		* Bayesian Regression
		* XG Boost
	* Try stacking of these models
	* Use result from SearchFeatureSelector to get the best relevant features and use them for fitting bayesian (since it was giving the best results) 
	* run on all data before generating final submission
* You can download the [file](https://www.kaggle.com/moradnejad/perfect-score-for-evaluation-purposes) with actual correct values on test data OR remove lines of code with "full-score.csv" in all files.


