# Workplace Absence Analysis

## Overview
This project analyzes employee absence data from 2015 to 2018, focusing on identifying patterns to distinguish between legitimate and fraudulent absences. The goal is to minimize future absence hours by understanding key factors contributing to absenteeism.

## Dataset
- **Absence Reasons**: Classified based on the ICD into 21 categories.
- **Categorical Features**: "Education Level," "Disciplinary Incident," "Social Drinker Status," and "Social Smoker Status" have been transformed into categorical format.
- **Date Handling**: The "Date" feature has been converted to timestamps, and individual day, month, and year features have been extracted.

## Preprocessing
- Handle null and duplicate data.
- Convert date features and drop the original "Date" column.
  
## EDA (Exploratory Data Analysis)
1. **Most Frequent Absence Reasons**: Bar plot to analyze the top 3 frequent reasons.
2. **ICD Classification**: Introduced a binary "Disease" variable to distinguish between absence due to illness and other reasons.
3. **Alcohol/Smoking Impact**: Violin plot to assess absence hours across drinkers and smokers.
4. **Distance & Transport Costs**: Joint plot to analyze the relationship between distance to work, transport costs, and absence hours. Apply Yeo-Johnson transformation to normalize skewed distributions.

## Further Analysis
- **Correlation Matrix**: Use a heatmap to explore correlations between features.
- **Age Analysis**: Displot to observe age distribution, violin plot to compare age and illness, and bar plot to check if older employees have more absence hours.
