# Road Accidents Analysis

## Table of Contents

- [Project Overview](#project-overview)
- [Tools](#tools)
- [Data Analysis](#data-analysis)
- [Recommendations](#recommendations)

### Project Overview

This project explores the analysis of road accidents. Our objective is to identify patterns, provide evidence-based recommendations, and attain an in-depth understanding of road accidents by examining various aspects of their causes. This involves investigating factors such as the condition of road surfaces, types of vehicles, classifications of roads, weather conditions, and the severity of casualties.

<img width="776" alt="Road accidents" src="https://github.com/IanLiam/Road_Accidents_-Tableau-/assets/117744677/f6ff1c9e-6c93-47ab-b267-fef0c0e6e0e1">


### Data Sources
The dataset utilized for this analysis is the "Road_accidents.csv" file, which comprises comprehensive details.

### Tools
- Excel - Data Cleaning  [Download here](https://www.microsoft.com/en-us/microsoft-365/download-office)
- Python - Data Cleaning  [Download here](https://www.anaconda.com/download)
- SQL Server - Data Analysis [Download here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)
- Tableau - Creating reports  [Download here](https://www.tableau.com/community/public)
  
### Data cleaning/ Preparation
In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting.

### Exploratory Data Analysis
EDA involved exploring the road accidents data to answer key questions, such as:

- What type of vehicle has the highest number of casualties?
- Which type of roads have the highest number of casualties?
- Which locations have the highest casualty count?

### Data Analysis
Features worked with:

1. SQL
```sql
-- Selecting with a condition
SELECT * FROM road_accidents;
```

2. Python
```python
# Transposing data
import pandas as pd

# Replace 'input.csv' with the path to your CSV file
input_file = r'C:\Users\ian.muthengi\Downloads\road_accidents.xlsx'

# Read the CSV file into a pandas DataFrame
df = pd.read_excel(input_file)

# Transpose the DataFrame
df_transposed = df.transpose()

# Replace 'output_transposed.csv' with the desired output file name
output_file = 'C:/Users/ian.muthengi/Downloads/transposed_road_accidents.xlsx'

# Write the transposed DataFrame to a new CSV file
df_transposed.to_excel(output_file, index=True, header=False)
```
### Results/Findings
The analysis results are summarized as follows:

1. Private cars have the highest number of casualties.
2. Single carriageways have the highest number of casualties.

### Recommendations
Based on the analysis, we recommend the following actions:

1. Advocate for stricter safety regulations and regular vehicle inspections to ensure all private cars meet high safety standards.
2. Implement more comprehensive driver education programs focusing on defensive driving techniques, awareness of road safety, and adherence to traffic laws.
3. Invest in improving road conditions, including better signage, road markings, and lighting, as well as the design and maintenance of safer roadways.
4. Conduct detailed safety assessments of high-casualty locations to identify specific risk factors contributing to accidents.

### Limitations
The accident data often lacks detailed context, such as road conditions, driver behaviors, and environmental factors, which are crucial for a comprehensive analysis of the causes and consequences of accidents.
