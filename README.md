# Operationalizing Machine Learning

## Overview
This is the second project of the Machine Learning Engineer with Microsoft Azure Nanodegree Program. In this project, we have to deploy an AutoML model, consume the model endpoints and finally create and publish a pipeline.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Archdiagram.PNG?raw=true)

## How could the project be imporved
I think the weakness of the project is in the deployment. The user needs to run files on the terminal, namely the endpoint.py file in order to interact with the model. This is not the most userfriendly proces it could be. Maybe a tool could be created for this, such as a web app for the user to feed with the data and get nswers and insights about it.

## The key steps for AutoML experiment and deployment
First we make sure that the dataset is registered in the Azure ML studio.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Bankmarketing%20dataset.PNG?raw=true)

We run an AutoML experiment for the previous dataset. The target column is called "y".

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Experiment%20completed.PNG?raw=true)

For the deployment, we need to enable applications insights.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Applications%20insights%20enabled.PNG?raw=true)

We enable logging by runing the logs.py file in the swagger folder.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Logs1.PNG?raw=true)

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Logs2.PNG?raw=true)

We run Swagger in localhost port 900 in order to get the HTTP API information

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Swagger.PNG?raw=true)
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Swagger2.PNG?raw=true)
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Swagger3.PNG?raw=true)
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Swagger4.PNG?raw=true)

Then, we run the endpoint.py file and get the following JSON output.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Endpoint.PNG?raw=true)

## Pipeline creation and publication
First, we create a pipeline for the AutoML experiment, with the help of the Jupyter notebook.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Pipeline%20Section.PNG?raw=true)

The created pipeline looks like this:

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Pipeline.PNG?raw=true)

After publishing the Pipeline we can see the rest endpoint in the overview

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Published%20Pipeline%20Overview.PNG?raw=true)

Here is the output for Rundetails in the Jupyter notebook:
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Run%20details.PNG?raw=true)

We get some active Endpoints for the Pipeline deployment
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Pipeline%20Endpoint%201.PNG?raw=true)
![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Pipeline%20Endpoint%202.PNG?raw=true)

And finally we show both runs of the pipeline.

![alt text](https://github.com/yimp341/nd00333_AZMLND_C2-1/blob/master/Scheduled%20run.PNG?raw=true)

## Screencast
https://drive.google.com/file/d/18ZPQI7ztnFpgxf2mwwWWb4wVUkRz-Bxz/view



