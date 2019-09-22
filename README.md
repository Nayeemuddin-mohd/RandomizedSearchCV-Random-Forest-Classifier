# RandomizedSearchCV-Random-Forest-Classifier


Randomized Search CV toSelect the best hyperparameter for any Classification Model

Grid Search CV vs Randomized Search CV

grid Search works good when you have a small number of hyperparameters,and when each hyperparameter has about the same magnitude of impact on validation score.

Randomized search is a better option when magnitudes of influence are imbalanced, which is more likely to happen as your number of parameters is growing

The most efficient way to find an optimal set of hyperparameters for a machine learning model is to use random search.

The randomized search meta-estimator is an algorithm that trains and evaluates a series of models by taking random draws from a predetermined set of hyperparameter distributions. 

The algorithm picks the most successful version of the model it’s seen after training N different versions of the model with different randomly selected hyperparameter combinations, leaving you with a model trained on a near-optimal set of hyperparameters.

Note that random search is called a meta-estimator because it’s not an estimator in itself, but rather an algorithm applied to an existing estimator in order to tune the estimator’s hyperparameters.

This method has an advantage over grid search in that the algorithm searches over distributions of parameter values rather than predetermined lists of candidate values for each hyperparameter. 

Being able to search over hyperparameter distributions also allows you to be more opinionated about what you expect a hyperparameter’s best value to be; if you want to draw values from a distribution that is normally, poisson, uniformly distributed, etc., you can specify it as such.

Random search is usually used in tandem with cross validation to achieve a more reliable estimate of what each candidate model’s out of sample performance will be.
