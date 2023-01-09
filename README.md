# Customer service problem classification.

![twitter](https://user-images.githubusercontent.com/109353419/211259124-6e9a63d5-ad5e-46a3-9911-5f9b0d00bdc7.jpeg)


#### Authors:
Antony Brian, Arnold Kalage, Betty Bett, Faith Makokha, Julia Karanja

#### Table of Contents
* Business Understanding 
* Data Understanding
* Data Preparation
* Modeling
* Evaluation

## Business Understanding.

#### Overview
-The advancement of technology has enhanced communication abilities with the use of social media in business and other sectors. Better communication increased the ability of most companies to get in touch with their consumers through an easier and faster medium.  Client care is, therefore, at the core of all successful businesses because developing customer interactions is one of the keys to increasing customer loyalty.  Most companies receive customer service complaints and requests via Twitter, especially Kenya Power and Safaricom, where the requests can be instantaneous and frequent. Some of these complaints require classification to be forwarded to the right customer service department or a person who specializes or deals with the problem directly.


-Safaricom PLC is a leading telecommunications company in Kenya, serving millions of customers across the country. Founded in 1997, the company has become a household name in Kenya, providing various services, including mobile voice and data services, financial services, and enterprise solutions.The company operates a network of over 18,000 mobile towers across Kenya, providing coverage to over 99% of the country’s population. Safaricom offers a range of mobile plans to suit different needs and budgets, including prepaid and postpaid options.From the products and services Safaricom offers, the company has a large user base, creating the challenge of managing all its consumers. Due to the large customer base, some consumers might feel unsatisfied with the customer service offered by Safaricom, especially on social media. The Safaricom_care Twitter handle depicts the number of people complaining about different services at a given time. 

-Handling these complaints can be challenging, especially since numerous people can tweet about different services at a given time. Customer care remains one of the most important elements of a successful business since it maintains the relationship between the company and its consumers.

#### Business Problem.
In recent years, several companies have migrated to using social media for customer service and customer support, with companies having specific accounts dedicated to customer care queries. This has led to the problem of classifying said complaints or services according to the department that needs to work on them and generate tickets for the services. Numerous customers can tweet about different services simultaneously, making it easy for the company’s staff to miss such complaints. This might be unsatisfactory to the affected consumers, leading to the loss of business. This data comes at a high frequency, so a machine learning model is the easiest way to handle such data and accelerate response rates. This model will classify all tweets directed to the company’s customer care handle and classify and direct them to the relevant departments. This will help manage the traffic of complaints made to the customer care handle and increase the speed of responses to the consumers since each department will be responsible for the complaints of their products and services.

## Data Understanding
#### Overview.
The data used in this project is from the Safaricom_Care twitter handle. The data contained 1,000,000 records representing any comment made on the Safaricom_Care handle, including the replies made by Safaricom_Care.

#### Data description.
The dataset contains 1,000,000 rows and 5 columns.
The description of the columns are as follows:
* Datetime - This refers to the date of the tweet
* Tweet Id - This refers to the unique id of the tweet
* Text - This refers to the actual text in the tweet
* Username - This refers to the name of the user who commented
* Like Count -This refers to the number of likes a tweet receives

## Data Preparation.

We performed the following tasks:
Data Cleaning, which included:
* Removing Tweets by Safaricom in order to have tweets from their customers only
* Converting all the tweets to lowercase, removing: links, usernames, hashtags, punctuations, emojis, stopwords, and numbers, to eliminate the noise in our data.
* Creating labels for our data by placing common words in categories.



## Modeling.
This is an NLP project that aims to build a model that accurately classifies text into one of the several categories. We will compare several different models to find the one that performs the best in our dataset. These models include:
* KNN
* Decision Trees
* Random Forest
* SVM
* Decision Trees with Grid Search CV
* Neural Networks
* XG Boost


## Conclusion.
-The inception of social media has enhanced communication, and with it, businesses have an easier time connecting with their customers worldwide. Social media accounts have become an essential part of any business and contribute heavily to the success of the business. Safaricom has done an amazing job creating and using social media for the success of its business. The company has adopted social media marketing and efficient customer service on social media to reach its numerous customers.
-Millions of people use social media every day, which poses a unique challenge amidst numerous opportunities. A company must have vast resources to allocate to social media management to effectively handle all the complaints and comments sent at a given period. In this case, Safaricom receives thousands of comments at any given time due to its wide pool of consumers. It can be very challenging to evaluate all these tweets, classify them to the respective departments, and discard the irrelevant ones. Furthermore, consumers complain about serious issues on social media accounts, which might need immediate responses from Safaricom to satisfy the consumers
-To alleviate this challenge, we scrapped data from Twitter to use in training and testing our models, and we wanted to draw some insights using EDA. We noted that most tweets are sent in the morning despite the categories. We also discovered that M-Pesa has numerous complaints distributed throughout the day. Consumers face numerous challenges with M-Pesa services and products, and the company needs to allocate adequate resources to manage this challenge.
-After understanding the challenge and the data, we devised a model that classifies the comments and directs them to their respective departments. Using scraped data from Safaricom Care’s Twitter account, we trained and tested three models, i.e., Decision Tree, KNN, and an XG Boost model, to find the best model from their accuracies. From these models, the XGB model performed the best, with an average accuracy of 94%. Therefore, our deployment was based on the XGB model, which will classify tweets by department. The deployment page is easily accessible for the company, and it can review the comments sent to Safaricom’s Twitter account and classify them according to their departments.


## Recommendations.
-We recommend that Safaricom focuses more resources on the M-Pesa department since numerous customers complain about M-Pesa services daily. The company should investigate the services provided by M-Pesa and where the problem lies. Furthermore, M-Pesa handles people’s money, which can be a sensitive issue when customers complain. The increased resources focused on M-Pesa will reduce the response time of these complaints since the increased number of staff can comfortably handle all the complaints.
-We recommend that more staff members be available in the morning since we saw that more tweets are sent in the morning than in the afternoon and the evening. Due to this, mornings seem like the busiest time of the day regarding receiving and dealing with customer complaints.
-The general category can be used for the company’s general improvement since it contains customer comments on general matters on the company and its business. The comments can be used to address issues like sponsorship and other sectors that enhance the company’s image.

