# Stock Sentiment Analysis using News Headlines

1. Develop a sentiment-based stock market analysis system to predict stock price movements by analyzing and interpreting sentiment data from news articles, social media, and other sources.
2. The system should identify and categorize sentiment as positive, negative, or neutral and then correlate this sentiment data with historical stock market data to provide insights into potential price trends.
3. The goal is to create a predictive model that helps traders and investors make informed decisions based on sentiment analysis.
4. [Dataset Used](https://drive.google.com/file/d/1TofKCCkTKKDeXtHvyw4GT-N3DiyPcvyq/view?usp=sharing)

# IMPLEMENTATION STEPS :

### Data Collection

### Data Pre-processing

- Cleaned and preprocessed text data to remove noise, special characters, and punctuation.
- Tokenized text data and performed stemming or lemmatization.
- Created a Bag of Words representation of the text data.

### Sentiment Analysis

- Labeled the text data with sentiment scores (e.g., positive, negative, neutral).
- Created a target variable based on stock price movement (e.g., 'Up', 'Down').

### Dataset Splitting

- Split the dataset into training and testing subsets for model evaluation.

### Model Building (Random Forest Classifier)

- Trained a Random Forest classifier on the training data.
- Utilized the BoW features and sentiment labels.

### Model Evaluation

- Evaluated the Random Forest model's performance using metrics like accuracy, precision, recall, F1-score, and confusion matrices.
- Analyzed feature importance to identify influential words.
