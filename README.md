# CALL CENTER PROJECT

## Table of Content
[project Analysis](#project-analysis)

[Data Source](#data-source)

[Data Preparation](#data-preparation)

[Data Description](#data-description)

[Data Analysis](#data-analysis)

[Insights](#insights)

[Dashboard](#dashboard)


### Project Analysis


This Power BI project aims to analyze a comprehensive call center dataset with features including Emp ID, Name, Inbound, outbound, Avg call handled, call handled, Total calls, Productivity, managers, process and region. The goal is to gain valuable insights into call center productivity comprising of the managers, the region, and the process productivity. 
Power BI's interactive visualizations will enable drill-down analysis and the ability to slice and dice the data based on various dimensions such as weekend, process, name, manager, region and productivity rating. This will empower call center managers and stakeholders to make data-driven decisions, optimize operations, and enhance customer service.


### Data Source

[Download Here](https://drive.google.com/drive/folders/1SYg550GcP0mdE3kZkMtQ3iJVy1ku3mdl)


### Data Preparation 

Data transformation was done in Power Query and the dataset was loaded into Microsoft Power BI Desktop for modeling.

### Data Description 

The tabulation below shows the Call data table, manager data table and process data table with their column names and  description:

|      Column Name|                                                Description|
|      -----------|                                                -----------|
|      Weekend    |It shows the dates the calls were made                     |
|      Emp Id     |Represents every unique observation in the dataset         |
|      Name       |Describes the name of the agent                            |
|      Inbound    |Describes a call initiated by the customer or prospect     |
|      Outbound   |Describes a call initiated by a call center representative |
| Avg Call handled|Represent the average call time                            |
|    Call handled |Represent the numbers of calls by agent per time           |
|Total Calls      |Represent the sum of inbound call and Outbound call        |
|Productivtiy     |Describes the call handled divided by total calls          |
|Manager          |Describes the name of the manager                          |
|Region           |Represent the country                                      |
|Rating           |Represent the ratings of the calls                         |


### Data Analysis 

The Dax functions used are as follows:

```DAX

Productivity = 'Call Data'[Call handled]/'Call Data'[Total calls]*1

Total calls = 'Call Data'[Inbound]+'Call Data'[Outbound]

```


### Insights

- The total number of customers is 162
- The sum of inbound calls is 2081(31.48%) while the sum of outbound is 4530(68.52%) and the total number of calls is 
  6611.
- The average productivity comes at 82.7%.
- November is the month with the highest total calls having 2208
- Shiva Reddy and Trisha ken are the managers who were recorded to have the highest number of calls
- The most inbound, outbound and total calls  were made in the sales process aspect
- Canada has the highest productivity with 82.7%  
- Canada recorded higher calls in October and December and a lower rate of calls in November , meanwhile India and USA 
 possess the highest call rate in November and lower call rate in October and December.


### Dashboard


![call center dashboard](https://github.com/ADETOLAADEBANJI/CALL-CENTER-PROJECT/assets/149164492/7b61a49a-7363-4037-8067-1d58927ca62e)
















