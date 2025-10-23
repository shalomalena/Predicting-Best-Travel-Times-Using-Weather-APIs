# Weather-Based Travel Prediction Analysis

## Project Overview
This project analyzes historical weather data to predict the best times to travel to major U.S. cities.

## Goal
Identify the optimal months to visit 10 U.S. cities based on temperature, precipitation, and humidity patterns.

## Dataset
- **Source:** Open-Meteo Historical Weather API
- **Time Period:** January 2022 - December 2023 (2 years)
- **Cities:** Austin TX, Miami FL, Seattle WA, Denver CO, Boston MA, Phoenix AZ, Chicago IL, Portland OR, Nashville TN, San Diego CA
- **Records:** 7,300+ daily weather observations
- **Variables:** Date, Temperature (High/Low), Precipitation, Humidity

## Technologies Used
- **Python** - Data collection and analysis
- **SQL** - Data querying and aggregation
- **pandas** - Data manipulation
- **matplotlib & seaborn** - Data visualization
- **API Integration** - Real-time weather data collection

## Key Findings
- **Best Overall:** San Diego (July - 55 ideal days)
- **Winter Travel:** Miami, Phoenix, Austin
- **Summer Travel:** San Diego, Seattle, Portland
- **Fall Travel:** Denver, Nashville, Boston

**Ideal Weather Criteria:**
- Temperature: 65-80°F
- Precipitation: < 0.15 inches/day
- Humidity: < 70%

## Files
- `weather_data.csv` - Raw weather data
- `main.ipynb` - Jupyter notebook with all analysis code
- `travel_analysis_summary.txt` - Final recommendations

## How to Run
1. Open `main.ipynb` in Google Colab or Jupyter Notebook
2. Run all cells in order
3. View visualizations and analysis results

## Skills Demonstrated
- API integration and data extraction
- Data cleaning and preprocessing
- SQL queries (GROUP BY, WHERE, aggregations)
- Exploratory data analysis (EDA)
- Statistical analysis
- Data visualization
- Predictive modeling
"""

