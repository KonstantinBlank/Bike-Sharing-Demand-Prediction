# Seoul Bike Sharing Demand Prediction 🚲📊

## Authors
* Jagoda Wiecek
* Konstantin Blank
* Baptiste Rimet

## Context and Motivation
Bike-sharing systems are a growing trend in urban mobility, offering sustainable transportation solutions. This project analyzes the Seoul Bike Sharing Demand dataset to explore how factors like weather, time of day, and holidays influence hourly bike usage. While the dataset is specific to Seoul, the analysis provides a practical case study for understanding bike-sharing dynamics—a highly relevant topic in cycling-centric regions like Denmark.

For bike-sharing operators, balancing supply and demand is critical. Poor management can lead to:
* User frustration due to bike shortages during peak hours.
* Inefficient operations and unnecessary manual bike redistribution.

## Research Question
**Which factors explain the variation in hourly bike-sharing demand, and how can this information inform better bike management?**

## The Dataset
The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand) and consists of 14 variables, with **Rented Bike Count** serving as the target variable. These features capture comprehensive temporal, environmental, and operational conditions:

* **Target Variable:** `Rented Bike Count` (Number of bikes rented each hour)
* **Time Features:** `Date`, `Hour`, `Seasons`, `Holiday`
* **Weather Features:** `Temperature (°C)`, `Humidity (%)`, `Wind Speed (m/s)`, `Visibility (10m)`, `Dew Point Temperature (°C)`, `Solar Radiation (MJ/m2)`, `Rainfall (mm)`, `Snowfall (cm)`
* **Operational Features:** `Functioning Day`

## Project Goals & Methodology
1. **Exploratory Data Analysis:** Leveraging descriptive statistics and visualizations to identify initial historical trends.
2. **Predictive Regression Modeling:** Applying and comparing various machine learning models to quantify factor impacts and predict future demand accurately.
3. **Practical Takeaways:** Providing data-driven insights to help operators manage bike availability proactively.

## Tech Stack
This project is built using Python. Key libraries and frameworks include:
* **Data Processing & Manipulation:** `numpy`, `pandas`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning (Scikit-learn):** `Linear Regression`, `Ridge`, `Lasso`, `ElasticNet`, `DecisionTreeRegressor`, `RandomForestRegressor`, `GradientBoostingRegressor`
* **Advanced Gradient Boosting:** `XGBoost`
* **Deep Learning:** `PyTorch` (Neural Networks)

## Key Findings & Conclusions
The analysis reveals that bike-sharing demand is a complex interplay of predictable patterns and external influences:
1. **Daily & Seasonal Commute Patterns:** Demand peaks correlate strongly with standard commuting hours. Operators should increase fleet sizes and maintenance efforts during summer/autumn and adapt scheduling for daily commute peaks.
2. **Weather-Driven Strategies:** Externalities like temperature, rainfall, and snow significantly shift user behavior. During periods of poor weather, operators can reduce availability in certain areas, while preparing for increased demand on optimal weather days.
3. **Strategic Event Planning:** Comparing known local event calendars with predicted high-demand periods allows operators to proactively position extra bikes and staff near venues, successfully handling outlier patterns.

By integrating predictive modeling with an understanding of these influential factors, operators can shift from reactive fixes to **proactive management**, ensuring optimal bike availability, reducing operational inefficiencies, and enhancing the overall user experience.
