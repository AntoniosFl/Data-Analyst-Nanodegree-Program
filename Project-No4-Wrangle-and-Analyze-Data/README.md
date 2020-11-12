# Project Overview

In this project I was asked to wrangle (also analyze and visualize) the tweet archive of Twitter user @dog_rates, also known as WeRateDogs.

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has almost 9 million followers and has received international media coverage.

## Project Details
My tasks in this project were the following:

Data wrangling, which consists of:
- Gathering data 
  - Assessing data
  - Cleaning data
- Storing, analyzing, and visualizing the wrangled data
- Reporting on my data analyses and visualizations

<ins>**Gathering Data**</ins>

1. The WeRateDogs Twitter archive: This file was manually downloaded

2. The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) was downloaded programmatically using the **Requests** library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

3. Each tweet's retweet count and favorite ("like") count using the tweet IDs in the WeRateDogs Twitter archive. I queried the Twitter API for each tweet's JSON data using Python's **Tweepy** library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data was written to its own line. Then I red this .txt file line by line into a pandas DataFrame with tweet ID, retweet count, and favorite count.


<ins>**Assessing Data for this Project**</ins>

After I gathered each of the above pieces of data, I assessed them visually and programmatically for quality and tidiness issues. I detected and documented eight (8) quality issues and two (2) tidiness issues in the wrangle_act.ipynb Jupyter Notebook. 


<ins>**Cleaning Data for this Project**</ins>

I then cleaned each of the issues I documented while assessing in wrangle_act.ipynb as well.


<ins>**Storing, Analyzing, and Visualizing Data for this Project**</ins>

I stored the clean DataFrames in CSV files with the name twitter_archive_master.csv, image_predictions_clean.csv, and twitter-archive-enhanced.csv.
I then analyzed and visualized the wrangled data in the wrangle_act.ipynb Jupyter Notebook.

<ins>**Reporting for this Project**</ins>

I lastly created a written report called act_report.pdf that communicates the insights and displays the visualizatio produced from your wrangled data in an informal, lighter manner like a magazine article, for example.
