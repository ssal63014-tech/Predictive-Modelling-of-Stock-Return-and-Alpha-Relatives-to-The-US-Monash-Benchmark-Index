# Predictive-Modelling-of-Stock-Return-and-Alpha-Relatives-to-The-US-Monash-Benchmark-Index

## Overview
This project focuses on predicting the monthly relative performance of stocks against the US Monash Index, a custom benchmark representing the broader US equity market. The objective is to estimate the magnitude of excess returns, enabling a deeper understanding of market behaviour and sector dynamics.

The analysis covers 616 US-listed companies across various sectors and market capitalisations, providing a comprehensive view of factors influencing relative stock performance. By leveraging a regression-based approach, the project explores how systematic patterns and financial indicators can be used to generate data-driven insights for investment decision-making.

## Key Findings
- The analysis indicates a significant decline in overall market performance, with predicted excess returns decreasing by approximately 52.78% in July 2023.
- This downturn is primarily driven by sharp corrections in cyclical sectors such as Energy (-80.34%) and Materials (-61.51%), suggesting a strong mean-reversion effect where previously high returns are not sustained.
- The critical sectors including Healthcare (+522.42%) and Utilities (+101.57%) demonstrate substantial recovery, indicating potential resilience during periods of market weakness.
- The platform-based companies, although present in fewer sectors, exhibit more stable and balanced performance with over 60% outperformance, highlighting their scalability and adaptability.

## Data Usage
- `stock_data`: Monthly stock-level data for 616 US companies from 2020 to 2023 (42 months).
- `company_info`: Static company attributes providing detailed business characteristics.
- `monash_index`: A custom benchmark representing the overall US equity market, used to calculate relative performance (excess return) for each stock.
- `macroeconomic instruments`: External economic indicators used to capture global market conditions and their impact on stock performance.

**NOTE**

**Data Availability**: This project uses datasets provided by Monash University for academic purposes.  
The data is not included due to academic integrity and usage restrictions.

## Methodology
1. Data Exploration
    - Performed exploratory data analysis (EDA) to understand data structure, distribution, and initial patterns.
    - Visualised key variables to identify trends, relationships, and sector-level behaviour.
2. Data Preparation
    - Conducted data wrangling to clean and organise datasets.
    - Detected and handled data anomalies, including missing values and outliers.
    - Merged multiple datasets (stock, macroeconomic, and company information) into a unified dataset.
    - Validated data consistency across time-series and identifiers.
3. Data Transformation
    - Created time-series features such as lag features to prevent data leakage.
    - Encoded categorical variables
    - data scaling
4. Model Development
    - Built a predictive pipeline using `Random Forest Regression`.
5. Model Evaluation
    - `Root Mean Squared Error (RMSE)`