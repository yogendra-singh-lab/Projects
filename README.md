# Human-Activity-Recognition-Case-Study
This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying.

## Problem Statement:
Given a new datapoint we have to predict the Activity. 

### Type of Problem:
It is a Multiclass classification problem. The performance metric used is Accuracy.

## Solution implemented:
For this project I have tried predicting the activity type in two ways. In the first part I have taken the 561 expert engineered features and implemented classical machine learning models on top of them. In the other part I took the raw gyroscope and BodyAcceleration reading and implemented Deep learning models on it to try to get similar results to the classical machine learning models with the expert engineered features.

## About the Dataset:
This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.

#### Quick overview of the dataset :
Accelerometer and Gyroscope readings are taken from 30 volunteers(referred as subjects) while performing the following 6 Activities.

1. Walking
2. WalkingUpstairs
3. WalkingDownstairs
4. Standing
5. Sitting
6. Lying.

- Readings are divided into a window of 2.56 seconds with 50% overlapping.
- Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y and z components each.
- Gyroscope readings are the measure of angular velocities which has x,y and z components.

- Jerk signals are calculated for BodyAcceleration readings.

- Fourier Transforms are made on the above time readings to obtain frequency readings.

- Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.

- We get a feature vector of 561 features and these features are given in the dataset.

- Each window of readings is a datapoint of 561 features.
