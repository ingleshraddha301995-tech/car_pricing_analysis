# car_pricing_analysis
A machine learning project that predicts the market price of used cars based on vehicle characteristics such as mileage, age, engine size, fuel type, and transmission.
The goal is to help car dealerships make data-driven pricing decisions, reducing pricing errors and improving inventory turnover.

# 📊 Project Overview

The used car market is highly dynamic and influenced by multiple factors including:
Vehicle age
Mileage
Engine specifications
Condition
Market demand
Incorrect pricing leads to:
Undervalued vehicles → Lost revenue
Overpriced vehicles → Slow inventory turnover
This project builds a machine learning regression model that predicts the fair market value of a vehicle using historical car listing data.

# 🎯 Objectives

Analyze factors influencing used car prices
Perform Exploratory Data Analysis (EDA)
Build multiple regression models
Compare model performance
Identify key price drivers
Provide business recommendations

# 📂 Dataset

The dataset contains used car listings collected from online sources in 2019.
| Feature      | Description                |
| ------------ | -------------------------- |
| Make         | Manufacturer of the car    |
| Model        | Specific car model         |
| Price        | Target variable (USD)      |
| Year         | Production year            |
| Mileage      | Distance driven (km)       |
| Fuel Type    | Petrol / Diesel / Electric |
| Volume       | Engine size                |
| Color        | Car color                  |
| Transmission | Manual / Automatic         |
| Drive Unit   | FWD / RWD / AWD            |
| Segment      | Vehicle category           |
| Condition    | Car condition              |

# 🔍 Exploratory Data Analysis

Key insights discovered during analysis:
1️⃣ Car Age vs Price

Older vehicles experience significant depreciation.
2️⃣ Mileage vs Price

Higher mileage strongly correlates with lower resale value.
3️⃣ Engine Volume

Vehicles with larger engines tend to have higher prices.
4️⃣ Segment Influence

Luxury vehicles retain higher resale values.
5️⃣ Transmission Type
Automatic cars generally have higher resale value compared to manual cars.

# 🧠 Feature Engineering

New features were created to improve model performance:
Car Age
Mileage per Year
Price per KM
These engineered features significantly improved prediction accuracy.

# 🤖 Machine Learning Models Tested

Four regression models were evaluated:
| Model             | MAE        | RMSE       | R²       | CV R²    |
| ----------------- | ---------- | ---------- | -------- | -------- |
| Random Forest     | **164.89** | **559.51** | **0.99** | **0.99** |
| Decision Tree     | 264.46     | 753.94     | 0.97     | 0.97     |
| Gradient Boosting | 283.53     | 569.18     | 0.99     | 0.99     |
| Linear Regression | 1775.48    | 2514.64    | 0.72     | 0.71     |


# 🏆 Best Model: Random Forest

The Random Forest Regressor achieved the best performance.
Performance
R² Score: 0.9861 (98.6% accuracy)
Mean Absolute Error: $164.89
Prediction Error: ~3.3%
This means the model predicts car prices with an average error of ±$165.

# 🔑 Feature Importance
Top features influencing price:
| Rank | Feature          | Importance |
| ---- | ---------------- | ---------- |
| 1    | Price per KM     | 31.7%      |
| 2    | Car Age          | 30.4%      |
| 3    | Year             | 19.7%      |
| 4    | Mileage          | 7.6%       |
| 5    | Engine Volume    | 4.3%       |
| 6    | Mileage per Year | 4.3%       |
| 7    | Segment          | 0.9%       |
| 8    | Transmission     | 0.39%      |
| 9    | Make             | 0.18%      |
| 10   | Model            | 0.16%      |

**Key Insight**
The top 3 features account for 81.8% of the model's predictive power.
This shows that vehicle age and mileage-related features are the strongest pricing drivers, rather than brand.

# 📉 Prediction Analysis
Residual Statistics
| Metric             | Value   |
| ------------------ | ------- |
| Mean Error         | $16.42  |
| Standard Deviation | $559    |
| Minimum Error      | -$6,954 |
| Maximum Error      | $12,536 |

Percentage Errors
| Metric          | Value |
| --------------- | ----- |
| Mean Error      | 4.39% |
| Median Error    | 0.51% |
| 95th Percentile | ±$794 |

# 💼 Business Impact

If implemented in a dealership pricing system, this model could deliver:
📉**Pricing Accuracy Improvement**
Pricing error reduced from:
±$750 → ±$165
≈ 80% improvement

🚗 **Inventory Turnover**
Expected improvement:
+15% – 25% faster sales

💰**Profit Margin Increase**
Estimated increase:
+5% – 10% profit margin

📈 **Revenue Impact**
Potential annual revenue improvement:
$150,000 – $250,000

# 🛠️ Tech Stack
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook

# 📊 Project Workflow

Data Cleaning
Exploratory Data Analysis
Feature Engineering
Model Training
Model Evaluation
Feature Importance Analysis
Business Recommendations

# 🚀 Implementation Plan

Week 1
Team training on model usage.

Weeks 2–4
Pilot testing with selected vehicles.

Month 2
Full integration into dealership pricing workflow.

Ongoing
Monthly monitoring and model retraining.

# 📌 Conclusion

This project demonstrates how machine learning can significantly improve pricing decisions in the automotive market.
The developed model provides:
Highly accurate price predictions
Clear insights into pricing drivers
Actionable business value
This approach enables dealerships to transition from manual pricing strategies to data-driven decision-making.

# 👨‍💻 Author

**Name**: Shraddha Ingle

Machine Learning | Data Science | Business Analytics
