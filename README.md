# Natural Language Processing with Disaster Tweets

## Project Overview
This project is part of the Kaggle competition "Natural Language Processing with Disaster Tweets". The goal is to build a machine learning model that predicts which Tweets are about real disasters and which ones are not.

## Dataset
The dataset contains 7,613 tweets that have been manually classified. The features include:
- id: A unique identifier for each tweet
- text: The text of the tweet
- location: The location the tweet was sent from (may be blank)
- keyword: A particular keyword from the tweet (may be blank)
- target: 1 if the tweet is about a real disaster, 0 if not (this is the target variable)

## Approach
1. Data Preprocessing:
   - Cleaned text by removing URLs, special characters, and extra spaces
   - Converted text to lowercase
   - Tokenized the text and removed stop words

2. Exploratory Data Analysis (EDA):
   - Analyzed the distribution of tweet lengths
   - Created word clouds for disaster and non-disaster tweets
   - Examined the balance of the target variable

3. Model Architecture:
   - Implemented a Bidirectional LSTM (Long Short-Term Memory) neural network
   - Used an embedding layer to create word vectors
   - Applied dropout for regularization

4. Training and Evaluation:
   - Split the data into training and testing sets
   - Trained the model using early stopping to prevent overfitting
   - Evaluated the model using accuracy, precision, recall, and F1-score

## Results
- Achieved an accuracy of 80.30% on the test set
- Produced a balanced performance between disaster and non-disaster tweet classification

## Files in the Repository
- `disaster_tweets_analysis.ipynb`: Jupyter notebook containing all the code and analysis
- `Kaggle-score`: Kaggle competition score
- `README.md`: This file, providing an overview of the project

## How to Run
1. Ensure you have the required libraries installed (tensorflow, keras, pandas, numpy, matplotlib, seaborn)
2. Open and run the Jupyter notebook `disaster_tweets_analysis.ipynb`
3. The `submission.csv` file will be generated for Kaggle submission

## Future Improvements
- Experiment with more advanced architectures like BERT
- Implement ensemble methods
- Conduct more extensive hyperparameter tuning

## Acknowledgements
This project was completed as part of "Introduction to Depp Learning". The dataset is provided by the Kaggle competition "Natural Language Processing with Disaster Tweets".
