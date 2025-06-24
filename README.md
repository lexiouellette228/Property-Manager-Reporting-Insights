# Property Manager Reporting & Insights

This project focuses on leveraging data analytics to enhance the efficiency and transparency of rental deposit refund payments. The project analyzes anonymized datasets related to disbursements, recipients, and properties to provide critical financial insights. Key objectives include developing Power BI reports for high-level and granular performance tracking, identifying anomalies such as error spikes or payment expirations, and uncovering geographic and demographic trends impacting payment completion rates Utilizing Microsoft Fabric Lakehouse for data storage, along with SQL and Python for data processing, this project enhances decision-making through automated reporting.

## Data Sets
Our project relied on two datasets: 

- Static data: Disbursements, Recipient Payments, Recipient Feedback, Apartment Names​
- Census Data: Income, Population, Business, Unemployment rates, Education, Housing, Poverty, and Family Demographics ​
- The static data was given by the company as a means of looking into their disbursement refund program. ​
- The census data was collected by us to enable data driven insights into the program with regards to the outside factors listed above. 

---

## Project Files

- `DAX_Formulas`: DAX formulas used in Power BI Desktop to analyze data for visualizations.
- `Education_By_ZipCode.csv`: A CSV file containing cleaned and sorted education level data by zip code from http://census.gov/.
- `Notebook 1`: Python code to create a correlation matrix between median income and disbursement data in Power BI Desktop. 
- `Notebook 2`: Python code to create a scatter plot showing MedianIncome vs Completion/Expiration Rate by IncomeGroup in Power BI Desktop.
- `Notebook 3`: Python code to create a heatmap showing the correlations between median income and disbursement data in Power BI Desktop.
- `Notebook 4`: Python code to create a scatter plot showing Median Income vs Completion & Expiration Rates with Trendlines in Power BI Desktop .
- `Notebook 5`: Python code to create a scatter plot showing the top 5 expiration zip codes and lowest 5 income zip codes in Power BI Desktop. 
- `Notebook 6`: Python code to create a scatter Plot with 2 Y-Variables and Data Point Labels in Power BI Desktop.
- `SQL`: PySpark SQL code to create tables, join tables, and analyze data.
- `income data padded.csv`: A CSV file containing cleaned and sorted income data by zip code from http://census.gov/.
- `FinalReport.pbix`: Final Power BI report containing the entire groups work.

---

## Methods

- Analyzed anonymized datasets covering disbursements, recipients, and properties.​
- Developed dynamic Power BI reports for both high-level and detailed financial tracking.​
- Created virtualization reports.

## Report Screenshots
- `Disbursement_Report.png`: displays a comprehensive dashboard of static data regarding the given apartment complexes. It allows the flexibility of seeing the overall picture and being able to drill down into each state or individual complex. The layout of visuals allows users to navigate the data smoothly. This display also ensures users are only seeing data relevant to their desired level of granularity.
  
- `Insight_Grapg.png`: shows percentage of the different of different types of disbursement status either completed, expired, errored, pending, revoked, in progress, and you can see there is more disbursement are completed than other status. In the card there are total, completed, and non-completed amount  of disbursement and to show that there are more amount of completed disbursement than non-completed disbursement.

- `Correlation.png`: analyzes the correlation between median income and various factors like completion rate, expiration rate, feedback, and housing type (single-party vs. multi-party). It includes a correlation matrix, a dynamic scatter plot with trendlines for income vs. selected metrics, and another scatter plot comparing income vs. party type counts. The insights help determine if income levels are significantly associated with housing and disbursement behaviors.
  
- `Final_Report_1`: visualizes the relationship between education attainment level (% High School Graduate, % Associates, % Bachelors, %Graduate Degree) and disbursement outcomes (% Completed vs. % Expired) across ZIP codes. The combined bar and line chart enables comparison of degree types with disbursement status by location, while filters (income, household size, party type, etc) allow for focused analysis.
  
- `Final_Report_2`:  provides a comprehensive overview of payment activity by apartment over time, showing a total of 3.28 billion in payments across 192K transactions. It breaks down payment trends by month and year, highlights payment vehicle types (ACH, Check, VirtualCard), and shows ACH as the dominant method (~90%). The visuals help monitor volume fluctuations and method preferences across different time periods and apartments.

- `Final_Report_3`: provides a breakdown of disbursements totaling $244.51K, analyzing trends in payment count and total amount by month and year. It includes a pie chart of disbursement status—with 82% marked as complete and 18% as expired—and allows filtering by apartment name, disbursement status, and date. The dual-axis bar and line chart highlights fluctuations in disbursement volume and value over time.
  
- `Final_Report_4`: presents disbursement performance for 2023, showing 18K payments totaling $236.45M. The bar and line chart tracks monthly disbursement volume and total value, with a noticeable spike in November and December. A pie chart shows that 85.1% of funds were successfully completed, while 14.9% expired, helping assess disbursement status by outcome. The graphs are dynamic to the apartment name filter, disbursements type filter, and year filter.
  
- `Final_Report_5`: presents a geographic and categorical overview of 994 apartment properties totaling $3.29 billion in disbursements across 131K transactions. Users can toggle between state and city views to analyze apartment counts, disbursement volume, and status distribution, which is predominantly completed (85.9%). A map visual and detailed table highlight key cities like Brunswick, ME and Los Angeles, CA, while pie charts break down disbursement status by both count and dollar amount.
  
- `Final_Report_6`: presents a dynamic scatter plot showing the relationship between Median Income and a selected parameter, currently set to average feedback score. It includes a selector for metrics like completion_rate, expiration_rate, and party type counts, enabling users to explore how different variables correlate with income. The plot shows that most high feedback scores cluster between $50K–$100K income levels.
  
- `Final_Report_7`: provides a nationwide overview of apartment-related disbursements. It shows 994 apartment complexes with a combined $3.29 billion disbursed over 131K transactions, visualized on a US map by city. Users can filter by state, city, or apartment name, and the disbursement status breakdown shows that nearly 86% of funds are in completed status, with detailed metrics available by location and parameter type.

## Context
- This project is for educational use only. 
