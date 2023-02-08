# Canada’s Disaster Database Analysis
#### _A Data Analysis Project using SQL, Visual Studio, PowerBI, and MS Excel Forecast and Monte Carlos Simulations_
_This is a report on the Assignment submitted as one of the Credit coursework for the Southern Alberta Institute of Technology SAIT’s Diploma program in Data Analytics._

This project analyzes the Canada’s disaster database that store information on natural disasters and man-made incidents that have occurred since 1900. 
The analysis is divided into **different stages**, starting with the _Business understanding, Data Understanding, Data Preparation through ETL, SQL SSMS, SSIS, PowerBI Modelling, and MS Excel functions application.

## Business Understanding
The Canadian Disaster Database (CDD) contains information on over one thousand natural and human-made disaster events that have occurred in Canada and abroad since 1900 and that have affected Canadians directly. The data in the CDD can be used across a breadth of fields and industries to support research and inform decision-making.
 
## Data Understanding
One of the critical stages of any Data analysis project is understanding the available data, and the relationships that exists between the various business concepts. The publicly accessible database provides details on each disaster, such as the date and location, the number of evacuations, injuries and fatalities, and the estimated costs.
The following questions will be addressed:
Question 1: How many natural disasters have occurred since 1900? Organize the disaster by event.
Question 2: How many fatalities have occurred since 1900? Organize the fatalities by event. 
Question 3: What is the estimated cost of disasters since 1900? Organize the disaster by event and provide a subtotal of the disasters per year. 
Question 4: What percentage of all disasters (100%) were human-made? 
Question 5: What is the next forecasted natural disaster? 
Question 6: When is the next forecasted human-made disaster? 
Question 7: Run 1,000,000 simulations for disasters.

## Data Preparation
This stage involved Data Extraction, Transformation and Load **(ETL)**. Steps carried here include data wrangling and manipulation, use of SQL Server Import and Export Wizard to load the dataset into SQL Server management studio **(SSMS)**, and use of Visual studio integration services **(SSIS)** to create a Dimensional model with Dimensions and Facts.
In **SSMS**, I set the Primary key **(PK)** column for each Dimension table, telling the software which column to use as PK. Next, I defined the relationships between each Dimension table PK and corresponding Foreign Key in my Fact table. Afterwards the database diagram was generated.

## Visualization & Deep Dive
The first business questions askes How many natural disasters have occurred since 1900. 859 Natural disasters have occurred. Organizing by event, there are 20 possible categories of natural disasters ranging from avalanche, cold event, drought, to tornado, volcano, wildfire and winter storm. The top 5 contributing event to natural disasters are flood, storms, wildfire, winter storm, and drought.

![1 natural disatsers](https://user-images.githubusercontent.com/114383545/217646551-4132cecc-cc9b-4b1a-b5cf-0517e5483355.png)

Visuals for the second business question shows that 63,478 Fatalities have occurred since 1900. 55,642 fatalities were caused by natural disaster, while 7,836 was caused by man-made incidents. Epidemic has contributed the most to the number of fatalities at 50,599, while the second highest contributor is marine event, at 3,531 fatalities.

![2 fatalities](https://user-images.githubusercontent.com/114383545/217646631-20a6888f-d824-47bb-b9f8-adef50663a58.png)

For the third business question, the Cost of disasters since 1900 stands at C$25billion. The highest contributor to the cost was flood incidents (estimated cost = C$8.5million), followed by wildfire (estimated cost = C$5.7million).


The most expensive year for disasters in Canada was 1998, with a cost of C$4.7billion, followed by year 2016, 2013, 2010, and 2011, with estimated cost C$4.1billion, C$3.6billion, C$2.6billion, and C$1.4billion respectively.

![year totals](https://user-images.githubusercontent.com/114383545/217656730-70602f97-a431-43c2-8022-2837b58cb43c.png)

For the fourth business question, visuals show that 21.12% of all events was human-made (incident).

![4a percent manmade incident](https://user-images.githubusercontent.com/114383545/217646727-2618be47-b1db-4912-81b1-8a730ee7d6b8.png)

The two event categories that contribute to human made incident are technology and conflict. Conflict contributed 11.30% and Technology 88.70%. 

![4b breakdown of manmade incident](https://user-images.githubusercontent.com/114383545/217646765-eacf34c1-a270-4714-b17a-3207976c66a9.png)

By subgroup category, the highest contributor to fatality was Meteorological (72.45%), and the least hijacking (0.09%)

![subgroup fatalities](https://user-images.githubusercontent.com/114383545/217656812-d01dafe1-1804-4c5c-8721-3d383ee70834.png)
