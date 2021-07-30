# Email Anomaly Detection

This is a project to detect anomalies (i.e., spam, phishing) in email datasets using machine learning and features extracted from email headers. A total of 96 features are extracted. Both supervised and unsupervised learning is used, with supervised learning achieving 99%+ accuracy and unsupervised achieving 87-90% accuracy. 

Two datasets are used, which were obtained from:
(1) https://plg.uwaterloo.ca/~gvcormac/treccorpus07/about.html
(2) https://monkey.org/~jose/phishing/

The first dataset (1) contains both spam and ham emails, while the second dataset contains phishing emails. The first dataset was parsed using the 'Capstone project - Extract HamSpam.ipynb' notebook. The second dataset (2) was parsed using the 'Capstone Project - Extract Phishing.ipynb' notebook. The resulting .CSV files are all parsed by the 'Capstone Project - Preproccess + Feature Extraction.ipynb' notebook, which outputs the 'preprocessed_spam_ham_phishing.csv' file. The 'preprocessed_spam_ham_phishing.csv' file contains the information used during the training and testing of learning algorithms.

The class labels in the preprocessed_spam_ham_phishing.csv are:
0: ham emails
1: spam emails
2: phishing emails

Four rounds of testing were performed:
1) Supervised learning, ham and spam email classification
2) Supervised learning, ham and phishing email classification
3) Unsupervised learning, ham and spam email classification
4) Unsupervised learning, ham and phishing email classification