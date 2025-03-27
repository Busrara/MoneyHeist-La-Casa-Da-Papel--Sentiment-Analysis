# 🟣 Money Heist Sentiment Analysis

## Project Overview:
This project performs sentiment analysis on tweets about the popular TV series "Money Heist" (La Casa de Papel). By using the **Tweepy** library to retrieve tweets and **TextBlob** for sentiment classification, the project classifies the sentiment of each tweet as **Positive**, **Negative**, or **Neutral**. Then, the results are visualized in a **Pie Chart** by **Matplotlib**.

## Technical Details:
 **API Used**: Twitter API by the `tweepy` library.
- **Sentiment Analysis**: Performed using the `TextBlob` library, which calculates the sentiment polarity (ranges from -1 to 1).
    - Positive sentiment: Polarity > 0
    - Negative sentiment: Polarity < 0
    - Neutral sentiment: Polarity == 0
  
- **Visualization**:
- A **Pie Chart** is generated using `matplotlib` to visualize the sentiment distribution for better understanding.

## Data Collection:
- **Number of Tweets Collected**: 100 tweets about the query "Money Heist".
- **Date of Collection**: 01/03/2025.
- **Language of Tweets**: English (`lang="en"`).
  
### Limitations:
- The programme collects only 100 tweets, which is a small sample for sentiment analysis.
- Sentiment analysis is based on TextBlob, which may not always successfully understand sarcasm or complex emotions.
- The analysis does not consider context (e.g., season or episode-specific tweets).

## Requirements:
- Python 3.x
- Libraries:
  - `tweepy`: For accessing the Twitter API and retrieving tweets.
  - `textblob`: For performing sentiment analysis.
  - `matplotlib`: For visualizing the results as a pie chart.

## How to Run:
1. **Install the required libraries**:
    ```bash
    !pip install tweepy textblob matplotlib
    ```
2. **Set up Twitter API credentials**:
   - Create a [Twitter Developer Account](https://developer.twitter.com/en/apps).
   - Create an app on Twitter Developer Dashboard.
   - Get your API Key, API Secret Key, Access Token, and Access Token Secret.
3. **Authenticate and Retrieve Tweets**:
   - Replace the placeholders with your Twitter API credentials.
4. **Run the notebook** to fetch tweets and analyze their sentiment.

## Sentiment Analysis Results:
- **Positive Tweets**: 73
- **Negative Tweets**: 21
- **Neutral Tweets**: 6

### Example Output:

**Sample Tweets**:
- Tweet 1: "Money Heist is an incredible show! #MoneyHeist"
- Tweet 2: "I can't believe the ending! #MoneyHeist #WorstEnding"
- Tweet 3: "Not as exciting as I thought it would be. #MoneyHeist"

**Sentiment Distribution**:
- Positive: 50%
- Negative: 30%
- Neutral: 20%


## Conclusion:
This analysis gives insights into how the audience feel about "Money Heist", with the results visually presented. The positive sentiment makes us understand that most viewers like the show, while a smaller percentage feels negative about it.

## Future Improvements:
- **Increase the number of tweets**: We can collect more tweets to get a broader sentiment analysis.
- **Use advanced sentiment analysis models**: Utilize machine learning models to improve sentiment classification accuracy.
- **Topic Modeling**: Perform topic modeling to understand the specific themes which are being discussed in the tweets.

## License:
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


