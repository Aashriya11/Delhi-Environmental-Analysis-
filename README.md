# Data Environmental Analytics
**✨ Turning Delhi’s environmental data into actionable insights (2021–2024) ✨**
                  
This project, Data Environmental Analytics, leverages **Power BI** to provide a comprehensive analysis of Delhi’s environment using **interactive dashboards**. The objective is to monitor, visualize, and understand key environmental indicators that directly impact urban sustainability, public health, and policy-making.

---

## 1.	Introduction

The Data Environmental Analysis project brings Delhi’s changing environment to life through interactive Power BI dashboards, focusing on the crucial years 2021 to 2024. By combining authentic datasets from government sources, this project provides a 360° view of Delhi’s environment, people, and growth.

The analysis is showcased across four dashboards:
1.	**Climate & Air Insights** – Track air quality, temperature shifts, and rainfall patterns.
2.	**Population Overview** – Explore trends in population, birth rate, and death rate.
3.	**Land & Water Overview** – Understand land usage, vegetation cover, and water body distribution.
4.	**Infrastructure Growth** – Visualize how Delhi’s infrastructure has expanded in recent years.

By narrowing in on 2021–2024, this project highlights short-term shifts that reflect broader environmental and urbanization challenges—offering valuable insights for sustainability, planning, and decision-making.

