# ⛽ Grandmeister Station Fuel Analysis

## 🚀 Project Overview
This project analyzes transactional and environmental data from Grandmeister Station with the goal of predicting average flow rates and identifying patterns in fuel dispensing behavior. By integrating transaction logs with sand ocean weather data, our goal is to optimize equipment usage and reduce operational downtime.

## 🧠 Problem Statement
“Predict average flow rates and analyze fuel dispensing patterns at Grandmeister units to optimize equipment usage and reduce downtime.”

Fuel stations face irregular usage patterns, influenced by factors such as temperature, time of day, and day of the week. This analysis supports decision-making through predictive modeling, downtime analytics, and flow efficiency tracking.

## 📂 Datasets Used
Grandmeister Transfer Transactions Dataset

Sand Ocean Weather Dataset

These datasets were merged for integrated analysis of fuel station performance alongside weather conditions.

## 🔧 Project Workflow
## 1. 🧹 Data Cleaning
Removed missing and inconsistent values

Converted timestamps and formatted categorical variables

Merged transactional data with weather information

## 2. 📊 Exploratory Data Analysis (EDA)
A wide range of visualizations were generated to explore:

Transaction Count by Hour

Average Flow Rate Distribution

Scatter Plot: Flow Rate vs Air Temperature

Downtime Analysis

Flow Rate by Day of the Week and Part of the Day

Effect of Temperature & Precipitation on Flow Rate

High Downtime Flags

## 3. 🏗️ Feature Engineering
Engineered new features to enrich the dataset:

Downtime: Time spent not dispensing fuel

Temperature Categories: Binned temperature ranges (e.g. cold, moderate, hot)

Is High Flow: Flag transactions above average flow rate

Temperature Impact Category: Combines temperature and downtime for risk assessment

## 4. 🤖 Model Building
Used Random Forest Regressor to predict the average flow rate based on engineered features.

Key Steps:
Defined features and target

Train-test split (80/20)

Preprocessing pipeline:

Imputation

Scaling

Encoding

Model training & evaluation (using RMSE)

## 📈 Key Insights from EDA
Temperature and flow rate are positively correlated — colder weather may reduce fuel performance.

Downtime is higher during colder or extreme weather conditions.

Afternoon and weekday transactions tend to have higher average flow rates.

Some pumps consistently show lower flow rates, signaling possible maintenance issues.

## 💡 Technologies & Libraries
Python

Pandas, NumPy – Data manipulation

Matplotlib, Seaborn, Plotly – Data visualization

Scikit-learn – Modeling and pipelines

Google Colab – Cloud-based development

## 👥 Team Members
Ashna Batra

Jannat Narang

Rakshit Bhardwaj

## 📌 Conclusion
This project demonstrates how data fusion and predictive analytics can support better resource management at fuel stations. By correlating environmental conditions with performance metrics, we’ve taken the first step toward data-driven operational efficiency.

## Link to the Jupyter Notebook
[Project2_Link](https://github.com/Ashna-20/Ashna-Portfolio/blob/main/Restaurant_Locator_System.ipynb)
