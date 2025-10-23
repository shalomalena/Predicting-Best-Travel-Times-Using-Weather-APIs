
# Predicting Best Time to Travel: Weather-Based Analysis & ML Model

##  Project Summary
A data-driven project that uses historical weather data and machine learning to predict the optimal travel times for 10 major U.S. cities. Combines API integration, SQL analysis, predictive modeling, and interactive visualizations.

##  Business Problem
Travelers want to visit cities during ideal weather conditions but lack data-driven insights. This project analyzes 2 years of weather patterns to recommend the best months for travel based on temperature, precipitation, and humidity.

## Technical Approach

### 1. Data Collection via API
- **Source:** Open-Meteo Historical Weather API
- **Method:** Python `requests` library for API calls
- **Data Retrieved:**
  - Daily temperature (high/low)
  - Precipitation levels
  - Humidity percentages
  - 730+ days per city across 2022-2023

### 2. Data Cleaning & Preprocessing
- Converted JSON API responses to pandas DataFrame
- Handled missing values and standardized formats
- Created derived features: month, day of year, travel score
- Final dataset: 7,300+ clean records

### 3. Exploratory Data Analysis (EDA)
- **SQL Queries:** Aggregated data by city and month using pandasql
- **Statistical Analysis:** Calculated means, medians, and distributions
- **Pattern Recognition:** Identified seasonal trends and optimal conditions
- **Visualization:** Line plots, heatmaps, and bar charts using matplotlib & seaborn

### 4. Machine Learning Model
- **Algorithm:** Random Forest Regressor (scikit-learn)
- **Target Variable:** Travel Score (0-100 scale)
- **Features:** City, month, day of year, temperature, precipitation, humidity
- **Performance:** 
  - Mean Absolute Error: ~X points
  - R² Score: ~X
- **Output:** Predicts travel suitability for any city/date combination

### 5. Key Visualizations
- **Temperature Trends:** Line charts showing seasonal patterns across cities
- **Heatmap:** Monthly ideal weather days by city
- **Precipitation Comparison:** Rainfall patterns throughout the year
- **Model Performance:** Actual vs. predicted score scatter plot

##  Key Findings

### Top Travel Destinations by Season:
- **Summer:** San Diego (July - 55 ideal days), Seattle (July - 40 days)
- **Fall:** Denver (October - 27 days), Nashville (October - 26 days)
- **Winter:** Phoenix (November - 37 days), Miami (January - 22 days)
- **Spring:** Austin (March - 19 days), Boston (May - 21 days)

### Climate Insights:
- **Ideal Weather Criteria:** 65-80°F, <0.15" precipitation, <70% humidity
- **Most Consistent:** San Diego (year-round pleasant weather)
- **Best Value:** Phoenix (37 ideal days in November alone)
<img width="655" height="315" alt="my screenshots 2025-10-23 at 11 21 15 AM" src="https://github.com/user-attachments/assets/d4a39a54-292d-44b0-abb0-f3e44a8a4818" />
<img width="645" height="375" alt="my screenshots 2025-10-23 at 11 21 04 AM" src="https://github.com/user-attachments/assets/c48f662c-452b-4d89-be73-6e4155b4ea07" />
<img width="648" height="371" alt="my screenshots 2025-10-23 at 11 20 52 AM" src="https://github.com/user-attachments/assets/e5915103-9bc6-4435-8a01-ecaca63fe4f1" />
<img width="651" height="408" alt="my screenshots 2025-10-23 at 11 21 29 AM" src="https://github.com/user-attachments/assets/d9321927-b751-4eeb-9461-1c1d6d56b0b1" />

##  Technologies & Skills

**Programming & Libraries:**
- Python (pandas, numpy, scikit-learn, requests)
- SQL (pandasql for data querying)
- Data visualization (matplotlib, seaborn)

**Data Science Skills:**
- API integration & ETL pipelines
- Feature engineering
- Machine learning (supervised regression)
- Model evaluation (MAE, R², feature importance)
- Statistical analysis

**Tools:**
- Google Colab / Jupyter Notebooks
- Git version control

## Project Structure
```
├── weather_data.csv              # Raw historical weather data
├── main.ipynb                    # Full analysis notebook
├── README.md                     # Project documentation
└── travel_analysis_summary.txt   # Business recommendations
```

## How to Run
1. Open `main.ipynb` in Google Colab or Jupyter
2. Install dependencies: `pip install pandas requests pandasql scikit-learn matplotlib seaborn`
3. Run all cells sequentially
4. View analysis outputs and ML predictions

## Business Impact
This analysis enables:
- **Travelers:** Make data-driven decisions on when to visit cities
- **Tourism Industry:** Optimize marketing campaigns by season
- **Travel Agencies:** Provide personalized recommendations
- **Hotels/Airlines:** Understand demand patterns for dynamic pricing

## Learning Outcomes
- Real-world API data extraction
- End-to-end data pipeline (extraction → cleaning → analysis → modeling)
- SQL for data aggregation and filtering
- Machine learning model development and evaluation
- Translating technical findings into business recommendations

## Future Enhancements
- Add flight price data for cost-benefit analysis
- Interactive dashboard (Plotly/Streamlit)
- Expand to 50+ cities globally
- Incorporate hotel prices and tourist attractions
- Deploy as web application
