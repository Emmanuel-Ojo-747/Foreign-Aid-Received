# Inequality in Education Around the World

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Recommendations](#recommendations)


### Project Overview
---

This data analysis project aims to uncover the story of educational inequality across the globe by analyzing trends, comparing regions, and exploring the factors that may contribute to disparities. Over the period from 2010 to 2021, we are investigating how inequality in education has evolved in different countries and regions, with a special focus on identifying who is being left behind and why some areas experience greater inequality than others.


### Data Sources
---

The primary dataset used for this analysis is the "Inequality in Education Around the World.csv" file, containing historical data covering a range of indicators pertaining to educational inequality on a global scale. The dataset's prominent components include: ISO3, Country, Human Development Groups, UNDP Developing Regions, HDI Rank (2021), and Inequality in Education spanning the years 2010 to 2021.

### Tools
---


- Microsoft Excel - Data Preparation and Cleaning 
    -[Download here](https://microsoft.com)
- Python - Data Analysis
- Plotly.js - Data Visualization
- HTML - Dashboard Development


### Data Cleaning and Preparation
---

In the Initail data preparation phase, the following task were pweformed:
1. Data loading and Inspection
2. Handling missing values
3. Data cleaning and formatting

### Exploratory Data Analysis
---

EDA Involved exploring the Inequality in Education Data to answer key question, such as:

- Is there a correlation between a country’s HDI rank and its educational inequality in 2021?
- Which regions and countries experienced the highest or lowest educational inequality in 2021?

![newplot (1)](https://github.com/user-attachments/assets/9de659fe-cfdf-4d69-8d9f-ba6042f302ee)


![newplot (2)](https://github.com/user-attachments/assets/c5437101-2735-4133-9dad-9b9d121336c2)


### Data Analysis
---

```Python
import pandas as pd

data = pd.read_json('inequality_data.json')  # Load the JSON dataset
average_inequality = data.filter(like='Inequality in Education').mean()  # Calculate the average inequality per year
print(average_inequality)  # Display results for each year (2010-2021)
```

### Results/Findings
---

The analysis results are summarized as follows:

1. Countries with higher HDI ranks (lower development) tend to have higher educational inequality.
2. Sub-Saharan Africa and South Asia displayed the highest regional inequality in education, with countries like Niger, Chad, and Pakistan consistently ranking at the top.

### Recommendations
---

Based on the analysis, we recommend the following:

- To reduce disparities, target educational interventions in low-HDI countries with high inequality, such as Niger, Chad, and South Sudan, should be prioritized. This includes investments in infrastructure, rural schools, teacher training, and programs that improve education access.
- Policymakers should address non-economic barriers to educational equality in middle- and high-HDI countries like India and Brazil, where inequality persists due to gender gaps, rural-urban divides, and systemic discrimination.
- Encouraging regional collaboration to address common challenges in regions like sub-Saharan Africa can help countries share best practices and successful education reforms.
- Countries must monitor and evaluate progress using tailored metrics that go beyond general HDI scores, including measures for gender-specific, rural vs. urban, and marginalized group disparities.

### References
---

1. Plotly for data analysis and visualization

😄
💻
