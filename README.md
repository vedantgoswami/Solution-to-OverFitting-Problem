#Solution to OverFitting-Problem
This repository shows how Dropout can help in eliminating overfitting Problem.
> Dropout in Deep Learning refers to dropping out or ignoring neurons during the training phase of certain set of neurons which is chosen at random.

## Dataset Used: 

<p align="center">
  <img src="https://github.com/vedantgoswami/OverFitting-Problem/blob/main/Images/dataset.png">
</p>

<p>
<b>The below graph shows how the plotted line is overfitting every data point due which there is high accuracy on training dataset but poor on the testing dataset.</b>
</p>

<p align="center">
  <img src="https://github.com/vedantgoswami/OverFitting-Problem/blob/main/Images/overfitting.png">
</p>
<p>
  <h3> What is the Problem ? </h3>
    Overfitting occurs when a model tries to predict a trend in data that is too noisy. This is the caused due to an overly complex model with too many parameters. A model that is overfitted is inaccurate because the trend does not reflect the reality present in the data. <b> This can be judged if the model produces good results on the seen data(training set) but performs poorly on the unseen data(test set) </b> .The goal of a machine learning model is to generalize well from the training data to any data from the problem domain. This is very important as we want our model to make predictions in the future on data that it has never seen before.
 </p>    
<h3> To Overcome this problem we use different Techniques such as: </h3>

- Simplyfing the model
- Early Stopping
- Use Data Augmentation
- Use Regularization( L1 or L2 )
- Dropouts

<p>
In this repository i am using the last one that is <b> Dropout </b>.
Dropout method randomly drops neurons from the neural network during training in each iteration. When we drop different sets of neurons, it’s equivalent to training different neural networks. The different networks will overfit in different ways, so the net effect of dropout will be to reduce overfitting.
</p>

<h3> The Below visualization shows how dropout works</h3>

<p align="center">
  <img src="https://github.com/vedantgoswami/OverFitting-Problem/blob/main/Images/GIF.gif">
</p>

<h3> I have also used the dropout and here is how my model performed </h3>
<p align="center">
  <img src="https://github.com/vedantgoswami/OverFitting-Problem/blob/main/Images/dropout.png">
</p>

Before Regularizing my model have an error on training and testing dataset as follows:
> Train: 0.004
> Test: 0.046

The model was having high accuracy on training but was performimg very poor on test dataset which was the sure shot case of Overfitting.<br>
After a Dropout on hidden layer there was an increase in accuracy of testing dataset:
> Train: 0.014
> Test: 0.037


  
