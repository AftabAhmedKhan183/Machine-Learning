# GridSearchCV and RandomizedSearchCV

This project demonstrates **hyperparameter tuning** using `GridSearchCV` and `RandomizedSearchCV` on the **Iris dataset**. It compares parameter combinations for **K-Nearest Neighbors (KNN)** and **Support Vector Classifier (SVC)** models.

## Dataset

The project uses the Iris dataset available through Seaborn:

* 150 samples
* 4 numerical features:

  * Sepal Length
  * Sepal Width
  * Petal Length
  * Petal Width
* Target: `species`

## Models Used

### K-Nearest Neighbors (KNN)

The notebook uses KNN with different values of `n_neighbors`:

`[3, 5, 7, 9]`

### Support Vector Classifier (SVC)

The notebook explores different combinations of:

* `C`: `[1, 10, 20, 30, 40]`
* `kernel`: `['rbf', 'linear']`
* `gamma`: `['auto', 'scale']`

## Hyperparameter Tuning

### GridSearchCV

`GridSearchCV` evaluates the specified parameter combinations using **5-fold cross-validation**.

It is applied to both:

* SVC
* KNN

The notebook examines `cv_results_` and compares the mean test scores for the different parameter combinations.

### RandomizedSearchCV

`RandomizedSearchCV` samples a fixed number of parameter combinations instead of evaluating every possible combination.

The notebook uses:

* `n_iter=4`
* `cv=5`

It is applied to both:

* SVC
* KNN

## Workflow

1. Load the Iris dataset.
2. Inspect the dataset and target classes.
3. Split the data into training and testing sets.
4. Train a KNN model.
5. Train an SVC model.
6. Experiment with different hyperparameters.
7. Use `GridSearchCV` for systematic hyperparameter tuning.
8. Use `RandomizedSearchCV` for randomized hyperparameter tuning.
9. Analyze cross-validation results using Pandas.

## Libraries Used

* Python
* NumPy
* Pandas
* Seaborn
* Matplotlib
* Scikit-learn

## Learning Outcomes

* Understand the purpose of hyperparameter tuning.
* Learn how `GridSearchCV` searches through parameter combinations.
* Understand the difference between `GridSearchCV` and `RandomizedSearchCV`.
* Use cross-validation to compare model configurations.
* Analyze hyperparameter search results using Pandas.
  ::: 
