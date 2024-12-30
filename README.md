### Where to put your money?

**Doug Summe**

# Capstone Project  
**Optimizing Quarterly Capital Allocation for Top Technology Companies**

---

## **Define the Problem Statement**  
The problem is to develop a machine learning model to optimize quarterly capital allocation among the top 20 technology companies based on financial and stock performance data. The goal is to maximize upside potential while minimizing downside risk, enabling long-term investors to make informed and sustainable investment decisions. The challenge lies in leveraging historical data to predict trends and inform portfolio adjustments without relying on short-term trading.

---

## **Model Outcomes or Predictions**  
- **Type of Learning**: Supervised learning.  
- **Expected Output**:  
  - **Classification**: Predict the target category of stock performance (e.g., "low," "medium," "high").  
  - **Regression**: Forecast stock price movements.  
- **Algorithms Used**: Models like XGBoost and Random Forest were selected for their ability to handle complex datasets with mixed feature types effectively.  

---

## **Data Acquisition**  
**Data Sources**:  
1. **Yahoo Finance (via yfinance)**: Used to acquire historical stock prices and financial metrics, such as revenue growth, gross margin, ROA, ROE, and debt-to-equity ratios.  
2. **Quarterly Reports**: Provided detailed financial performance data.  
3. **Macroeconomic Indicators**: Supplemented financial metrics for external market context (if applicable).  

**Data Visualization**:  
- Histograms, correlation matrices, and rolling average plots were used to explore data distributions and identify trends.  
- Feature importance charts helped evaluate the most predictive variables for stock performance.  

---

## **Data Preprocessing/Preparation**  
### **Steps Taken**  
1. **Handling Missing Values**:  
   - Imputed missing financial metrics using forward and backward fill or median imputation.  
   - Replaced missing lagged values with rolling averages to maintain trend consistency.  

2. **Feature Engineering**:  
   - Created lagged features for stock prices and financial metrics (e.g., `revenue_growth_lag_1`).  
   - Generated rolling averages and standard deviations for volatility tracking.  
   - Computed quarter-over-quarter and year-over-year changes in financial performance.  

3. **Encoding**:  
   - Encoded categorical variables such as `Ticker` using label encoding.  
   - Introduced a numerical `quarter` feature to capture seasonal trends.  

4. **Train-Test Split**:  
   - Split the data into training (80%) and test (20%) sets, ensuring chronological integrity to mimic real-world prediction scenarios.  

---

## **Modeling**  
### **Machine Learning Algorithms**  
1. **XGBoost**: Selected for its high accuracy (~94%) and ability to handle imbalanced datasets effectively.  
2. **Random Forest**: Used for comparison and feature importance analysis.  
3. **Gradient Boosting**: Explored as an alternative ensemble method but slightly underperformed XGBoost.  

### **Feature Selection**  
- Key features included stock prices, financial ratios (e.g., gross margin, ROA), and engineered features like `stock_price_yoy`.  

---

## **Model Evaluation**  
### **Metrics**  
1. **Classification Accuracy**: XGBoost achieved ~94% accuracy in predicting stock performance categories.  
2. **Regression Metrics**: Root Mean Square Error (RMSE) was used for regression tasks to evaluate stock price prediction.  
3. **Portfolio Metrics**: Metrics like the Sharpe Ratio and Maximum Drawdown were applied during backtesting to assess the model's impact on investment performance.  

### **Findings**  
- XGBoost consistently outperformed other models in classification tasks (~94%).  
- Feature engineering significantly improved model accuracy, with lagged and rolling features playing a critical role.  

---

## **Future Work**  
1. **Model Deployment**:  
   - Develop a user-friendly interface for real-time portfolio suggestions based on user-provided holdings.  
2. **Data Augmentation**:  
   - Incorporate sentiment analysis from social media and news to enhance predictive capabilities.  
3. **Model Enhancement**:  
   - Explore neural network architectures to further improve model performance and scalability.  

---

## **Outline of Project**  
1. **Data Preparation**:  
   - Collected, cleaned, and engineered data features for modeling.  
2. **Model Selection**:  
   - Evaluated multiple machine learning algorithms.  
3. **Model Deployment**:  
   - Exported the final XGBoost model for integration with real-world investment tools.  


#### Outline of project

- [Data Prep and Model evaluation](https://github.com/dsumme-ai/BCapstone/blob/main/Capstone.ipynb)



##### Contact and Further Information

dsumme@gmail.com
