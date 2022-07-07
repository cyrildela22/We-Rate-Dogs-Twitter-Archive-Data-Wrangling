# We-Rate-Dogs-Twitter-Archive-Data-Wrangling
## Introduction
This project was a partial fulfilment of the Udacity Data Analyst Nanodegree program and its primary objective focused on wrangling data from the WeRateDogs Twitter account via Python which is documented in a Jupyter Notebook (wrangle_act.ipynb). WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators sometimes are greater than 10. 11/10, 12/10, 13/10, etc because some owners think they are good dogs. WeRateDogs has over 4 million followers and has received international media coverage.

## Installation
Installation of the following packages via conda or pip.
- pandas
- NumPy
- requests
- tweepy
- json



## Project Details /Overview

Considering this project, we only wanted original ratings (no retweets) that have images. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.
Entirely assessing and cleaning the dataset completely would require a lot of time. Therefore, the requirements of this project are only to assess and clean at least 8 quality issues and at least 2 tidiness issues in this dataset.


Data wrangling steps consisted of:
- Gathering data
   - Gather data from file on hand
   - Download file using Requests library and URL
   - Gather data from twitter API using Python's Tweepy library and store data
- Assessing data
- Cleaning data
- Storing data
- Analyzing and visualizing wrangled data
- Reporting 
   - wrangled effort (wrangle_report.pdf) 
   - data analyses and visualizations (act_report.pdf)

## The Data
In this project, I worked on the following three datasets.
- #### The twitter archive (WeRateDogs)
 This archive.csv file was manually downloaded from the WeRateDogs Twitter Archive. The downloaded dataset which consist 2356 tweets was read using pandas command for reading `.csv` files.
 
- #### The tweet image predictions
The image prediction file was programmatically downloaded by using the Requests library(`requests.get`) to retrieve the tweet image prediction (image_predictions.tsv) from the URL provided by Udacity.
 The retrieved data was saved and created a dataframe for the saved data.
 
- #### Each tweet's retweet count and favorite ("like") count
My twitter developer account application was not approved so I downloaded the file (`tweet_json`) which contains the JSON data for each tweet and read it line by line into a pandas DataFrame to extract the needed features ie (retweet and like counts).

## Resources
- Files downloaded from Udacity
