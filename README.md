# Binary Text Classification Task

## Introduction

Binary text classification is typically done using some form of supervised machine learning. As such, having labelled data is essential. In this data science task, we would like you to download the data provided and build a supervised classification model that can identify positive movie reviews within a large corpus of documents. This classifier should be capable of classifying positive movie reviews in a highly imbalanced population, where positive movie reviews might make up only 5%-10% of the population.

## Data description
You are provided with two data sets;

1. `review_data_with_labels.csv.gz`
   1. This data set is a gzipped csv file with two columns, `review` and `label`, with 241,999 rows.
   2. You will use this training data set to develop, train and test your classifier.
   3. The positive class, `label: 1`, contains only positive movie reviews
   4. The negative class, `label: 0`, contains negative movie and product movie

2. `runtime_test_without_labels.csv.gz`
   1. This data set is also a gzipped csv file with a single column, `review`, with 198,988 rows.
   2. You will use this data set as a simulated runtime scenario, where your classifier will be tested in recovering a known set of positives.


## Guidelines

1. You solution should be captured in a jupyter/google colab notebook (google colab notebook can be use for free with a google account)
2. You should aim to achieve a minimum positive class F1 score of ~0.8 based on a random test split of the labelled data
3. You are free to use any classification framework you think will be good at solving the problem
4. Algorithm selection is not part of the task, so unless you really want to, there is no expectation that you should compare different algorithms
5. You should demonstrate machine learning best practice during model development and testing
6. You should demonstrate NLP best practice according to your model architecture of choice
7. You should demonstrate model optimisation of some kind. This can follow simple heuristic-based hyperparameter selection through to full scale optimisation (grid search etc.).
8. You should aim to spend no more than 2 hours on the problem (excluding computation)
9. You should demonstrate threshold analysis and selection

## What you will provide as part of your solution

1. A summary of your solution and rationale for the methodology used (this can be a text cell in the notebook)
2. You should capture all of the steps you took to solve the problem in a reproducible notebook. Documenting your rationale with comments is good.
3. You should provide your final classification report at the optimal threshold on a random holdout test sample from the `review_data_with_labels.csv.gz`
4. Using your optimal threshold determined using your holdout test set, you should use your model to classify all reviews in the `runtime_test_without_labels.csv.gz` data set. Classification labels should be appended to the corresponding row of the dataframe, and the resulting dataframe written to csv
5. Please email your results back to `kevin.keenan@smarsh.com` from the email address provided during the application process.
