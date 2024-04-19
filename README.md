# Stock Sentiment Analysis using News Headlines

1. Develop a sentiment-based stock market analysis system to predict stock price movements by analyzing and interpreting sentiment data from news articles, social media, and other sources.
2. The system should identify and categorize sentiment as positive, negative, or neutral and then correlate this sentiment data with historical stock market data to provide insights into potential price trends.
3. The goal is to create a predictive model that helps traders and investors make informed decisions based on sentiment analysis.
4. [Presentation Link](https://docs.google.com/presentation/d/1LBmARgbd_I-7k4FbuzoT4gE_axkdfUrc-txeirvlaoY/edit?usp=sharing)
5. [Dataset Used](https://drive.google.com/file/d/1TofKCCkTKKDeXtHvyw4GT-N3DiyPcvyq/view?usp=sharing)

# IMPLEMENTATION STEPS :

### Data Collection

- Using the given dataset (.csv file)

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

# Common Terms and Functions :

1. **Stopwords :** A stop word is a commonly used word (such as “the”, “a”, “an”, or “in”) that a search engine has been programmed to ignore, both when indexing entries for searching and when retrieving them as the result of a search query. Used in `from nltk.corpus import stopwords`

   ![Stop word removal using NLTK](https://media.geeksforgeeks.org/wp-content/cdn-uploads/Stop-word-removal-using-NLTK.png)

2. **Stremmer :** The process of producing morphological variants of a root/base word. Stemming programs are commonly referred to as stemming algorithms or stemmers. A stemming algorithm reduces the words “chocolates”, “chocolatey”, and “choco” to the root word, “chocolate” and “retrieval”, “retrieved”, “retrieves” reduce to the stem “retrieve”. Used in `from nltk.stem import PorterStemmer`
3. **Precision:** Precision measures the accuracy of positive predictions. It is the proportion of true positives against all the positives predicted by the model. This metric is particularly important when the cost of a false positive is high. **Precision = True Positives (TP) / (True Positives (TP) + False Positives (FP))**
4. **Recall (Sensitivity) :** Recall measures the ability of a model to find all the relevant cases (i.e., true positives) within a dataset. It is the proportion of actual positives that were correctly identified. This metric is crucial when the cost of a false negative is high. **Recall = True Positives (TP) / (True Positives (TP) + False Positives (FN))**
5. **F1 Score :** The F1 score is the harmonic mean of precision and recall. It is used as a single metric to balance both the precision and recall of a binary classification model. It is particularly useful when you want to find a balance between precision and recall and there is an uneven class distribution (large number of actual negatives).
