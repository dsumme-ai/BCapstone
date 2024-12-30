### Where to put your money?

**Doug Summe**

#### Executive summary
This research focuses on analyzing the top 20 technology companies that have seen the largest stock market gains. As a long-term investor, the goal is to optimize capital allocation among these companies to maximize upside potential while minimizing downside risk. The strategy involves using quarterly data to decide on adding or trimming positions, avoiding day trading in favor of more sustainable portfolio adjustments. This study aims to develop a data-driven model for effective investment decision-making.

#### Rationale
Why should anyone care about this question?
The large-cap technology firms have amassed significant market value and are key drivers of the stock market’s overall performance. Understanding their growth trends and financial health is critical for investors seeking to capitalize on these companies’ long-term growth potential. By leveraging data and financial metrics, investors can make informed decisions to enhance returns while mitigating risks.

#### Research Question
What are you trying to answer?
How can a data-driven model be used to optimize quarterly capital allocation among the top 20 technology companies, maximizing upside potential and protecting against downside risk?


#### Data Sources
What data will you use to answer you question?

	1.	Yahoo Finance (via yfinance): Historical stock prices, financial metrics (revenue growth, margins, ratios).
	2.	Quarterly Reports: Earnings reports for detailed financial performance.
	3.	Macroeconomic Indicators (if applicable): To provide context on external market influences.


#### Methodology
What methods are you using to answer the question?

1.	Feature Engineering:
	•	Create lagged features, rolling averages, and financial ratios.
	•	Calculate quarter-over-quarter and year-over-year changes for financial metrics and stock prices.
2.	Modeling Approach:
	•	Train machine learning models (e.g., Random Forest, XGBoost) to predict stock price trends.
	•	Use regression for price prediction and classification for price direction.
3.	Backtesting:
	•	Simulate portfolio performance using historical data to evaluate investment strategies.
4.	Evaluation Metrics:
	•	Sharpe Ratio, Maximum Drawdown, RMSE for regression, and classification accuracy for model performance.

#### Results
What did your research find?
XGBoast was the best performing model


### Future work and considerations 

Given Market sentiment Twitter/X have API for how stocks maybe trending, as MEME stocks and other conditions can cause stock to fluxuate on not finance outcomes/potential. 

1. **Model Deployment**:  
   - Develop a user-friendly interface for real-time portfolio suggestions based on user-provided holdings.  
2. **Data Augmentation**:  
   - Incorporate sentiment analysis from social media and news to enhance predictive capabilities.  
3. **Model Enhancement**:  
   - Explore neural network architectures to further improve model performance and scalability.  

#### Outline of project

- [Data Prep and Model evaluation](https://github.com/dsumme-ai/BCapstone/blob/main/Capstone.ipynb)



##### Contact and Further Information

dsumme@gmail.com
