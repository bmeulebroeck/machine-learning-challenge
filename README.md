# machine-learning-challenge

### Feature Selection
Being new to the subject matter, I started by researching the dataset to determine what some of the columns mean and also looked into a few articles on feature selection for machine learning. 

I decided to remove the uncertainty columns for each possible feature to simplify the dataset, then started by putting the remaining columns through a correlation matrix to see where there may be relationships.
![Correlation Matrix](screenshots/exoplanet_features_corr.png)

I also used an information gain calculation method I found in the SciKit Learn documentation (explained on: https://www.analyticsvidhya.com/blog/2020/10/feature-selection-techniques-in-machine-learning/) to see which factors scored highest.
![Information Gain](screenshots/info_gain.png)

These are in the 'corr.ipynb' notebook.

I also found an article that covered using RandomForest importances to help guide feature selection and decided to run that analysis (in the 'random_forest.ipynb' notebook).

After completing this analysis - I had a narrowed down list of features to try with my models.

### Models Run
1. Logistic Regression and then GridSearch to tune: scored 0.8153
2. Deep Learning Neural Network: scored 0.8878
3. K-Nearest Neighbors: scored 0.867

I tried several variations on scaling and features to see how it impacted the final scoring in each model - notes are in the comments in each notebook.