Project developed as partial requirement for the advanced predictive analysis discipline in Business Analytics and Big Data postgraduation degree.

Fictious Case:

In order to relate the chemical characteristics of its wines to the quality perceived by its consumers, the luxury conglomerate LVMH (Moët Hennessy Louis Vuitton) asked its data scientist João Vitor de Paiva Marcotti to develop a predictive binomial classification model.

The wines analyzed belong to the brands Château Cheval Blanc and Château d'Yquem, both renowned wineries, with bottles priced above $3,000 and focused on demanding, refined and high-income customers.

A multilabel problem with grades from 0 to 10 was transformed in a binary one following this rule:
- Reproved: wines rated between 0 and 5.
- Approved: wines rated between 6 and 10.

Logistic Regression, SVM, Naive Bayes, Neural Networks and Random Forest models were tested and the one with the best combination of MSE, accuracy, F1, recall and AUC metrics, was selected through grid search, cross-validation and test of different standardization methods.

Best model: RandomForestClassifier(max_depth=20, min_samples_leaf=2, n_estimators=200, random_state=123), with MSE=0.1708, Accuracy=0.8292, F1=0.8682,	Recall=0.8941, AUC=0.8066.
