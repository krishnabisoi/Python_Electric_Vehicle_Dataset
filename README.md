# 🚗 Electric Vehicle Trends in the USA

## **EV Adoption, Range Analysis & Predictive Modeling (Washington State Focus)**

### 📌 Project Overview

This project analyzes Electric Vehicle (EV) adoption trends in the United States, with a deep focus on Washington State, using publicly available government data. The study examines Battery Electric Vehicles (BEVs) and Plug-in Hybrid Electric Vehicles (PHEVs) to uncover patterns in adoption, electric range, pricing, and geographic distribution.

Beyond exploratory analysis, the project builds a machine learning model to predict EV type using vehicle attributes such as make, model year, and electric range.

The goal is simple: turn raw EV registration data into actionable insights for policymakers, manufacturers, and researchers

### 🎯 Research Questions
This project answers the following:
  1. How is EV adoption distributed across Washington State by county and city?
  2. What trends exist in EV adoption, electric range, and pricing over time?
  3. How do BEVs and PHEVs differ in range characteristics and market dominance?
  4. Can we predict EV type using vehicle-level features?

### 📊 Dataset
  * Source: [U.S. Government Open Data] (https://catalog.data.gov/dataset/electric-vehicle-population-data).
  * Dataset: Electric Vehicle Population Data (Washington State).
  * Scope: Vehicle registrations, electric range, MSRP, model year, make, and geographic attributes.
  * Link: https://catalog.data.gov/dataset/electric-vehicle-population-data.

The dataset includes both BEVs and PHEVs, making it suitable for comparative analysis and supervised learning.

### 🧠 Methodology
  1️⃣ Data Cleaning & Preprocessing
    * Loaded and processed using Pandas.
    * Handled missing values to maintain data integrity.
    * Encoded categorical variables (Make, EV Type) using label encoding and one-hot encoding
    * Selected relevant features for analysis and modeling

  2️⃣ Exploratory Data Analysis (EDA)
  Key analyses include:
    * Distribution of BEVs vs. PHEVs.
    * Electric range distribution (short, medium, long).
    * Adoption trends over model years.
    * EV penetration by county and city.
    * Manufacturer comparison by electric range.
    * EDA revealed that BEVs dominate the dataset, with significantly higher adoption than PHEVs across Washington State 

  3️⃣ Predictive Modeling
    * Model Used: Random Forest Classifier.
    * Target Variable: Electric Vehicle Type (BEV vs. PHEV).
    * Features: Make, Model Year, Electric Range.
    * Train/Test Split: 70% / 30%

### 📈 Key Insights
  
  * BEVs dominate EV adoption in Washington State by a wide margin.
  * Most EVs fall into the short to medium electric range, highlighting infrastructure and battery constraints.
  * Tesla leads the market in electric range performance, consistently outperforming other manufacturers.
  * EV adoption increased sharply post-2015, peaking between 2020–2025.
  * King County (Seattle area) shows the highest EV penetration, indicating strong urban adoption patterns.
  * Machine learning can reliably classify EV types using basic vehicle attributes.

### 🚀 Future Enhancements

  * Generalize the model using multi-state EV datasets.
  * Predict electric range (regression) instead of EV type.
  * Integrate charging infrastructure data.
  * Deploy insights via an interactive dashboard (Tableau / Power BI)
