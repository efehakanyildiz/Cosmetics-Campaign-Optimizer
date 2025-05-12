🧴 Cosmetic Campaign Optimization with Machine Learning

This project builds a machine learning-based system to optimize digital marketing campaigns in the cosmetics industry. It predicts key performance indicators (KPIs) such as clicks, conversions, revenue, and ROI based on input factors like campaign type, channel, brand, region, and product category. The system also recommends the most effective strategy tailored to user constraints.


💼 BUSINESS RULE
This project aims to build a data-driven decision support system to maximize the Return on Investment (ROI) of marketing campaigns in the cosmetics industry. The business goal is to identify the key factors influencing campaign success based on historical campaign data and customer interactions, and to provide strategic predictions for future campaigns.

The core business rules are as follows:
Campaign profitability is calculated based on total revenue and campaign cost.
ROI values are predicted using regression models, and high-ROI campaign characteristics are identified.
Features such as campaign type, target audience segment, marketing channel usage, and spending level hold strategic importance in decision-making.
Model outputs support marketing teams in making more efficient budget allocations and campaign planning decisions.
The aim is to enhance both short-term profitability and long-term customer value.

🚀 Features

Data Cleaning & Feature Engineering
Handles missing values and outliers
Extracts date-based features
Calculates ROI and net profit
Multi-Target Prediction
Predicts campaign duration, clicks, conversions, revenue, and net profit using models like:
RandomForestRegressor
GradientBoostingRegressor
Automatic Strategy Recommendation
Evaluates all combinations of campaign types and channels
Suggests the highest-scoring strategy based on expected ROI, profit, and conversion efficiency
Data Visualization
ROI by product category
Budget vs ROI scatter plot
Average conversions by channel
Interactive Console Interface
Lets users enter their region, brand, product category, and budget
Returns strategy recommendations and performance expectations
🧠 Tech Stack

Python
Scikit-learn for modeling
Pandas for data manipulation
Matplotlib & Seaborn for visualizations
Joblib for model saving (optional)
📁 File Structure

.
├── main.py                 # Main script with functions and execution
├── kozmetik_dataset.csv    # Input dataset (example)
├── feature_importance.png  # Saved feature importance plots
├── *.png                   # Visual reports (e.g., budget vs ROI)
└── README.md               # Project overview
📊 Models & Evaluation

Each target variable is modeled separately. Model performance is evaluated using:

RMSE
MAE
R² Score
Visual comparisons between predicted and actual values are saved for each KPI.

🧪 How to Use

Prepare your dataset
Must include features like budget, region, brand, product_category, etc.
Run the script
python main.py
Interact with the console
Select region, brand, product category, and budget
View top strategies and predictions
📈 Example Output

*** Recommended Campaign Strategy ***
Region: Istanbul
Brand: BrandX
Product Category: Skincare
Budget: 10,000 TL

Campaign Type: Social Media
Channel: Instagram
Recommended Duration: 15 days

Estimated Clicks: 12,000
Estimated Conversions: 2,300
Estimated Revenue: 36,000 TL
Estimated Net Profit: 26,000 TL
ROI: 2.6x
📌 Notes

ROI is capped at 3.0 to avoid skewed results from outliers
Campaign duration is bounded between 3 to 60 days
Predictions assume mid-year campaigns for consistency
📷 Visualizations

Sample output plots:

feature_importance.png
budget_roi.png
category_roi.png
channel_conversions.png
🤝 Contributing

Feel free to open issues or submit PRs for improvements, especially for:

New model integrations (e.g., XGBoost, LightGBM)
Web-based UI implementation
Multilingual support
📜 License

This project is licensed under the MIT License. See LICENSE for more details.
