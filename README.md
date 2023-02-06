# Lab1 - Scikit-learn

## Goal

The goal of this lab is to become familiar with the scikit-learn library.

You will practice loading example datasets, perform classification and regression with linear scikit-learn models, and infestigate the effects of reducing the number of features (columns in X) and the number of samples (rows in X and y).

## What to do

Follow `lab1.ipynb`. Here is an overview.

### Datasets
yellowbrick spam - classification  
https://www.scikit-yb.org/en/latest/api/datasets/spam.html

yellowbrick energy - regression  
https://www.scikit-yb.org/en/latest/api/datasets/energy.html

You will use the yellowbrick functions `load_spam()` and `load_energy()` to load the data.

### Models
Classification: sklearn LogisticRegression

`from sklearn.linear_models import LogisticRegression` 

https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html


Regression: sklearn LinearRegression 

`from sklearn.linear_models import LinearRegression`

https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html


### Steps

For each dataset and the corresponding model we will loosly follow five step process in _Python Data Science Handbook_ Chapter 5. More specifically, you will:

1. Load and prepare the data: Using yellowbrick functions and sklearn `train_test_split()`
1. Import the model from sklearn
1. Instantiate model
1. Compare training and validation metrics (accuracy for classification, MSE for regression) between:
    - Using all data
    - Using only 2 features and all samples
    - Using all features and only 1% of the samples

### Specifications
To implement the above steps, you will write the following functions: 
- `get_classifier_accuracy()`
- `get_regressor_mse()`

Function headers and documentation are included in `lab1.ipynb`. Implement the function body accordingly.

Use these functions to implement the tasks as directed and answer the questions below in the corresponding sections in the notebook.

### Questions
1. What is the validation score using all data? What is the difference between training and validation score?
1. How does the validation score and difference between training and validation change when only two columns are used? Provide values.
1. How does the validation score and difference between training and validation change when only 1% of the rows are used? Provide values.

## What to hand in
- In the Jupyter notebook `lab1.ipynb` implement the steps above as indicated. 
- Keep code clean and remove any unnecessary cells. 
- Use the results obtained to summarize your findings in *4. Observations/Interpretation*. 
- In a section *5. Reflection*, include a sentence or two about what you liked/disliked, found interesting/confusing/challangeing/motivating while working on this assignment.

During development, check-in progress with git and use descriptive commit messages.
