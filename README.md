Covid impact on Service Industries in Finland (detail analysis): -
1.	Data Collection: - Web Scrapping from Statistics’ Finland web pages.
2.	Link: - https://stat.fi/en/statistics/documentation/plv#Source%20data%20and%20data%20collections
3.	Data Name: - Turnover of Service Industries (10 Years Data taken to analyze)
4.	Data Preparation with power query
5.	Data upload in Power BI
6.	Created New measures by using DAX
7.	Data Visualization
8.	Dashboard preparation.
9.	AI help to generate following DAX functions.


DAX functions used: -

1.	COVID Drop = CALCULATE(AVERAGE('ServiceIndustry1'[Turnover_Index]), 'ServiceIndustry1'[Year] = 2020) - CALCULATE(AVERAGE('ServiceIndustry1'[Turnover_Index]), 'ServiceIndustry1'[Year] = 2019)
2.	Period = IF('ServiceIndustry1'[Year] < 2020, "Pre-COVID", IF('ServiceIndustry1'[Year] = 2020, "COVID Year", "Post-COVID"))
3.	Recovery Rate = CALCULATE(AVERAGE('ServiceIndustry1'[Turnover_Index]), 'ServiceIndustry1'[Year] = 2024) - CALCULATE(AVERAGE('ServiceIndustry1'[Turnover_Index]), 'ServiceIndustry1'[Year] = 2020)


Insights to Highlight
1. Industries most affected by COVID (e.g., Accommodation and food services)
2. Industries that recovered quickly (e.g., Computer programming)
3. Industries that were relatively unaffected
4. Relationship between volume and turnover changes


   
<img width="1222" height="961" alt="OverallAnalysis" src="https://github.com/user-attachments/assets/e005db46-a7f5-40e3-8151-46e24b6eae45" />
<img width="1216" height="974" alt="DrillThrough" src="https://github.com/user-attachments/assets/e8151724-6495-4be3-a313-a593a6de03d9" />
<img width="1224" height="963" alt="CovidImpact" src="https://github.com/user-attachments/assets/1117802b-2069-4956-b84b-3e2246319f43" />



