### Stock Market Prediction Via NLP Sentiment Analysis

**Author**

#### Executive Summary

This project focuses on using sentiment analysis to predict bullish and bearish market sentiment for stock trading sessions. Predictive models in this domain can provide significant value by aiding in capital accretion (the process of growing investment returns) and risk management. By classifying pre-market news articles, the project aims to explore how natural language processing (NLP) and machine learning can predict whether a trading day will yield a positive or negative return.

#### Rationale

Stock market predictions based on sentiment analysis can offer traders and investors a competitive edge. Sentiment-driven predictions enable market participants to anticipate trends and align their strategies with the expected outcomes. This reduces uncertainty, optimizes risk management, and fosters better decision-making, especially in volatile or unpredictable markets. Understanding the sentiment behind pre-market news can reveal underlying market behavior and help manage exposure to potential losses while capitalizing on favorable trends.

#### Research Question

Can pre-market news be used to predict the outcome (advance or decline) of stocks on a trading day?

#### Data Sources

The data for this project is sourced from:
- Pre-market news articles scraped from popular financial market news sites, including CNBC and Bloomberg.
- Publicly available stock market data to track daily stock performance.

#### Methodology

1. **Data Collection**: Pre-market news articles are aggregated from financial news websites and matched with daily stock performance data.
2. **NLP Preprocessing**: Pre-market news data is processed using techniques like stemming and lemmatization. Various vectorization methods, such as `CountVectorizer` and `TfidfVectorizer`, are applied.
3. **Classification**: Machine learning classification algorithms, including `LogisticRegression`, `DecisionTreeClassifier`, and `MultinomialNB`, are employed to predict whether a trading day will yield a return greater than or less than 0.
4. **Evaluation**: Models are evaluated against a baseline accuracy derived from guessing the most likely outcome, and the best-performing model is selected based on accuracy and classification metrics.

#### Results

- **Data Collection**: Data from June 2024 through October 2024 was collected, covering 105 trading sessions.
- **Baseline**: A 58% baseline accuracy was established by always predicting a positive trading day (61 out of the 105 trading sessions in the time period were positive).
- **Best Model**: 
  - **Vectorizer**: TfidfVectorizer
  - **Classifier**: MultinomialNB
  - **Best Parameters**: {'MultinomialNB__alpha': 0.5, 'MultinomialNB__fit_prior': True}
  - **Accuracy**: 70.4%
  - **Classification Report**:
    ```json
    {
      "0": {"precision": 0.67, "recall": 0.14, "f1-score": 0.24, "support": 14},
      "1": {"precision": 0.50, "recall": 0.92, "f1-score": 0.65, "support": 13},
      "accuracy": 0.52,
      "macro avg": {"precision": 0.58, "recall": 0.53, "f1-score": 0.44, "support": 27},
      "weighted avg": {"precision": 0.59, "recall": 0.52, "f1-score": 0.43, "support": 27}
    }
    ```

## Next Steps

- **Expand Data**: Train the model on at least one or two years of data for improved performance.
- **Explore Advanced Models**: Experiment with deep learning architectures and other classification algorithms to enhance prediction accuracy.

## Project Outline

The project is organized into a single Jupyter notebook with clearly defined sections covering data collection, preprocessing, model training, and evaluation.

## Contact Information

**Odean Maye**  
Email: odean@spectususa.com

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information