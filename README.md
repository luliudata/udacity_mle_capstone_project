# Starbucks Capstone Project
This is my Starbucks Capstone Project as part of the Udacity Machine Learning Engineer Nanodegree. 
Udacity partnered with Starbucks to provide a real-world business problem and simulated data mimicking their customer behavior.

# Overview
Starbucks Corporation is an American coffeehouses company and it is one of the world`s largest coffeehouse chain. 
Once every few days, Starbucks sends out an offer to users of the Starbucks rewards mobile app. 
The offers contain three types: an advertisement for a drink, an actual offer such as a discount and BOGO (buy one get one free). 
Some users might not receive any offer during certain weeks.
Starbucks wants to utilise technology to provide their customers a better personalised experience and boost their marketing performance. 
To be specific, they want to target the right customers who are most likely to make a purchase and also know about customers who might not want an offer.

The motivations of this project is to gain more machine learning hands-on practice and have a better understanding about how the technology can make an impact on the real business.

# Data Sets

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

# Python Libraries Used
* pandas==1.0.5
* numpy==1.16.4
* json==2.0.9
* progressbar==3.37.1
* sklearn==0.23.1
* tensorflow==1.14.0
* keras==2.3.1
* seaborn==0.10.1
* matplotlib==3.2.2
* shap==0.35.0
