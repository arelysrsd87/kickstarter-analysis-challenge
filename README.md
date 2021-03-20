# kickstarter-analysis-challenge
Using Kickstarter dataset we visualize campaign outcomes based on their launch dates and funding goals.
# Kickstarting with Excel

## Overview of Project
Performed analysis on Kickstarter data set to uncover trends based on: 
- Outcomes for theater campaigns based on launch dates 
- Outcomes for play campaigns based on different funding goal amounts

This analysis builds-up on previous results that [theater campaigns in the US](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Theater_Outcomes_US_pie.png) had a 58% sucess rate, and more specifically, [play campaigns in the US](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Play_Outcomes_US_pie.png) had a 68% success rate. Successful theater campaigns had an [average goal amount of $5,049 and average pledged amount of $5,602](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Descriptive%20Statistics%20for%20Successful%20and%20Failed%20theater%20campaigns%20in%20US.png)

### Purpose
The purpose of this project will be to advise Louise if there are any hidden trends based on goals and launch dates for how kickstarter campaigns fare, more specifically, for theater/plays campaigns.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To perform this analaysis, we used Pivot Tables and graphs to visualize campaign outcomes based on launch dates. 
- We added a filter for theater campaigns and the year campaigns were launched. 
- We looked at launch dates as a function of count of outcomes. 
- Launch dates were grouped by month to give a more comprehensive picture on how theater campaigns performed based on their launch date. 
- We filtered out live theater campaigns. 
- Note - these results were not filterd by country.

![Theater_Outcomes_vs_Launch](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
To perform this analysis, we used the COUNTIFS function and percentages for successful, failed and canceled play campaigns based on the funding goal amount. A line graph was created to help visualize the results.
- We set dollar-amount goal ranges so projects can be grouped based on their goal.  
- We counted the number of isntances a campaing was successful, met a certain goal-amount range and play was the subcategory. 
- The same function was applied to failed and canceled play campaigns. 
- We added the total number of projects for each goal range.
- The count number was converted to percentage to standarize the results.
- The percentage of successful, failed and canceled play campaigns as a funtion the goal-amount ranges was graphed using a line graph.
- Note - these results were not filtered by country.

![Outcomes_vs_Goals](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
A challenge could be be errors introduced to the COUNTIFS equation's syntax, as the number of criteria increases. To overcome this, we reccomend adding the number of succesful, failed and canceled play campaigns. Compare the results to a pivot table that filters out plays as a subcategory and looks at each of the outcomes and count of outcomes.

![COUNTIFS_syntax_verification](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/COUNTIFS_syntax_verification.png)

## Results

- The Theater Outcomes Based on Launch Date graph showed successful campaigns had more fluctuations, whereas failed campaigns had less fluctuantions. Overall, most successful campaigns were launched between May-June, while tapering off wowards end-of year. 
 
- The Outcomes Based on Goal graph showed play campaigns with a goal of less than $5,000 had a success rate of 73%. 

### What are some limitations of this dataset?
One limitation of this dataset is the condational formatting based on color for the percentage funding results. The purpose of the condital formatting based on color is to help visulaize which projects were fully funded at a glance. In this intance, we have a couple of successful campaigns with a $1 goal, skewing our results for percentage funded. We recommend filtering out campaigns with unrealistic low goals and applying the conditional formatting again.  

### Possible tables and/or graphs that we recommend are: 
- Play outcomes based on campaign duration indicated 70% of successful play campaigns lasted between 1-45 days. 61% of failed play campaigns lasted between 61-75 days.
---
![Play_Outcomes_vs_Campaign_Duration](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Play_Outcomes_vs_Campaign_Duration.png)
- Average donations descriptive statistics indicated successful campaigns average donations were $93, whereas failed campaigns average donation were $50. 
---
![Average_Funded_Descriptive_Statistics](https://github.com/arelysrsd87/kickstarter-analysis-challenge/blob/main/Average_Funded_Descriptive_Statistics.png)
