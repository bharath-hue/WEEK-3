# WEEK-3
🌐 Project Title:
AI-Based Forecasting of CO₂ Emissions per Capita Using Random Forest Regression

🔍 Project Overview:
The accelerating climate crisis demands accurate and proactive tools to understand, predict, and mitigate CO₂ emissions. This project focuses on using machine learning (ML) to model and forecast CO₂ emissions per capita across countries based on socio-economic and environmental indicators.

🎯 Objectives:
Predict a country’s CO₂ emissions per capita using historical development indicators.

Identify the most influential factors affecting emissions.

Use long-term trends to simulate and forecast emissions over the next 20 years.

Provide data-driven insights to support environmental policy, planning, and global sustainability efforts.

🧠 Modeling Approach:
Algorithm Used: Random Forest Regression

Target Variable: CO₂ emissions per capita (in metric tons)

Features Used:

Cereal yield

GNI per capita

Energy use per capita

Urban population %

Protected area %

Population growth rate

Urban population growth rate

FDI as % of GDP

Feature Selection:
Recursive Feature Elimination with Cross-Validation (RFECV) was used to retain only the most impactful predictors.

Hyperparameter Tuning:
RandomizedSearchCV optimized the model using 10-fold cross-validation.

📈 Performance Highlights:
Training CV R² Score: 0.986 (with very low variance)

Testing R² Score: 0.982

Root Mean Squared Error (RMSE): Low, indicating highly accurate predictions

Visual Inspection: Strong linear correlation between predicted and actual CO₂ emissions.

🔮 Future Forecasting (2025–2045):
Countries Selected: India, USA, Pakistan, Russia, New Zealand

Methodology:

Compute Compound Annual Growth Rates (CAGR) for each key feature from 1991–2008.

Simulate growth in features year-by-year for 20 years.

Use the trained model to predict CO₂ emissions based on simulated features.

Output:

Forecasted emissions dataset (CSV format)

Country-wise emissions trend visualization (line plots)

📌 Key Insights:
Developed countries like USA and Russia show declining per capita CO₂ emissions, possibly due to green policies.

Developing nations like India and Pakistan are expected to see a gradual rise in emissions due to industrialization and energy demand growth.

The model emphasizes how economic growth, urbanization, and energy use influence CO₂ emissions.

💾 Technical Stack:
Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, joblib

Model Output: forecasting_co2_emission.pkl (serialized model), forecast_results.csv

✅ Conclusion:
This AI-based forecasting tool demonstrates the power of machine learning in environmental monitoring. By combining robust historical data, advanced modeling techniques, and future simulation, the system enables policymakers and researchers to proactively plan for emissions reduction and support sustainable development.
