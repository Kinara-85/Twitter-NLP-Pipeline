# Twitter NLP Pipeline

## Overview
This project involves collecting, processing, and analyzing tweets using Natural Language Processing (NLP) techniques. The main objective is to clean and label tweets based on sentiment analysis and other text-processing tasks.

## Workflow
The pipeline follows these steps:

1. **Authentication**: Connect to Twitter API using Tweepy.
2. **Extract Tweets**: Fetch recent tweets using specified keywords.
3. **Save to CSV**: Store the extracted tweets in a CSV file.
4. **Sentiment Analysis**: Label tweets as Positive, Negative, or Neutral using TextBlob.
5. **Data Cleaning**:
   - Convert short words (e.g., "u" → "you").
   - Replace contractions (e.g., "can't" → "cannot").
   - Remove retweets, special characters, and duplicates.
   - Perform spell correction.
   - Remove stopwords.
   - Tokenize and lemmatize text.
6. **Save Cleaned Data**: Export the processed dataset to a CSV file.

## Flowchart

```
        +-------------------+
        | Authenticate API  |
        +-------------------+
                 |
                 v
        +------------------+
        | Extract Tweets   |
        +------------------+
                 |
                 v
        +------------------+
        | Save to CSV      |
        +------------------+
                 |
                 v
        +----------------------+
        | Sentiment Analysis   |
        +----------------------+
                 |
                 v
        +------------------+
        | Data Cleaning    |
        +------------------+
                 |
                 v
        +------------------+
        | Save Processed   |
        | Data to CSV      |
        +------------------+
```

## Notes
This project was part of my final year thesis. Some sections have been removed as they were directly related to my research work.

