# SMSSpam-Classifier
This is Spam and Ham Classifier
Spam messages are messages sent to a large group of recipients without their prior consent, typically advertising for goods and services or business opportunities.
In the recent period, the percentage of scam messages amongst spam have increased sharply. Scam messages typically trick people into giving away money or personal details by offering an attractive or false deal. 
A spam message classification is a step towards building a tool for scam message identification and early scam detection.

# Dataset

The dataset is from Kaggle, a collection of spam SMS messages, with 5572 messages, all classified as either ‘ham’ or ‘spam’. The dataset contains 13.4% spam and 86.6% ham.

# Methodology
The methodology is divided into
1.	Data Pre-processing and Exploratory Data Analysis
2.	Model Training, Comparison and Selection
3.	Model Evaluation

# Email-Spam-Classifier-Using-Naive-Bayes

Naive Bayes is a supervised classification technique based on Bayes' Theorem with an assumption of independence among predictors. That is, a Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature.

It is a popular technique for text categorization, judging documents as belonging to one category or the other (such as spam or legitimate, sports or politics, etc.) with word frequencies as features.

# Model Training

The models used are Logistic Regression, k-Nearest Neighbors classifier, Random Forest classifier, Bernoulli Naïve Bayes classifier and Complement Naïve Bayes classifier.

Count Vectorizer is used to encode the documents into vectors as input into the models for training and test. In addition, Tfidf vectorizer, Count Vectorizer with Latent Semantic Analysis, Count Vectorizer with Latent Dirichlet Allocation has been used with the Logistic Regression model.

The data is split into 80% train and validation set, 20% test set. Grid Search CV is applied across 10 folds on the data, to find the best hyperparameters for all the models. Prediction is based on the average of 10 predictions.

# Conclusion
A model with a 100% precision has been built. Precision is valued over recall so that ham messages will not be misclassified as spam.

A more customized pre-processing step will contribute to a more precise model. 

For this dataset, linear models with high bias and low variance like the Logistic Regression and Naïve Bayes classifier have performed better than non-linear models like k-Nearest Neighbor classifier and Random Forest classifier.