![image alt](https://github.com/Aashriya11/Delhi-Environmental-Analysis-/blob/8a3b80aa6d3e3be4f45106ecd296ea212275d214/Dashboard.JPG)

---

## 2. Source of Dataset

The datasets used in this project were collected from reliable government and open data platforms to ensure accuracy and credibility. The data primarily covers the years 2021 to 2024 and includes the following:

* **Climate & Air Data**-
 [Delhi Rainfall Data](https://www.iari.res.in/bms/daily-weather/),
 [Temperature Data](https://data.opencity.in/dataset/daily-temperature-70-years-data-for-major-indian-cities),
 [Pollution Concentration](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2089055) 

* **Population Data**-
 [Birth Rate & Death Rate](https://des.delhi.gov.in/sites/default/files/inline-files/annual_report_2023.pdf),
 [Population Estimates](https://statisticstimes.com/demographics/india/delhi-population.php)

* **Land & Water Data**-
 [Land Coverage](https://en.wikipedia.org/wiki/List_of_districts_of_Delhi),
 [Vegetation Index](https://forest.delhi.gov.in/forest/recorded-forest),
 [Water Bodies](https://www.data.gov.in/resource/state-wise-data-first-census-water-bodies-delhi)

* **Infrastructure Data**-
 [Infrastructure Growth](https://delhiplanning.delhi.gov.in/sites/default/files/Planning/economic_survey_of_delhi_2023-24_english.pdf)

---

## 3.	Data Pre-processing Process

To prepare the datasets for analysis in Power BI, several pre-processing steps were applied to ensure data consistency, accuracy, and readiness for visualization. The key steps include:

### 1. Merging Queries
*	Combined multiple datasets using Merge Queries in Power Query.
*	Integrated rainfall, pollution, temperature, and other datasets into unified tables for better relational modeling.

### 2. Data Cleaning
*	Deleted duplicate rows across datasets to avoid double counting.
*	Rectified errors (e.g., invalid dates, negative values in population/rainfall fields).

### 3. Column Management
*	Removed unnecessary or irrelevant columns to reduce dataset size and focus only on analysis-relevant fields.
*	Renamed column into clear, user-friendly labels for better understanding and visualization (e.g., Pop_Growth → Population Growth).
*	Created a Custom Column in Power Query using the function `Text.Proper([District Name])` to convert district names into proper case (e.g., NORTH EAST → North East) for better readability in the dashboards.

---

## 4.	Data Feature Engineering 

Beyond cleaning and preparing the raw datasets, a few new features were engineered to enrich the analysis and provide deeper insights:

### 1.	Date Hierarchy Creation
*	Extracted Year, Month, and Day from raw date fields.
*	Built a proper date hierarchy (Year → Month → Day) to enable trend analysis and drill-down in dashboards.

### 2.	Season Classification
Added a new Seasons column derived from Month values to group data into meaningful seasonal patterns:
*	Winter: December – February (12–2)
*	Summer: March – May (3–5)
*	Monsoon: June – September (6–9)
*	Autumn: October – November (10–11)

---

## 5. Data Analysis

### Dashboard 1: Climate & Air Insights

1. **Air Pollutant Concentration (2021–2024)**
- Pollutant levels peak mainly in *November and December*, with *PM10* and *PM2.5* dominating.  
- *2021* recorded the highest pollution.  
- *2022–23* showed slight improvement before rising again in 2024.  

2. **Rainfall & Temperature**
- Rainfall is highest in *July*, followed by *August and September* (monsoon).  
- Average temperature peaks in *June–July*, then decreases after monsoon.  
- Winters (*Nov–Jan*) have the lowest rainfall and cooler temperatures.  

3. **Temperature by Months**
- Maximum temperature: ~*39.4°C* in June (hottest).  
- Minimum temperature: ~*7–8°C* in Jan & Dec (coldest).  
- Average temperature follows a *bell-shaped curve*, peaking in summer, dipping in winter.  

4. **Average AQI by Years**
- Highest average AQI: *2022 – 209.03* (poor air quality).  
- Lowest average AQI: *203.63*.  
- Overall, AQI remains in the *unhealthy range* across years.  

---

### Dashboard 2: Population Overview

1. **Life Expectancy**  
   - Females live longer than males.  
   - Population increases by ~*0.4M per year*.  

2. **Share % of Delhi in India & Growth Rate**  
   - 2021: Delhi contributed **1.51%** of India’s population, growth rate *1.89%*.  
   - 2024: Share increased to *1.56%*, but growth rate declined to *1.833%*.  
     **Insight:** Delhi’s share is rising, but growth is gradually slowing.  

3. **Birth & Death Rate**  
   - Highest *birth rate*: 2023 (*315,087*).  
   - Highest *death rate*: 2021 (*171,476*).  

4. **Average Registered Births & Deaths**  
   - Average daily *births > deaths*, showing *positive natural population growth*.  

---

### Dashboard 3: Land & Water Overview

1. **Area Distribution**  
   - Largest: *North West Delhi* (443 sq. km).  
   - Smallest: *Central Delhi* (25 sq. km).  

2. **Population Distribution**  
   - Highest: *North West Delhi* (3,651,261).  
   - Lowest: *Shahdara* (322,931).  

3. **Forest Cover**  
   - 3 main zones: *South, West, North*.  
   - Largest: *South Forest* (82.14 sq. km in South Delhi).  

4. **Water Bodies**  
   - Maximum found in *South West Delhi*.  

---

### Dashboard 4: Infrastructure Growth

1. **Per Capita Income Growth**
- Fluctuated: *-9% (2020–21)* → Peaked *17% (2021–22)* → Declined in following years.  
- Similar patterns in *NSDP & GSDP*, indicating need for balanced sector investments.  

2. **Sector-wise Priority in Expenditure**
   
   | Year       | Most Prioritized Sectors            | Least Prioritized Sectors              |
   |------------|-------------------------------------|----------------------------------------|
   | 2020–2021  | Education, Water Supply & Sanitation| Energy, Development & Food Control     |
   | 2021–2022  | Transport & Education               | Development & Food Control, Others     |
   | 2022–2023  | Transport & Education               | Development & Food Control, Others     |

   Delhi Govt. consistently prioritizes *Transport & Education*, while *Development & Food Control* remain least funded.  

3. **Sector-wise Growth**
   
   | Year       | Best Performing Sectors                                      | Worst Performing Sectors       |
   |------------|--------------------------------------------------------------|--------------------------------|
   | 2020–2021  | Mining & Quarrying                                           | Trade, Hotels, Transport, etc. |
   | 2021–2022  | Construction                                                 | Mining & Quarrying             |
   | 2022–2023  | Trade, Hotels, Transport, Communication & Broadcasting       | Mining & Quarrying             |
   | 2023–2024  | Public Administration, Defence & Other Services              | Manufacturing                  |

---

## 6.	Conclusion
 
The Data Environmental Analysis project provides a holistic view of Delhi’s environmental and demographic landscape between 2021–2024. Through four dashboards – Climate & Air Insights, Population Overview, Land & Water Overview, and Infrastructure Growth – the study highlights key findings:

* Air quality remains consistently unhealthy, with PM10 and PM2.5 dominating, especially during winter months (Nov–Dec).
*	Rainfall is concentrated in the monsoon season (July–Sept), while summers peak at ~39°C and winters dip to ~7–8°C, reflecting Delhi’s extreme climate cycle.
*	Delhi’s population is growing steadily by ~0.4M per year, with births outnumbering deaths, and its contribution to India’s population has increased from 1.51% in 2021 to 1.56% in 2024.
*	North West Delhi leads in both area (443 sq. km) and population (3.65M), while Central Delhi is the smallest district.
*	South Forest covers the largest forested area, and South West Delhi contains the most water bodies, underscoring spatial variations in natural resources.
*	Delhi Government expenditure shows consistent focus on Transport and Education, whereas Development & Food Control sectors remain least funded. However, growth performance varies across sectors, with Construction (2021–22) and Public Administration (2023–24) performing well, while Mining and Manufacturing lag.

Overall, the dashboards reveal that Delhi is undergoing rapid urbanization, population pressure, and environmental challenges, with imbalances between development and sustainability.

---

## 7.	Future Scope

*	Forecasting future weekly sales using time series models
*	Migrating dashboards to Power BI or Tableau
*	Analyzing the impact of promotions and events
*	Adding location-based insights using geographic data
*	Expanding to product-level (SKU) sales analysis
*	Integrating machine learning for clustering and predictions
*	Automating dashboard refresh and report generation
*	Enabling real-time data streaming and live dashboards

---

## 🙏 Acknowledgments
Special thanks to **NovaNectar Services Pvt. Ltd.** for mentorship and guidance. Data sourced from CPCB, IMD, Delhi Govt., and open data portals.  

---

## 🔗 Connect
Feel free to connect for collaboration, reviews, or suggestions to enhance this project further.

