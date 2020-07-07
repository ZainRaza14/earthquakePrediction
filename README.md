# earthquakePrediction

Earthquake Prediction 

1 Summary
I participated in an active competition of predicting earthquakes on Kaggle. The ﬁnal model I choose is RNN-LSTM stacked, a deep recurrent neural network architecture, which takes given features as inputs and outputs the time remaining before the next earthquake. I implemented RNN-LSTM stacked using Keras and ran the code on a cloud platforms i-e AWS-EC2-Instance and Google Cloud Instance. Amazon EC2 instance had a CPU 4 CPU’s and GPU of NVIDIA TeslaM60 with 30 GB memory and Google Cloud Instance had CPU 4 CPU’s and GPU of NVIDIA TeslaP100 with 15 GB memory. Performance is evaluated using mean absolute error. The competition is still active so in the public leaderboard, my score is 1.443; I rank 691 among the 4063 teams.

2 Problem Description
Problem. In Earth sciences, forecasting earthquakes is one the great challenges. Due to their destructive nature, earthquakes have always a big impact on our Earth. In this competition, the goal is to predict when the next earthquake will take place. This is a regression and time series prediction problem where we have to predict the time before the next laboratory earthquake happens. The competition is at https://www.kaggle.com/c/LANL-Earthquake-Prediction/overview.
Data. The data for this competition was generated using laboratory methods and setup. The data has one feature ”acoustic data” which are the seismic signals which will help us to predict earthquakes. The labels are ”time to failiure” which is the time remaining before the next earthquake. Training data is of 9GB size. The number of training samples is n = 629.1million. Test data has 2624 segments, each of which has seismic signals and we have to predict the ”time to failure” for each signal.
Challenges. One of the challenges for this project is the imbalance data. Only 13 times an earthquake happened in almost 630 million samples. Another interesting thing is that the training data is gathered using single continuous experiment. On the other hand, test data has diﬀerent segments, for each of which we don’t know whether they were captured within same and continuous experiment or maybe each segment was gathered in a diﬀerent set of experiments. The predictions can not be assumed to follow the same pattern as that of the training data.

