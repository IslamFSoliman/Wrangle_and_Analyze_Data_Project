# Wrangle and Analyze Data
## Udacity Data Analysis Professional Nano-Degree January 2021  - March 2021.

### Project 2: Wrangle and Analyze Data - WeRateDogs twitter account

[Click to preview report](https://github.com/IslamFSoliman/Wrangle_and_Analyze_Data_Project/blob/main/wrangle_report.pdf)

### Project Overview
#### Introduction
The dataset that I will be wrangling, analyzing, and visualizing is the tweet archive of Twitter user @dog_rates, also known as `WeRateDogs`. *WeRateDogs* is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 6 million followers and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

##### What Software Do I Need?
You need to be able to work in a Jupyter Notebook on your computer.

The following packages (libraries) need to be installed. You can install these packages via conda or pip. Please revisit our Anaconda tutorial earlier in the Nanodegree program for package installation instructions.

* pandas
* NumPy
* requests
* tweepy
* json
* You need to be able to create written documents that contain images and you need to be able to export these documents as PDF files.

### Project Specifications
#### Code Functionality and Readability
All project code is contained in a Jupyter Notebook named wrangle_act.ipynb and runs without errors.
The Jupyter Notebook has an intuitive, easy-to-follow logical structure. The code uses comments effectively and is interspersed with Jupyter Notebook Markdown cells. The steps of the data wrangling process (i.e. gather, assess, and clean) are clearly identified with comments or Markdown cells, as well.

#### Gathering Data
##### This is the initial step in which we collect the data for this project from three main sources:
1. Twitter_archive_enhanced.csv file, this file was downloaded manually and uploaded to the project workspace and finally imported to our working environment using Pandas function “pd.read_csv()” creating “archive_df”.
2. Image_predictions.tsv file, this is the second file that was hosted on a webpage and imported from its URL using Requests library function “get()” and Pandas function “read_csv()” creating “image_predictions_df”. (Note: This file contains image predictions for the rated dogs).
3. The final dataset was gathered from Twitter API via tweepy library, alternatively via the provided “tweet_json.txt” creating “api_df”.


#### Assessing Data
##### Two types of assessment are used:
Visual assessment: each piece of gathered data is displayed in the Jupyter Notebook for visual assessment purposes. Once displayed, data can additionally be assessed in an external application (e.g. Excel, text editor).
Programmatic assessment: pandas' functions and/or methods are used to assess the data.
At least eight (8) data quality issues and two (2) tidiness issues are detected, and include the issues to clean to satisfy the Project Motivation. Each issue is documented in one to a few sentences each.

#### Cleaning Data
##### This part of the data wrangling was divided in three parts:
Define, code and testing the code. These three steps were on each of the issues described in the data assessment section.\
First I’ve create a copy of the three original DataFrames. I wrote the codes to manipulate the copies. This allowed me to create a new copy from the original whenever needed in case of errors or mistakes, I could create another copy of the original DataFrames and continue working on the cleaning part.\
This stage has challenged me in many ways and made me feel more comfortable cleaning data programmatically on my own.


#### Report
##### Two reports:

Wwrangling efforts are briefly described in `wrangle_report.pdf`.\
The three (3) or more insights the student found are communicated in `act_report.pdf` including visualization.
