# Project Title: HDB Resale Price Prediction

## Overview:
This project aims to address the competitive landscape in the Singapore property market by providing a data-driven solution to predict the resale prices of HDB flats. By leveraging machine learning models, the tool assists property agents with more accurate pricing strategies, enabling them to better serve their clients in a fast-evolving market.

## Problem Statement:
The real estate market in Singapore is rapidly evolving, with disruptors offering lower commission rates and more DIY options. Property agents need more than just experience—they need data. This project aims to help the property agency and agents regain the competitive edge by providing insights based on historical data and machine learning algorithms to predict future trends and prices in the HDB resale market.

## Key Objectives:
1. Empower Property Agents: 
Equip agents with valuable data insights on HDB resale prices.

2. Predict Pricing Trends: 
Use machine learning models to accurately predict future resale prices.

3. Increase Client Satisfaction: 
Provide property agents with a tool to guide clients on pricing, maximizing transaction value.

4. Identify Key Market Factors: 
Understand and highlight important features that influence HDB resale prices.

## Data Analysis:
### Factors Influencing HDB Resale Prices:
- Floor area is the strongest predictor of resale price.
- Proximity to amenities like MRT stations, malls, and schools.
- Significant variance in resale prices across different towns.
- Flat type and model also significantly influence the price, with newer developments often commanding higher values.
- Economic health, such as interest rates, GDP growth, and job market conditions.
- Government policies and cooling measures.
- Supply and demand dynamics.

## Machine Learning Models:
After experimenting with various models, the following top three models were chosen:

|                         | Train RMSE | Test RMSE  | Train R²  | Test R²   | Model Run Time (s) |
|------------------------:|------------|------------|-----------|-----------|--------------------|
| Random Forest Regressor | 16,789     | 26,227     | 0.986     | 0.966     | 52                 |
|   Extra Trees Regressor | 14,894     | 26,421     | 0.989     | 0.966     | 56                 |
|             **XGBoost** | **25,166** | **27,074** | **0.956** | **0.964** | **13**             |

XGBoost was selected among the 3 based on its balance between speed, accuracy, and reliability. It provided consistent performance without overfitting. More details on the modelling and the features selected can be found here:
[View HDB Resale Price Predictive Model](https://github.com/DenzilNg/HDB-Resale-Price-Predictive-Model/blob/main/HDB%20Resale%20Price%20Predictive%20Model.ipynb)

## Key Insights:
1. Location Matters: Towns like Bishan, Woodlands, Bukit Timah, and Choa Chu Kang were highlighted as important predictors for resale price.

2. Flat Features: Factors such as flat type (1-5 rooms, executive units), flat model and floor area play a significant role in determining price.

3. Block Features: Characteristics such as the highest floor in the block also contribute to price prediction.

## Future Improvements:
Additional features such as inflation data, flat direction, school rankings, and demographic purchase data will be considered to improve future predictions. Furthermore, government policy changes and other key amenities like preschools and parks will be integrated into the model.

## App Demo:
The app showcases how property agents can utilize the model to predict resale prices in real-time, assisting clients in making informed decisions. The App can be found here: [View HDB Resale Price Predictive Model App](https://hdb-resale-price-predictive-model-denzilng.streamlit.app/)

## Conclusion:
This tool provides a competitive advantage in the dynamic HDB resale market by equipping property agents with the data-driven insights needed to offer better client service. By focusing on critical features like floor area, flat type, and location, agents can now predict resale prices more accurately and make more informed recommendations to their clients.