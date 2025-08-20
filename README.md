# Data Environmental Analytics
**✨ Turning Delhi’s environmental data into actionable insights (2021–2024) ✨**
                  
This project, Data Environmental Analytics, leverages **Power BI** to provide a comprehensive analysis of Delhi’s environment using **interactive dashboards**. The objective is to monitor, visualize, and understand key environmental indicators that directly impact urban sustainability, public health, and policy-making.

---

## 1.	Introduction
The Data Environmental Analysis project brings Delhi’s changing environment to life through interactive Power BI dashboards, focusing on the crucial years 2021 to 2024. By combining authentic datasets from government sources, this project provides a 360° view of Delhi’s environment, people, and growth.

The analysis is showcased across four dashboards:
1.	Climate & Air Insights – Track air quality, temperature shifts, and rainfall patterns.
2.	Population Overview – Explore trends in population, birth rate, and death rate.
3.	Land & Water Overview – Understand land usage, vegetation cover, and water body distribution.
4.	Infrastructure Growth – Visualize how Delhi’s infrastructure has expanded in recent years.

By narrowing in on 2021–2024, this project highlights short-term shifts that reflect broader environmental and urbanization challenges—offering valuable insights for sustainability, planning, and decision-making.

---

## 2. Source of Dataset
The datasets used in this project were collected from reliable government and open data platforms to ensure accuracy and credibility. The data primarily covers the years 2021 to 2024 and includes the following:

**•	Climate & Air Data**-
i	Delhi Rainfall Data – [link](https://www.iari.res.in/bms/daily-weather/)
ii	Temperature Data – [link](https://data.opencity.in/dataset/daily-temperature-70-years-data-for-major-indian-cities)
iii	Pollution Concentration (PM2.5, PM10, NO₂, etc.) 

**•	Population Data**
o	Birth Rate & Death Rate – [link](https://des.delhi.gov.in/sites/default/files/inline-files/annual_report_2023.pdf)
o	Population Estimates – [link](https://statisticstimes.com/demographics/india/delhi-population.php)

**•	Land & Water Data**
o	Land Coverage – [link](https://en.wikipedia.org/wiki/List_of_districts_of_Delhi)
o	Vegetation Index – [link](https://forest.delhi.gov.in/forest/recorded-forest)
o	Water Bodies – [link](https://www.data.gov.in/resource/state-wise-data-first-census-water-bodies-delhi)

**•	Infrastructure Data**
o	Infrastructure Growth – [link](https://delhiplanning.delhi.gov.in/sites/default/files/Planning/economic_survey_of_delhi_2023-24_english.pdf)



## 2.	Data Pre-processing Process
To prepare the datasets for analysis in Power BI, several pre-processing steps were applied to ensure data consistency, accuracy, and readiness for visualization. The key steps include:
1. Merging Queries
•	Combined multiple datasets using Merge Queries in Power Query.
•	Integrated rainfall, pollution, temperature, and other datasets into unified tables for better relational modeling.
2. Data Cleaning
•	Deleted duplicate rows across datasets to avoid double counting.
•	Rectified errors (e.g., invalid dates, negative values in population/rainfall fields).
3. Column Management
•	Removed unnecessary or irrelevant columns to reduce dataset size and focus only on analysis-relevant fields.
•	Renamed column into clear, user-friendly labels for better understanding and visualization (e.g., Pop_Growth → Population Growth).
•	Created a Custom Column in Power Query using the function Text.Proper([District Name]) to convert district names into proper case (e.g., NORTH EAST → North East) for better readability in the dashboards.
