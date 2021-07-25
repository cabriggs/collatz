## Files included

- collatz.ipynb: a Jupyter notebook containing the analysis and narrative.
- collatz-notebook.pdfl: a pdf of the notebook
- collatz-report.pdf: a comprehensive report of the study

## Background

The Collatz length of a positive integer _n_ is the number of the following operations it takes to arrive at the number 1: if _n_ is even, divide by 2; else, triple and add 1. The Collatz conjecture says that every positive integer has finite Collatz length.

## Problem statement

Can machine learning models be used to predict the Collatz length of integers? Which models are successful, and why?

## What data

The first 10,000 positive integers and their Collatz lengths.

## What methods

Six model types were fit to the data: logistic regression, linear discriminant analysis, K-neighbors classifier, decision tree classifier, Gaussian naive-Bayes, and support vector machine. Their prediction accuracies on the training and test data were computed and compared. The best-performing models were analyzed.

### Technology

The analysis was performed in a Jupyter notebook, leveraging the sklearn library for machine learning.

## What conclusions

The models which performed best on the test data nevertheless failed to generalize above the test set.

Machine learning models are not interchangeable. The differences go beyond the linear and nonlinear. It is possible to find data sets on which some models perform very well, while others perform poorly. 

This study underscores a need when analyzing a data set which is often overlooked: it is sometimes insufficient to break a data set into training and testing chunks, then train on the one and test on the other. Sometimes it is necessary to acquire new data and test the model against the new data. This is especially true, for example, with time series data. The data analyzed here is not a time series, but analogies can be drawn between this data and time series.

## What questions remain

It would be an interesting exercise to find the theoretical maximum differences in performance of different models on a given data set.

It remains to attempt accurate predictions beyond the highest integer used in the training set.
