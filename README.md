# Music Recommendation
Music Recommendation Using Content Based Filtering

# Introduction

In this exercise, you will be building a content-based recommender system for digital music using the Amazon meta dataset. The goal is to recommend the top ten song titles to users who interact with your simple app. To achieve this, you will build a content-based filter that uses the songs’ features.

# Exercise Requirements

Load the dataset named “meta_Digital_Music.json.gz,” attached to this assignment into a dataframe, name it songs_firstname.
Data Exploration:
a. Carry out a thorough exploration and note the results into your analysis report. Make sure to check for empty data, not just null.
b. Also, in your analysis report, suggest which columns you will take into consideration for the recommender system and why. (There are 19 columns in total)
c. Based on the output of points a & b suggest any filtering steps, for example, if you need to drop any columns or filter out any rows and explain why. Write your explanation in the analysis report.
Feature Engineering:
a. Clean your data and prepare your feature space based on the results in point#2 above. You might combine columns, transform…etc. Make sure you follow all the recommendations you noted in your analysis report.
b. If your feature space has text data, which most likely is the case:
i. Pre-process the data and note the steps in your analysis report.
ii. Create TF-IDF vectors for the textual description (or overview) of every song
c. Compute the pairwise cosine similarity score of every song title.
d. Store the recommendations into a separate file that your simple app will access.
Recommender function: Write the recommender function that takes in a song title as an argument and outputs the top ten ‘song titles’ most similar to it.
a. Your app should receive a ‘song title’ as input from the user, for example, ‘Long Legends’, ‘There can be miracles’…etc. If the ‘song title’ is not available, then reply to the user “We don’t have recommendations for XXX” where XXX is the inputted song title. Then prompt the user to enter a different ‘song title’. (hint: use python input())
b. If the ‘song title’ is available, present the top-10 most similar song titles back to the user as a recommendation.
c. Continue accepting input from the user and responding until the user enters an “exit” text.
Name your python script “firstname_songs_recommender.py” and attach it to your submission. Make sure your script is callable from the command prompt without any errors.

# Conclusions
In conclusion, the content-based music recommender system based on the Amazon meta dataset for digital music provides a personalized music recommendation to users. The system uses the textual description of songs and computes pairwise cosine similarity scores of every song title to identify the top-10 most similar song titles.

During the data exploration phase, we discovered that some columns in the dataset were irrelevant to our recommender system, and there were empty values that required cleaning. We selected the relevant columns based on the insights gathered and used text pre-processing techniques to transform the textual data.

The feature space was created using a combination of columns, and we applied the Term Frequency-Inverse Document Frequency (TF-IDF) technique to generate vectors of the textual description for every song. Finally, the pairwise cosine similarity score was computed to identify the top-10 most similar song titles.

Overall, the music recommender app can help users discover new music that is similar to their preferred songs. The accuracy of the recommendations depends on the quality of the data and the relevance of the features selected. Therefore, there is a need for continuous monitoring and updates to improve the system's effectiveness.
