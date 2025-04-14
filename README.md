# news classfication

## files:
2 notebooks (1 for preprocess, 1 for model), and 1 csv that stores the preprocessed data.

preprocess.ipynb, takes the original dataset NewsCategoryDataset_v3.json and outputs a cleaned version news_tokenized.csv.

news_tokenized.csv is used by logistic_regression.ipynb

## model:
Dataset: News_Category_Dataset_v3.json (Misra, 2018). Features:  'link', 'headline', 'category', 'short_description', 'authors', 'date'
Model: multi-class logistic regression model implemented using one-vs-rest (OvR) strategy.
Loss: Cross-entropy loss
Train: log_reg.fit(X_train, y_train)
Test: log_reg.predict(X_test)
