# Starbuck customer behavior guide


1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>
For this project I have used the Starbucks reward mobile app data to offer patterns in customer behavior and to answer the following questions:
### Starbucks offers
1. What type of offers does Starbucks provide?
2. What is the minimum and maximum reward associated with an offer?
3. What is the average duration and difficulty for an offer depending on their characteristics?
4. Which channels are mainly prefered in promoting offers?

### Customers profile
6. What are the main demographic characterists for Starbucks typical customers?
7. What is the customer average income by offer type?
8. What type of events are prefered by customers taking into perspective the age, gender and income?

### Events
9. What are the proportions associated with each event type?
10. What is the average time needed to complete an offer?
11. How can we describe the Starbucks customer behaviour?
12. Can we predict the how much someone will spend based on customer characteristics and offer eligibility?
13. What are the main variables that influence the decision of a customer to respond to an offer?

## File Descriptions <a name="files"></a>
### Offers data: portfolio.json 
* id (string) - offer id
* offer_type (string) - type of offer (BOGO, discount, informational)
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings) - type of channel (email, mobile, social, web)

### Customers data : profile.json 
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

### Events data: transcript.json 
* event (str) - record description (transaction, offer received, offer viewed, offer completed)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Results<a name="results"></a>
The main findings of this study can be found in [here](https://medium.com/@claudiaandreea.toma/starbucks-customer-behavior-guide-1915f2dd1a17).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
I would like to give credit to Starbucks for the database used for this study and to Udacity for all the code techniques learning through the Data Science program. 
Feel free to use my code and maybe take a look at the blog post mentioned above. 
