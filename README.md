# Starbucks-Capstone-Project
This is a capstone project for the course completed in response to Udacity- Data Scientist Nanodegree Program.   
Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.
Not all users receive the same offer, and that is the challenge to solve with this data set.   
Main task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.
You can find the blog post link here [MEDIUM-BLOG](https://medium.com/@xpressprat/evaluating-starbucks-promotional-offers-capstone-challenge-31f7ced7ac19)
## Table Of Contents  
* [Motivation](#moti)  
* [Summary](#summary)  
* [File Description](#desc)  
* [Prerequisites](#prerequisite)
* [Acknowledgement](#acknow)  
* [Running the Application](#running)  


<a name="moti"></a>
## Motivation
The motivation behind this project was exploring the Starbuck’s Dataset which simulates how people make purchasing decisions and how those decisions are influenced by promotional offers.   
It was driven by 4 main questions that were answered as the project came to its completion:
* What is the proportion of client who have completed the offers based on Gender?
* What is the proportion of client who have completed the offers based on their Age?
* What is the proportion of client who have completed the offers based on their Income Level?
* What are the most important features that help drive the offers in customers?

<a name="summary"></a>
## Summary 
The project was completed in the following phases:
* Dataset Exploration and Preprocessing:- In this process, the data provided was cleaned, processed and merged for further analysis.
* Data Analysis &  Visualization: In this process, few questions were answered by analysing the question and  providing visualization which answers the questions 1-3:     
##### In order to compute the proportion of male or female within the age range of 29 to 69 with income ranging from 30k to 100k who have commpleted the offer, we need their respective data and the total number of participants in the test.   
* Creation of supervised Model and Performance Evaluation: In this step, various machine learning model(Decision Tree, Gaussian NB and Random Forest) were tested on the given dataset and their respective performances were evaluated. 
* Important Feature Analysis: In this process, the best estimator among the three was used to predict the most important feature that impacted the promotional offer completion in customers.   
##### We found out that Time, Duration , Reward, Difficulty and Discount are the top 5 feature drivers that estimate the offer completion with Time being the highest impact driver for features


<a name="desc"></a>
## File Descriptions
#### Data Dictionary
##### profile.json
Rewards program users (17000 users x 5 fields)

gender: (categorical) M, F, O, or null   
age: (numeric) missing value encoded as 118   
id: (string/hash)   
became_member_on: (date) format YYYYMMDD   
income: (numeric)      

##### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)

reward: (numeric) money awarded for the amount spent   
channels: (list) web, email, mobile, social   
difficulty: (numeric) money required to be spent to receive reward   
duration: (numeric) time for offer to be open, in days   
offer_type: (string) bogo, discount, informational   
id: (string/hash)     
 
##### transcript.json
Event log (306648 events x 4 fields)

person: (string/hash)   
event: (string) offer received, offer viewed, transaction, offer completed   
value: (dictionary) different values depending on event type   
offer id: (string/hash) not associated with any "transaction"   
amount: (numeric) money spent in "transaction"   
reward: (numeric) money gained from "offer completed"   
time: (numeric) hours after start of test   

<a name="prerequisite"/></a>
## Prerequisites
* Python
* VsCode
* Jupyter Notebook
* Pandas
* Numpy
* Matplotlib
* Anaconda
* Seaborn
* Json
* Sklearn model selections
* ProgressBar
* Sklearn.metrics 
* Matplotlib patches
* os
* sys
* Sklearn tree, Naive bayes, ensemble
* itertools


<a name="acknow"/></a>
## Acknowledgement
I would like to thank Udacity for this amazing project, and Starbucks  for providing the data.

<a name="running"/></a>
## Running the Application
In order to run the project, you can find the ipynb notebook file in the project directory which you can run directly, Make sure to keep the data set in the data folders, if the data location is changed, make sure to reflect the changes in the import section of the notebook file with necessary adjustments.   
In addition to this, you can also find the .html file in the project directory to take a quick glimpse of the project too.


