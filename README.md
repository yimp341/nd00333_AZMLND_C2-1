# Operationalizing Machine Learning

## Overview
This is the second project of the Machine Learning Engineer with Microsoft Azure Nanodegree Program. In this project, we have to deploy an AutoML model, consume the model endpoints and finally create and publish a pipeline.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Archdiagram.PNG?raw=true)

## How could the project be imporved
I think the weakness of the project is in the deployment. The user needs to run files on the terminal, namely the endpoint.py file in order to interact with the model. This is not the most userfriendly proces it could be. Maybe a tool could be created for this, such as a web app for the user to feed with the data and get nswers and insights about it.

## The key steps of the project
First we make sure that the dataset is registered in the Azure ML studio:
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Bankmarketing%20dataset.PNG?raw=true)

We run an AutoML experiment for the previous dataset. The target column is called "y".
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Experiment%20completed.PNG?raw=true)




