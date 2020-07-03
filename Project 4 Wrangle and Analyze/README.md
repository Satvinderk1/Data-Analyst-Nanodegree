# Project 4: Wrangle and Analyze Data

## Title:

Wrangle and analyze [**WeRateDogs**](https://en.wikipedia.org/wiki/WeRateDogs) Twitter data

## Introduction:

Wrangle, analyze and visualize the tweet archive of Twitter user [`@dog_rates`](https://twitter.com/dog_rates),
also known as [**WeRateDogs**](https://en.wikipedia.org/wiki/WeRateDogs) to create
interesting and trustworthy analyses and visualizations.

## Overview:

Real-world data is often dirty and messy. It rarely comes clean.  The whole process of making this dirty and messy data usable for making quality analysis, producing descriptive visualizations and building predictive models is called Data Wrangling. It is done in three different steps gathering the required data, assessing it to identify the quality and structural issues in it and cleaning data.

In this project, I am using Python and its libraries to gather data from a variety of sources and in a variety of formats, assess it for its quality and tidiness, then finally clean it. I will also be documenting the wrangling efforts in a Jupyter Notebook and showcasing them through analysis and visualizations.

## Data:

The dataset that is used in this project for wrangling, analyzing and visualizing is the tweet archive of Twitter user @dog_rates , also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10 and the numerators almost always greater than 10 (Ex: 11/10, 12/10, 13/10, etc.) because they are good dogs. WeRateDogs has over 8 million followers and has received international media coverage.

The required data for this project is stored in different places:

- Enhanced Twitter Archive (given in csv file)
- Image Predictions File (Stored on Udacity webpage)
- Additional Data via the Twitter API (Query from Twitter API)

## Install:

I have used following python libraries:

- pandas
- NumPy
- requests
- tweepy
- json
- matplotlib
- seaborn

## Project Goals:

- Use only original ratings (no retweets) that have images. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.
- Assessing and cleaning the entire dataset completely would require a lot of time, and is not necessary to practice and demonstrate skills in data wrangling. Therefore, the requirements of this project are only to assess and clean at least 8 quality issues and at least 2 tidiness issues in this dataset.
- Cleaning includes merging individual pieces of data according to the rules of tidy data.
- The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs.
- No need to gather the tweets beyond August 1st, 2017. As the image predictions for these tweets won't be available.

## Project Tasks:

- Data wrangling, which consists of:
    1. Gathering data
    2. Assessing data
    3. Cleaning data
- Storing, analyzing, and visualizing the wrangled data
- Reporting on 1) data wrangling efforts and 2) data analyses and visualizations
