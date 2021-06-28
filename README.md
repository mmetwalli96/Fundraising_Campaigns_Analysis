# Module One Challenge Report

## Overview of the Project
---
Louise’s play Fever came close to its fundraising goal in a short amount of time. Now, she wants to know how different campaigns fared in relation to their launch dates and their funding goals. Using the data available, an analysis will be performed by visualizing the campaign outcomes based on their launch dates and their funding goals.

## Analysis and Challenges
---
### Analysis of Outcomes Based on Launch Date
The lunch date was converted from unix timestamp to a readable format, using the following formula =(((J2/60)/60)/24)+DATE(1970,1,1), where J is the column in which the unix timestamp values exist and 2 is the number of the row. After doing that, it possible to know the year of each event. The function __year__ was utilized to creat a column containing the year, to allow for filtration based on the year. Hence, the pivot table was created and its fields were apointed as illustrated in the below figure.

![Capture 85](https://user-images.githubusercontent.com/59425631/123569538-7bf94f00-d794-11eb-9f0f-599619342ce3.PNG)

As the pivot table was created, the pivot chart was done as well. From the pivottable analyze tab there is box where you can click on it to creat the chart. the chart type is a line chart with markers. 


### Analysis of Outcomes Based on Goals
The goals were grouped as follows:
- less than 1000
- 1000 to 4999
- 5000 to 9999
- 10000 to 14999
- 15000 to 19999
- 20000 to 24999
- 30000 to 34999
- 35000 to 39999
- 40000 to 44999
- 45000 to 49999
- greater than 50000

the number of successful, failed, and canceled plays were counted using the function __counterifs__. There are three cretieria were used, the first is related to the goal category. As for the second, it is the status of the goal, whether it was successful, failed, or canceled. The last cretieria was to pick the subcategory plays.


### Challenges and Difficulties Encountered
One challenge was how to input the goal group when it is between two values. To solve it, for the case of 20000 to 24999, I input the creteria as less than or equal to 24999, Accordingly it will count all the groups before it, consequently, I substract the sum of the values of the other groups before it from the evalueted number based on the previously mentioned creteria. 

Another one, was finding the appropiate time to the required deliverables. I tried to do whatever can be done when I have the chance to do so. To submit this challenge on time.


## Results
---
### What are two conclusions you can draw about the Outcomes based on Launch Date?

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/59425631/123579816-9b997300-d7a6-11eb-9f73-875dbd7743b3.png)

- Based on the above figure, one deduction is the number of successful theater events peaks at the month of May and decreases afterwards till December. It increases starting from  January. As for the case of failed events it increases throughout the year. Lastly, the canceled occasions are almost constant over the year. 

- Another conclusion is that, the best time to lucnh an event is the begining of the year. As the rate of the increase of successful events is higher compared to the failed ones.

### What can you conclude about the Outcomes based on Goals?
Based on the graph below:
- As the fundraising goal is increasing, the chances of it failing goes up, and there is an adverse relation between the success of the event and its failer. 
- The cancelation percentage was zero all the time. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/59425631/123581126-4317a500-d7a9-11eb-937e-b7cdd187f259.png)

### What are some limitations of this dataset?

### What are some other possible tables and/or graphs that we could create?
- A table presenting the percentage of  successful, failed, and canceled theater events based on the lunch date and its chart.
- A table summerizing the period on which every event was succesfully completed. 
- A graph containing all the parent categories and the number of the successful outcome.  




