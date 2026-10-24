# YouTube Food Review Sentiment Analysis

## Project Overview

This project performs sentiment analysis on YouTube comments
collected from food review videos. It uses Natural Language
Processing (NLP) to identify whether people's opinions about
food and restaurants are positive, negative, or neutral.

The main objective is to collect up to 2,000 YouTube comments,
analyze their sentiments, and visualize the results.

## Objectives

- Collect comments from YouTube food review videos.
- Clean and preprocess the collected data.
- Perform sentiment analysis using NLP techniques.
- Classify comments into positive, negative, and neutral categories.
- Visualize the distribution of sentiments.
- Save the analyzed results in a CSV file.
- Explore the use of Big Data technologies for future improvements.

## Technologies Used

- Python
- Google Colab
- YouTube Data API v3
- Pandas
- NLTK
- VADER Sentiment Analyzer
- Matplotlib
- Seaborn

## Project Workflow

1. Data Collection
   Collect publicly available top-level comments from YouTube
   food review videos using YouTube Data API v3.

2. Data Cleaning
   Remove missing values, empty comments, and duplicate records.

3. Sentiment Analysis
   Use the VADER sentiment analyzer to calculate sentiment scores.

4. Sentiment Classification
   Classify each comment as Positive, Negative, or Neutral.

5. Data Visualization
   Create graphs to display the distribution of sentiments.

6. Data Export
   Save the collected comments and sentiment results in CSV format.

## Sentiment Classification

The VADER compound score is used to classify comments:

- Positive: Compound score >= 0.05
- Negative: Compound score <= -0.05
- Neutral: Compound score between -0.05 and 0.05

These classifications are automatic predictions and may not
correctly interpret sarcasm, slang, or every type of comment.

## Dataset

The project aims to collect up to 2,000 comments from multiple
YouTube food review videos.

The actual number of comments depends on video availability,
comment settings, API quota, and successful API requests.

The dataset may contain:

- Comment text
- Video title
- Video ID
- Comment publication date
- Comment like count
- Sentiment scores
- Predicted sentiment labels

## Installation

Install the required Python libraries:

pip install -r requirements.txt

## YouTube API Setup

1. Open Google Cloud Console.
2. Create or select a Google Cloud project.
3. Enable YouTube Data API v3.
4. Create an API key.
5. Configure the API key restrictions appropriately.
6. Enter the API key securely when running the notebook.

Never upload your API key or other credentials to GitHub.

## How to Run the Project

1. Open the Jupyter Notebook file in Google Colab.
2. Install the required libraries.
3. Enter your YouTube API key securely.
4. Run the data collection code.
5. Clean the collected comments.
6. Run the sentiment analysis code.
7. Generate the sentiment visualization.
8. Download the final CSV dataset.

## Output

The project generates a CSV file containing YouTube comments
and their predicted sentiment labels.

A bar chart displays the number of positive, negative, and
neutral comments in the dataset.

## Big Data Relevance

This project demonstrates API-based data collection,
text processing, sentiment analysis, and data visualization.

Although 2,000 comments are suitable for a prototype, this
dataset alone does not establish large-scale Big Data processing.

Future development can incorporate Apache Spark and PySpark
to demonstrate distributed data processing and analysis.

## Limitations

- VADER may misclassify sarcasm and complex opinions.
- Results depend on the available YouTube comments.
- Some videos may have disabled comments.
- The dataset may not represent all viewers' opinions.
- Sentiment predictions are not guaranteed to be accurate.

## Future Improvements

- Increase the size of the dataset.
- Use Apache Spark for distributed processing.
- Compare VADER with machine learning models.
- Evaluate model performance using manually labeled data.
- Improve handling of multilingual comments and sarcasm.
- Develop an interactive sentiment analysis dashboard.

## Author

Student Project — Big Data Sentiment Analysis

## License

This project is intended for educational and research purposes.
