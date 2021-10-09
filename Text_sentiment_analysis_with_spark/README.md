# Real time Sentiment analysis using spark Mllib and spark structured streaming 
This project presents a sentiment analysis pipeline implementation using spark in python to 
classify tweets polarity (positive/negative), this implementation uses data from kaggle, 
https://www.kaggle.com/kazanova/sentiment140.

This implementation:

• Preprocesses and cleans the text.

• Trains a Logistic regression model to classify tweets using spark’s Mllib.

• Applies the model to streaming tweets from twitter API using spark’s structured 
straming.

• Finally saves the output to a parquet file
