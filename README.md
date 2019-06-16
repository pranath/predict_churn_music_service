# Predicting churn for the Sparkify music service

## Project overview
Many online services these days provide flexible services to customers which are easy to subscribe to and unsubscribe from. Good examples of such services in the music industry include those such as Spotify and Pandora.

A common problem with these services is trying to anticipate customers who plan to cancel (also known as customer 'churn') with the idea of perhaps encouraging them to stay by providing a special offer, or other incentives. By minimizing customer churn, these services can aim keep more customers happy, and ensure their businesses are more profitable.

For this project, we have a dataset from a music service called Sparkify, very similar to Spotify and Pandora.

## Project definition
Streaming music services can produce huge datasets, and we will approach this project by using one of the most caperble tools for dealing with big data - Apache Spark.

In this project, we will analyse the dataset for user logs from the Sparkify service and seek to build a machine learning model that is able to predict customers that might churn.

## Results

Our most promising model was the Random Forrest classifier, which had a final validation score of 0.79. It should also be noted that a subsequent evaluation on a separate test set never seen produced a lower score of 0.62. This throws some caution on validation score of 0.79, however the smallness of the dataset as a whole and in particular this separate test set should also be noted.

It was certainly very useful to have a separate test set of data to question the validity of the performance of our model - even if we cannot be entirely certain of how much confidence we should place on this.

Nevertheless, this model and features developed seem to be good candidates for further exploration on bigger datasets, which would also yeild more conclusive results on our approach. It is my belief that on a bigger dataset, the disparity between the validation and test score would be much smaller, giving us more confidence in the performance of the model on an ongoing basis for larger datasets and more users for predicting churn more accurately.

## Libraries used

- pyspark
- scipy
- datetime
- numpy
- pandas
- seaborn
- matplotlib
- time

## Project files

- sparkify_small.ipynb : Jupyter notebook for developing the analysis and models for the project
