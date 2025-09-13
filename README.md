# Analysis-on-Global-Country-Macro-Data-using-ML


# Global Country Macro Dataset – Regression Analysis

## Project Overview
This project analyzes a *global macroeconomic dataset* containing indicators such as GDP, population, unemployment, education, health, and environmental factors across 195 countries.  
The goal is to build *machine learning regression models* that can explain and predict economic performance, enabling cross-country comparisons and insights into long-term global trends.

## Objectives
- Provide standardized and comparable macroeconomic indicators for global analysis.  
- Explore socio-economic, demographic, and environmental factors that influence GDP and related outcomes.  
- Develop regression models and neural networks to predict macroeconomic indicators.  
- Compare model performance and identify key drivers of global inequality and growth.  

## Dataset Details
- *Size:* 195 countries × 35 features  
- *Variables include:*  
  - Categorical: Country, ISO code, capital city, calling code  
  - Numerical: GDP, population, life expectancy, unemployment rate, CO₂ emissions, birth rate, land area, urbanization, tax revenue, etc.  
- *Data Quality:*  
  - No missing values reported  
  - Outliers present in features like GDP, population, and birth rate  
  - Multicollinearity tested using *Variance Inflation Factor (VIF)* → high-VIF variables removed before regression  

## Exploratory Data Analysis
- *Histograms & Pie Charts* – show distribution of key indicators such as life expectancy.  
- *Pairplots & Heatmaps* – highlight relationships between GDP, education, fertility, and health.  
- *Boxplots & Countplots* – display variation and frequency distributions across features.  

*Key Observations:*  
- GDP strongly correlates with life expectancy and education.  
- Higher fertility and birth rates correlate negatively with GDP and life expectancy.  
- Significant inequality exists across countries in terms of wealth, education, and healthcare.  

## Insights
- The dataset reflects *global inequality* in GDP, education, and life expectancy.  
- Health outcomes (infant & maternal mortality, life expectancy) are tied closely to GDP.  
- Education enrollment (primary, tertiary) varies widely across regions.  
- Environmental features (CO₂ emissions, forest area) highlight sustainability challenges.  
- *XGBoost* and *ANN* outperformed other algorithms, with ANN slightly ahead on the R² score.  

*ANN with architecture 6-5-4-3-1 and 500 epochs* achieved the best R² = *0.8297*, slightly surpassing XGBoost.  
- Traditional ensemble methods (Random Forest, Gradient Boosting, Bagging) also performed strongly.  
- The study shows that socio-economic indicators (GDP, education, life expectancy) are the best predictors of development, while fertility and birth rate negatively affect outcomes.
