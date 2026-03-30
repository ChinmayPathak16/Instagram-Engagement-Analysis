\# Instagram User Engagement Analysis (Big Data Project)



\## Introduction



This project focuses on analyzing Instagram user engagement using Big Data technologies and Machine Learning. It simulates how large-scale platforms process user interaction data and generate insights for content optimization.



\---



\## Problem Statement



To analyze large-scale Instagram engagement data and build a predictive model that classifies posts into high or low engagement categories using PySpark.



\---



\## Dataset



\* Synthetic dataset generated using Python

\* Total records: 1000+

\* Designed to simulate real-world Instagram data



\### Features:



\* likes, comments, shares, saves

\* followers

\* views, watch\_time

\* hashtags\_count, caption\_length

\* posted\_hour

\* post\_type (image, reel, video)



\---



\## System Architecture (Flow Diagram)



Raw Data Generation (Python)

↓

Data Storage (CSV)

↓

Data Loading (PySpark)

↓

Data Cleaning \& Validation

↓

Exploratory Data Analysis

↓

Feature Engineering (engagement\_score)

↓

Feature Transformation (VectorAssembler)

↓

Machine Learning Model (Logistic Regression)

↓

Prediction (High / Low Engagement)

↓

Results \& Insights



\---



\## Tools \& Technologies



\* Python

\* PySpark (Distributed Data Processing)

\* Spark MLlib (Machine Learning)

\* NumPy

\* Git \& GitHub



\---



\## Working Methodology



\### 1. Data Generation



A synthetic dataset was generated using Python to simulate Instagram-like engagement data.



\### 2. Data Processing



Data was loaded into PySpark DataFrames for distributed processing and scalability.



\### 3. Data Cleaning



Checked for missing/null values and ensured consistency across all columns.



\### 4. Exploratory Data Analysis



\* Calculated average likes, comments, shares

\* Compared engagement across post types

\* Identified best posting hours



\### 5. Feature Engineering



Created a new feature:



engagement\_score = (likes + comments + shares) / followers



\### 6. Feature Transformation



\* StringIndexer → convert post\_type to numeric

\* VectorAssembler → combine features



\### 7. Machine Learning



\* Algorithm: Logistic Regression

\* Library: Spark MLlib

\* Task: Binary Classification (High vs Low Engagement)



\---



\## Key Results \& Insights



\* Average Likes: \~5185

\* Average Comments: \~271

\* Average Shares: \~518



\### Engagement Insights:



\* Reels show slightly higher engagement than images and videos

\* Evening hours (19–21) show highest engagement

\* Engagement strongly depends on interaction metrics and follower count



\### Model Performance:



\* Accuracy: \~99% (due to synthetic dataset)

\* Successfully predicts engagement category



\---



\## Technical Highlights



\* Distributed data processing using PySpark

\* Feature engineering for normalized engagement metrics

\* Use of MLlib for scalable machine learning

\* End-to-end pipeline from raw data to prediction

\* Simulation of real-world recommendation systems



\---



\## Conclusion



This project demonstrates how Big Data tools like PySpark can be used to analyze large-scale social media data and build predictive models for engagement. It provides insights similar to real-world systems used by platforms like Instagram.



\---



\## Future Scope



\* Integration with real-world Instagram API data

\* Advanced ML models (Random Forest, Gradient Boosting)

\* Deployment using Flask or Streamlit

\* Real-time data streaming using Kafka

\* Dashboard visualization



\---



\## How to Run



pip install pyspark numpy

python generate\_data.py

python analysis.py



\---





