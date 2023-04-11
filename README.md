# Insight-Project---AutoBroker
Data analysis and prediction model related to my Insight Project - AutoBroker

Thank you for your interest.

This directory contains the files with the analysis for predicting the total claims amount from an insurance dataset "train.csv". The resulting regularized linear regression model is used to build the final prediction model for my Insight Data Science project called AutoBroker (http://autobroker.site).

The full model contains proprietary information from my project consulting partner so it is not shared publicly. 

Please feel free to contact me for more information.

*Edit 2023-04: For cost reasons, this webapp is no longer running. Please see the screen shots below for an example of how to interact with the app:*

The app was hosted on an AWS EC2 instance using Flask/Gunicorn behind an NGINX reverse proxy.

The app presents the user (presumably an insurance agent) with a form to enter information about a potential client.
<img width="514" alt="image" src="https://user-images.githubusercontent.com/40176380/231019382-3e771241-faa4-4738-bba7-1e4f33c7cabb.png">

The user populates the form with relevant information and clicks `Calculate Rating` to submit the information.
<img width="514" alt="image" src="https://user-images.githubusercontent.com/40176380/231019580-5d5858e9-9fd3-4c51-9f4d-a6056c99b2db.png">

Using the information, a python scripts uses the pretrained regularized linear regression model to calculate a predicted rating for a user.
<img width="521" alt="image" src="https://user-images.githubusercontent.com/40176380/231019630-0806a6fc-9a96-4632-8051-72f00aa23c5e.png">

The predicted rating is meant to help provide and initial evaluatuation incoming applications.

**Note about Fairness: The intent of this app was to be a portfolio project during my time as a fellow at Insight Data Science. The project used a publically available insurance dataset. I later realized that some of the features may introduce inherent biases. I fully acknowledge that for real world usage, the model would need to be reevaluated to ensure fairness and eliminate biases.
