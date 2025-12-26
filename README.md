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
  * Source: [U.S. Government Open Data](https://catalog.data.gov/dataset/electric-vehicle-population-data).
  * Dataset: Electric Vehicle Population Data (Washington State).
  * Scope: Vehicle registrations, electric range, MSRP, model year, make, and geographic attributes.

The dataset includes both BEVs and PHEVs, making it suitable for comparative analysis and supervised learning.

### 🧠 Methodology
  1. Data Cleaning & Preprocessing:
      * Loaded and processed using Pandas.
      * Handled missing values to maintain data integrity.
      * Encoded categorical variables (Make, EV Type) using label encoding and one-hot encoding
      * Selected relevant features for analysis and modeling

  2. Exploratory Data Analysis (EDA)
  Key analyses include:
      * Distribution of BEVs vs. PHEVs.
      * Electric range distribution (short, medium, long).
      * Adoption trends over model years.
      * EV penetration by county and city.
      * Manufacturer comparison by electric range.
      * EDA revealed that BEVs dominate the dataset, with significantly higher adoption than PHEVs across Washington State 

  3. Predictive Modeling
      * Model Used: Random Forest Classifier.
      * Target Variable: Electric Vehicle Type (BEV vs. PHEV).
      * Features: Make, Model Year, Electric Range.
      * Train/Test Split: 70% / 30%

### 📊 Data Visualizations & Key Insights

  1. Top 10 EV Manufacturers vs. Electric Range (Scatter Plot).
       * This scatter plot compares electric range distribution across the top 10 EV manufacturers.
       * Tesla clearly dominates the high-range segment, with multiple models exceeding 300+ miles, indicating advanced battery efficiency and consistent long-range offerings.
       * Other manufacturers (BMW, Nissan, Ford, Toyota, Volkswagen) show clustered mid-to-low range values, reflecting either hybrid-heavy portfolios or earlier EV generations.
       * The wide vertical spread for Tesla highlights model diversity, while tighter clusters for other brands indicate limited range variation.
       * Color intensity reinforces that higher electric range vehicles are concentrated among fewer manufacturers, primarily Tesla.
    
![alt text](https://github.com/krishnabisoi/Python_Electric_Vehicle_Dataset/tree/main/Visuals/01 Top 10 EV Manufacturers by Registration Frequency.png)


  2. Top 10 EV Manufacturers by Registration Frequency (Bar Chart)
       * This bar chart shows market dominance by volume, not performance.
       * Tesla overwhelmingly leads EV adoption, with registrations far exceeding all other brands combined.
       * Chevrolet, Nissan, and Ford form a second-tier adoption group, indicating strong but distant competition.
       * Emerging brands (Rivian, Hyundai, Volkswagen) show lower adoption counts, suggesting either newer market entry or niche positioning.
       * The chart confirms that brand presence and consumer trust heavily influence EV adoption, not just technical range.

  3. Distribution of Electric Vehicle Ranges (Short / Medium / Long)
       * EVs are categorized into Short, Medium, and Long electric range segments.
       * The majority of vehicles fall into the Short and Medium range categories, highlighting current battery and cost constraints in mass-market EVs.
       * Long-range EVs represent a very small fraction, indicating that extended range remains a premium feature, not an industry standard.
       * This distribution reinforces the trade-off between affordability and range in the EV market.

  4. EV Adoption Trends Over Time (Model Year Analysis)
       * EV adoption remained negligible before 2010, reflecting early technological and infrastructure barriers.
       * A sharp growth phase begins after 2015, aligning with policy incentives, charging infrastructure expansion, and improved battery technology.
       * Adoption peaks between 2020–2023, showing rapid mainstream acceptance of EVs.
       * The sharp drop in the latest year is likely due to partial-year data, not an actual decline.
       * Overall, the trend confirms that EV adoption follows a non-linear, accelerated growth curve.

  5. Distribution of EV Types (BEV vs. PHEV)
       * Battery Electric Vehicles (BEVs) significantly outnumber Plug-in Hybrid Electric Vehicles (PHEVs).
       * This indicates a clear market shift away from transitional hybrid solutions toward fully electric vehicles.
       * The dominance of BEVs suggests improved charging infrastructure and growing consumer confidence in all-electric mobility.
       * PHEVs remain relevant but appear to serve a narrower, transitional user base.

  6. Location-wise EV Adoption (Pie Chart & Bar Chart)
       * EV adoption is heavily concentrated in urban and suburban regions.
       * King County (Seattle and surrounding areas) accounts for the largest share of EV registrations, reflecting higher income levels, infrastructure availability, and environmental awareness.
       * Other regions show progressively lower adoption, highlighting a clear urban–rural adoption gap.
       * This visualization emphasizes that geography and infrastructure availability are major drivers of EV adoption.

  7. Electric Range Comparison: BEV vs. PHEV (Box Plot)
       * BEVs exhibit a much higher median electric range compared to PHEVs.
       * PHEVs show tight clustering at lower ranges, confirming their reliance on internal combustion engines for extended travel.
       * BEVs display wider variance and multiple high-range outliers, reflecting rapid technological improvements and diverse model offerings.
       * This comparison clearly validates why BEVs dominate long-range EV segments, while PHEVs serve short-distance or transition use cases.


### 🚀 Future Enhancements

  * Generalize the model using multi-state EV datasets.
  * Predict electric range (regression) instead of EV type.
  * Integrate charging infrastructure data.
  * Deploy insights via an interactive dashboard (Tableau / Power BI)
