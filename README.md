# Wrangle-and-Analyze-WeRateDogs-Twitter-Data

 Real-world data rarely comes clean. Using Python and its libraries, you will gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. 

### Dataset
The dataset used for this wrangling (and analyzing and visualizing) project is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

### Assessing Data
The download data were all loaded into dataframe using pandas and were assessed for quality and tidiness through visual and programmatic method. A number of Quality issues and tidiness issue.

### Summary of Findings
#### Quality issues
1.Rating_denominator column in the twitter_archive table had values that were less than 10 and greater than 10
2.Timestamp column in twitter_archive_ table was not in a date time format.
3.Some dog names in the twitter_archive table were in lowercase.
4.Missing values in ‘name’ and dog stages of twitter_archive table represented as ‘None’
5.Tweets beyond August 1st, 2017 in tweets_archive table were not needed.
6.Only original tweets were required (retweets and replies not needed)
7.id_str column in tweets table table needed to be renamed tweet_id to allow for merging with other tables
8.tweet_id columns in twitter_archive and image_prediction table were of the wrong data type.
9.Some Columns in the twitter_archive, tweets, are not relevant. also columns with much missing values.
#### Tidiness issues
1. Data in three separate Tables instead of one
2. Dog stage in twitter Archive data in four separate columns

#### Cleaning Data
all of the quality and tidiness issues that were documented above while assessing the data were cleaned and the cleaned data stored
