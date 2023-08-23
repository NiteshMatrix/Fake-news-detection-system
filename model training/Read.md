Fake News Detection
This repository contains code for scraping news articles from different sources, cleaning and processing the text data, training a machine learning model to detect fake news, and deploying the application using Flask and Heroku. The process involves collecting real and fake news articles, preprocessing the text data, training a model, and creating a web application for users to interact with.

Code Overview
The code is divided into several sections:

Scraping Data

The code uses BeautifulSoup and requests to scrape news articles from different sources, such as CNN, BBC, Breitbart, etc.
It collects both real and fake news articles, each labeled with a respective label.
Text Cleaning and Processing

Text data is cleaned by removing punctuation, converting to lowercase, tokenizing, removing small words, and removing stopwords.
Stemming and lemmatization are applied to further process the text.
TF-IDF Vectorization

The preprocessed text is converted into TF-IDF feature vectors, which represent the importance of words in each article.
Model Training and Evaluation

A Random Forest Classifier is trained on the TF-IDF vectors to detect fake news.
The model's accuracy and confusion matrix are displayed for evaluation.
Flask Web Application

The Flask framework is used to create a web application.
Users can input a news headline, and the trained model predicts whether it's fake or real.
Deployment with Heroku

The Flask web application is deployed on the Heroku platform, allowing users to access and use the fake news detection service online.