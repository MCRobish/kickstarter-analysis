# Kickstarting with Excel

## Overview of Project

### The purpose of this project was to help Louise compare how different fundraising campaigns for plays performed in comparison to their launch dates and to their monetary goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to create the theater outcomes based on launch date chart, a pivot table was added. A filter for the year was added as well as for parent category, which was filtered to theater. The field lists were set up as shown below. 

![Challenge1-PivotTable](https://user-images.githubusercontent.com/105991478/174460599-43c90d7a-7d4f-4b12-986a-05fb49a33f25.png)

A line pivot chart was also added with a title. The pivot chart field buttons were also hidden to keep the chart cleaner for the viewer. The _Theater Outcomes Based on Launch Date_ chart can be seen in the **Results** section below.  

### Analysis of Outcomes Based on Goals
The analysis of outcomes based on goals chart was created by using the COUNTIF function in excel. My formula for the category of  successful play campaigns for less than $1000 is =COUNTIFS(Kickstarter!D:D,"<1000",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays")
Once each COUNTIF Statement was created for the monetary categories, a percentage successful, failed and canceled was calculated. This was done by the formula =ROUND(B2/E2,2) as one example. I set the units for each of these columns to "Percentage" rather than multiplying by 100 in the formula. My final result chart is shown below. 
![Challenge1-outcomesgoalstable](https://user-images.githubusercontent.com/105991478/174460764-0090bab5-d0f2-417f-8fa2-1b65cadee149.png)
Lastly, a line chart was created to visualize the results. This can be seen in the **Results** section below as _Outcomes Based on Goal_.

### Challenges and Difficulties Encountered
Initially on the outcomes based on goals, I did not include "plays" as one of the conditions in the COUNTIF statement, causing my results to appear different from what was shown in the challenge. Another challenge was mainly getting used to the syntax with the github commits and understanding what to include in the analysis summary. 

## Results
### What are two conclusions you can draw about the Outcomes based on Launch Date?
The chart below shows the successful, failed and canceled theater fundraisers from 2009 to 2017 by month. Included in the theater category are plays, musicals, and space fundraising goals. More campaigns were successful in every month than were failed or canceled. Specifically reviewing trends over time, it appear that campaigns launched in late spring and early summer had the highest success levels, with a peak of 111 in the month of May. The average number of failed campaigns in a given month is 41. The highest number of failed campaigns was 52, which also occurred in May. Generally, it appears that the failed and canceled rate are not heavily influenced by time, and there is likely another variable that indicates whether the campaign will not meet the goal. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/105991478/174459918-3d45ad30-744a-4d65-aa4b-0cbe21f443c2.png)

### What can you conclude about the Outcomes based on Goals?
For the chart below, the previous data set was filtered to include only play campaigns in order to better compare to the _Fever_ results. The success and failed rates were compared to the initial fundraising goal. The highest success rates for plays were with the lowest goal categories: Fundraisers with less than $1000 as the goal had a 76% success rate, and fundraisers with the goal from $1000 to $4999 had a 73% success rate. For plays with goals below $40,000, it appears that as the goal increases, the failure rate also increases. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/105991478/174460256-5b70bfd8-911b-44a1-b780-8023bede47e8.png)

### What are some limitations of this dataset?
As the monetary goals increase, the total number of campaigns also decreased. Some of the categories above $40,000 have fewer than 5 results, so it is difficult to conclude whether these represent the population or if a larger sample size would mirror the trends of the campaigns below $40,000. Also, there were no cancelled play projects within this dataset, so conclusions for that result cannot be made. It would be interesting as well to see trend information about how the campaign was launched and its success rate- i.e. primarily a digital campaign versus formalized fundraising events. 
