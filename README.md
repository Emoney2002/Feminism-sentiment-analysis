# Feminism-sentiment-analysis
YouTube Sentiment Analysis on Feminism
This project performs sentiment analysis on YouTube comments related to feminism using the YouTube Data API and the VADER sentiment analysis tool. The goal is to fetch a set of comments from a specified video and analyze the overall sentiment—whether positive, negative, or neutral.

Features

Fetches comments from a specified YouTube video using the YouTube Data API.

Filters out comments from the video uploader and handles emoji filtering.

Analyzes the sentiment of each comment using the VADER Sentiment Analysis tool.

Visualizes the sentiment distribution with plots.

Prerequisites

Python 3.x
Jupyter Notebook

The following Python libraries:
google-api-python-client
vaderSentiment
emoji
matplotlib
re

Setup
Get a YouTube Data API key
You need to create an API key to access the YouTube Data API. Follow the instructions on Google Developer Console to generate one.

Run the Notebook
Open the Jupyter notebook file and replace the placeholder API key with your own:


API_KEY = 'YOUR_API_KEY_HERE'
Input the YouTube Video URL
After setting up the API, input the URL of the YouTube video from which you want to fetch comments. The notebook automatically extracts the video ID and channel ID of the uploader.

Fetch and Filter Comments
The script fetches the comments in batches and excludes comments from the uploader. It also supports filtering comments that contain only emojis.

Sentiment Analysis
The comments are analyzed using the VADER sentiment analysis tool, which classifies each comment into positive, neutral, or negative sentiment categories.

Visualization
Finally, the results are visualized using matplotlib, showing the distribution of sentiment across the collected comments.

Example Output
The notebook prints the top 5 fetched comments and displays a plot that illustrates the sentiment analysis distribution.

Notes
The number of comments fetched can be adjusted in the code by modifying the limit in the while loop.
Ensure you handle API quotas and limits imposed by YouTube's API.
