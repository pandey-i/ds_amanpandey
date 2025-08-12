Bitcoin Sentiment and Trader Behavior Analysis
This project analyzes the relationship between Bitcoin sentiment and trader behavior using a dataset containing sentiment classifications and detailed trading data.

Project Objective
The main objective of this project is to understand how different Bitcoin sentiment categories (Extreme Greed, Extreme Fear, Fear, Greed, Neutral) impact trading metrics such as:

Daily Total Volume
Daily Average Leverage (approximated by Daily Average Trade Size in USD)
Daily PnL (Profit and Loss)
Risk Metrics (Ratio of losing trades to total trades)
The analysis also investigates specific trading behaviors observed during different sentiment periods.

Data
The analysis utilizes two datasets:

bitcoin_sentiment.csv: Contains daily Bitcoin sentiment classifications.
trader_data.csv: Contains detailed individual trading data.
Both datasets are expected to be in the /content/csv_files/ directory.

Analysis
The analysis involves the following steps:

Loading and merging the sentiment and trader data based on the date.
Feature engineering to calculate daily trading metrics per trader.
Analyzing the engineered metrics across different sentiment categories.
Investigating specific patterns in trader behavior during 'Greed' periods.
Summarizing the key findings and insights.
The analysis is performed in the accompanying Jupyter Notebook.

Results and Outputs
The project generates the following outputs:

daily_metrics.csv: CSV file containing the calculated daily metrics per trader.
sentiment_metrics.csv: CSV file summarizing average metrics by sentiment category.
sentiment_difference.csv: CSV file showing the difference in metrics between 'Greed' and 'Fear' sentiment.
pnl_distribution.png: Box plot visualizing the distribution of Closed PnL under 'Fear' vs 'Greed'.
greed_daily_trade_counts.png: Plot showing the distribution of trade sizes and daily trade counts during 'Greed' periods.
These output files are saved in the /content/csv_files/ and /content/outputs/ directories respectively.

How to Run the Notebook
Ensure you have a Python environment with the necessary libraries installed (pandas, matplotlib, seaborn).
Place the bitcoin_sentiment.csv and trader_data.csv files in a directory named /content/csv_files/.
Open the Jupyter Notebook (.ipynb file) in a compatible environment (like Google Colab or Jupyter Notebook).
Run the cells sequentially to execute the analysis.
Conclusion
The analysis provides insights into how Bitcoin sentiment correlates with trader behavior and profitability. The findings suggest that trading during periods of 'Fear' and 'Extreme Greed' might be associated with higher average PnL, while 'Greed' periods show lower trading volume and average trade size, potentially due to the nature of trades executed during these times.


