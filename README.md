# Module One Challenge Report

## Overview of the Project
---
Louise’s play Fever came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals. Using the data available, an analysis will be performed by visualizing the campaign outcomes based on their launch dates and their funding goals.

## Analysis and Challenges
---
### Analysis of Outcomes Based on Launch Date
The lunch date was converted from unix timestamp to a readable format, using the following formula =(((J2/60)/60)/24)+DATE(1970,1,1), where J is the column in which the unix timestamp values exist and 2 is the number of the row. After doing that, it possible to know the year of each event. The function __year__ was utilized to creat a column containing the year, to allow for filtration based on the year. Hence, the pivot table was created ant its fields were apointed as illustrated in figure 1. ![Capture 85](https://user-images.githubusercontent.com/59425631/123569538-7bf94f00-d794-11eb-9f0f-599619342ce3.PNG)
  
