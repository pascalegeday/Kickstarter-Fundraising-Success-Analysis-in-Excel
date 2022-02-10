# Kickstarter Analysis - Excel
Analysis of Kickstarter Fundraising Efforts using Crowdfunding Data

## Overview of Project

### Purpose
  * In this analysis we are using raw data from Kickstarter campaigns to analyze several thousand crowdfunding projects in order to visualize any hidden trends that may help Louise figure out why certain campaigns are successful and others are not. 
  * The purpose of this analysis is to help Louise figure out why her play "Fever" came close to its fundraising goal in such a short amount of time. By doing this, we want to compare how other campaigns did in relation to their launch dates and funding goals. This way, we have a better understanding of how these components affect a campaigns success and can adjust future campaigns to have a better probability of success.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
  * The first analysis that I performed was the relationship between the success of campaigns in the "Theater" category to their launch date in the years.
  * First, we need to add a separate column in the Kickstarter sheet and using the YEAR() function to create a filter used in our analysis: 
  
  ![Years Function - Kckstarter Data](https://user-images.githubusercontent.com/94571150/142948005-0ca3e1d1-5031-472b-84a2-1074c8e97754.png)

  * Next, we need to create a pivot table in a new sheet using the filters listed below in their appropriate fields: 
 
  ![Pivot Table - Theater Outcomes by Launch Date](https://user-images.githubusercontent.com/94571150/142947874-fb26f4c6-cd79-4926-8d34-45a774d74a6c.png)
  ![Pivot Table Fields - Theater Outcomes by Launch Date](https://user-images.githubusercontent.com/94571150/142947922-36386c33-6824-4577-a92b-edc74f3441cf.png)

  * Then, we are able to view this pivot table in line graph format and better visualize the relationship between Outcomes and Launch Date: 

    ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/94571150/142946701-ffa18dc2-e957-4cad-8d20-b2c0bebacd6b.png)
    
### Analysis of Outcomes Based on Goals
  * The second analysis that I performed was the relationship between the "goal" amount and the outcome of the campaign.
  * First, we need to create a new sheet with the goal amounts, the number of successful, failed, canceled, and total number of projects and the percentage of each. We can do this using the COUNTIFS() formula and inserting the appropriate criteria to decipher the outcome and goal data by the “plays” subcategory. Below is an example of the criteria for cell B2:
  
![COUNTIFS Formula](https://user-images.githubusercontent.com/94571150/142948602-b5ddeda1-8d72-41de-9812-d33e116f90b8.png)

  * Next, we can create a line graph to visualize this data:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/94571150/142946754-de8e9471-c75d-464d-ac1b-f1a2a210cc36.png)

### Challenges and Difficulties Encountered
  * I encountered some difficulties when inputting the YEAR column. For some reason, when I wanted to copy the formula down the column it kept breaking. I had to go through the column and make sure all cells were filled in with the appropriate year. 
  * A difficulty that could be encountered when inputting the COUNTIFS formula in the "Outcomes based on Goals" sheet, is making sure that each criteria is correct with the right range of "goals." It was a bit tedious to make sure that the goals were filled in correctly for each column so it is important to double-check. 
  * A difficulty that could be encountered in the "Theater Outcomes Based on Launch Date" is double checking that the fields are in the correct areas.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    * The month that launched the most campaigns is May. May is also the month that the most successful Theater campaigns were launched. Thus, May shows to be a good time period to launch this type of campaign that will result in success. 
    * Campaigns launched in December, show a roughly equal amount of successful and failed campaigns. December is also tha month that the smallest amount of campaigns were launched. It may be safe to say that launched campaigns towards the end of the year will result in more failures and less successful campaigns.  
- What can you conclude about the Outcomes based on Goals?
    * We can conclude that the higher the funding goal amount, the less likely any given campaign is to be successful. The campaigns with a set funding goal of $9999 or less, had the highest number of successful campaigns, meaning that Kickstarter does better for campaigns that need less funding. 
- What are some limitations of this dataset?
    * There may be many external factors to why campaigns were successful while others were not. It could be possible to include more information on the "backers" in order to have a clearer picture of why backers chose to back certain campaigns and did not choose others.
- What are some other possible tables and/or graphs that we could create?
    * We could create a graph showing the relationship between how many backers there were in any given campaign and the outcome of that campaign. 
    * We could also create a graph showing the relationship between the country and the outcome. This graph may not be as insightful, but we could at least see in what countries these types of campaigns do well in. 
