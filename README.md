# 🏡 California Housing Prices Analysis
# 📌 Project Overview
This project explores housing prices across California using a dataset that includes geographic, demographic, and economic features. The goal is to prepare and analyze the data for predictive modeling, such as estimating median house values based on various factors.

# 📂 Dataset Information

Source File: housing.csv
Rows: ~20,433 entries
Columns: 10 features
Data Types:

9 numerical (float64)
1 categorical (object)



# Features
ColumnDescriptionlongitudeGeographic longitudelatitudeGeographic latitudehousing_median_ageMedian age of houses in the blocktotal_roomsTotal number of roomstotal_bedroomsTotal number of bedroomspopulationPopulation in the blockhouseholdsNumber of householdsmedian_incomeMedian income of householdsmedian_house_valueTarget variable: Median house value (USD)ocean_proximityCategorical: Distance to ocean (INLAND, <1H OCEAN, NEAR OCEAN, etc.)

# ✅ Data Preprocessing

Missing Values: Dropped rows with nulls.
Encoding: One-hot encoding applied to ocean_proximity.
Normalization: Log transformation on skewed features (total_rooms, total_bedrooms, population, households).
Train-Test Split:

X = All features except median_house_value
y = median_house_value
Split: 80% train / 20% test




# 📊 Visualizations

Histograms: Distribution of numerical features.
Correlation Heatmap: Shows relationships between features and target.
Sample Insights:

Median house values range from $69,300 to $500,001.
Median income strongly correlates with house value.
Ocean proximity significantly impacts pricing.




# 🔍 Modeling Intent
The dataset is prepared for regression tasks to predict housing prices. Future steps may include:

Linear Regression
Random Forest
Gradient Boosting
Model evaluation using RMSE, MAE, and R².


# 🛠 Tools & Libraries

Python: Data analysis and modeling
Pandas & NumPy: Data manipulation
Matplotlib & Seaborn: Visualization
Scikit-learn: Train-test split and modeling

# ✅ Understanding the Data

Summarizing distributions of features (e.g., income, house age, population).
Identifying patterns and relationships (e.g., how proximity to the ocean affects house prices).
Detecting anomalies or outliers.

# ✅ Answering Business or Research Questions

Which areas have the highest median house values?
How does median income correlate with housing prices?
What demographic factors influence housing markets?

# ✅ Visualization & Insights

Histograms, scatter plots, and heatmaps to show trends.
Geographic mapping of prices across California
