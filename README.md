# Cross-Validation
Invistico Airline dataset  handled by cross validation 
this is larg dataset cleand and visulaised .
I got 92% acc with cross validation using (SVC) model .


The cross_validate function differs from cross_val_score in two ways:

It allows specifying multiple metrics for evaluation.

It returns a dict containing fit-times, score-times (and optionally training scores, fitted estimators, train-test split indices) in addition to the test score.

For single metric evaluation, where the scoring parameter is a string, callable or None, the keys will be - ['test_score', 'fit_time', 'score_time']

And for multiple metric evaluation, the return value is a dict with the following keys - ['test_<scorer1_name>', 'test_<scorer2_name>', 'test_<scorer...>', 'fit_time', 'score_time']

return_train_score is set to False by default to save computation time. To evaluate the scores on the training set as well you need to set it to True. You may also retain the estimator fitted on each training set by setting return_estimator=True. Similarly, you may set return_indices=True to retain the training and testing indices used to split the dataset into train and test sets for each cv split.

The multiple metrics can be specified either as a list, tuple or set of predefined scorer names:
