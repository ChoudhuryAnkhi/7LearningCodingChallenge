# 7Learnings Data Scientist Code Challenges


## Table of contents
* [7LCodingChallenge.ipynb](# ipynbfile)
* [readme.md](#Readme file)
* [requirements.txt](#to load dependancies)


## Description of the problem "Will it snow tomorrow?" - The time traveler asked

Problem: 
* To detect if it would snow 11 years ago from today. So if today is 2021.5.5 we would like to know if it snowed on the date Wednesday, 2010.5.5 or not.
* A public dataset `bigquery-public-data.samples.gsod` has been provided which has climate information from over 9000 stations accross the world.
* The challenge is divided in two parts with subparts to answer the aforsaid question.

Solution:
* Using data exploratory analysis to get an idea on the data
* Further, feature engineering to see which parameters affect the colunm `snow`
* Computing Machine Learning algorithms to create a model that would predict the given category.

Reasoning:
* **LR(Logistic Regression)** was chosen as a classification algorithm for an initial test. The value of the target is categorical in nature, given the binary output this could be a good start.
* **DT(Decision Tree)** to imporve the recall which was not captured well
* **RF(Random Forest)** to improve further results on the DT

Trade Offs:
* LR could not capture the data as well, columns like `fog`,`rain`,`snow`,`thunder` exhibit very high correlation suggesting that there are values which are mostly similar.
* RF and DT performed better in comparison to LR

Setup

* to download and install requirements.txt
* establishing a connection with GCP

