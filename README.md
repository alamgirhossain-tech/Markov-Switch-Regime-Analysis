# Markov Switch Regime Analysis
This Notebook is applied time series regime analysis in python. My aim is to demonstrate how to detect and predict regimes in time series, with the application tailored to financial time series.
Markov Switching Autoregression
A Markov Switching model is a popular regime-switching model that rests on the assumption that unobserved states are determined by an underlying stochastic process known as a Markov-chain. A Markov-chain is a system describing possible events in which the probability of each event depends only on the state attained in the previous event.

There are a variety of approaches to understanding time series regimes. The approach presented in this Notebook is the use of a Markov Switching Autoregressive model for regime detection and classification. Furthermore, machine learning is explored for providing an expectation of the next day’s regime.

The first section deals with the MS-AR implementation for regime detection and classification. The second section deals with the machine learning, Random Forest Classifier, implementation for the prediction of the next regime.

On the testing set (unseen data), our model has achieved a true positive rate of 99.05% meaning that over 99% of actual high variance regimes in the next period were correctly predicted as high variance regimes. The model presented with a 0.013% false positive rate, meaning that 0.013% of actual low variance regimes in the next period were incorrectly predicted as high variance regimes. To get a view of overall accuracy we can compute the area under the curve (AUC). Our model has an AUC of 99.05%, meaning that the model is able to distinguish between high and low variance regimes 99.05% of the time. Alternatively we can also use an accuracy score computation. All metrics would suggest a model with a high degree of accuracy and low prediction error, providing a satisfactory result for this use case.

![image](https://user-images.githubusercontent.com/84444284/198501057-334a9743-98e1-4894-80bc-437a188986b2.png)
