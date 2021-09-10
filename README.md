# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends
Performing Chanllenges on Kickstarter data to uncover trends


Overview of Project
Purpose
The purpose of this project is to is to compare the results of fundraising campaigns based on their launch dates and their funding goals. We specifically looked at the trends of theaters and plays to determine the successful, failed, and cancelled campaigns.

Analysis and Challenges
Before diving into the analysis, we can see that the data provided is organized by many different aspects, including the description, status and goal of the campaign, amount pledged, average amount of donation, category and subcategory type, and the dates in which the campaigns began and ended. As mentioned earlier, much of the analysis performed was achieved by filtering the data and looking at simply the theater and play trends.

Analysis of Outcomes Based on Launch Date
For the Outcomes Based on Launch Date, I created a pivot table that filtered the outcomes by category and the launch date. The columns display the status of the campaign, while the row shows the months during the campaign. This allows us to see the total count of successful, failed, and canceled theater campaigns. Below is an image of the pivot table with a filter for the theater category.

Theater Outcomes Pivot Table

Analysis of Outcomes Based on Goals
To analyze the Outcomes Based on Goals, I created a table that retrieved the total number of campaigns based off of certain criteria. In order to retrieve the correct count, the COUNTIFS statement was used. Within this formula, I set multiple criteria, including a range for the desired campaign goal, the specific category, and the outcomes of these campaigns. In this case, we wanted to look at the subcategory, plays.

After I retrieved the number of successful, failed, and canceled campaigns for each goal range, I found the percentages by dividing each sub-total with the overall total. Below is a table that illustrates this analysis.

Play Outcomes Table

Challenges and Difficulties Encountered
One of the challenges that I encountered was forgetting to include a criteria within the COUNTIFS statement. Originally, I thought that filtering the data by plays would automatically become a criteria for the chart. However, this was not the case. Instead of filtering from the Kickstarter sheet, I had to include it as a criterion within the COUNTIFS statement. This guaranteed that I would retrieved only the play campaigns.

Results
Outcomes Based on Launch Date Conclusions
From the line chart, we can see that the best month to start a theater campaign is in May as it produces the highest amount of successful outcomes. Similarly, we can infer that December would not be the best month to launch a theater campaign, as it has the lowest number of successful outcomes. In fact, the number of successful campaigns is almost equivalent to the number of failed campaigns during the month of December.

# Outcomes Based on Launch Date

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85411967/132782481-7fd6a84d-611f-477c-af0a-2632d57b96bb.png)


# Outcomes Based on Launch Date Explanation
Although the pattern fluctuates, it is apparent that play campaigns with higher goals tend to have a greater percent chance of failing. We can see that there is a subtle decrease among campaign success as the goal amount becomes larger and larger. However, there is an anomaly at about $35,000, in which we see a sharp increase in the success rate and sharp decrease in failure rate.










# Outcomes Based on Goals

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85411967/132782183-2a4a749b-2f8a-4f46-9818-b48e0027db76.png)

# Outcomes Based on Goals Explanation
Some of the limitations on the dataset may include incomplete data. Although the data is complete for each campaign that is inputted in our spreadsheet, we may have missing data for campaigns that were never recorded. Additionally, we do have a few outliers within the dataset. Without further analysis, we are currently unable to determine the cause of these outliers.
