# Kickstarting with Excel
## Overview of Project
### Purpose
The purpose of this project is to examine Kickstarter data, assisting Louise in fundraising for future projects through Kickstarter campaigns. We look at project outcomes compared to their launch date and their goals. This will give Louise the information she needs to determine when to launch her Kickstarter campaign and what fundraising goal she should set for herself. Lastly, we focus our analyses on theaters and plays, as this is the type of fundraising campaign that interests Louise.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
Our analysis of outcomes based on launch date includes creating a pivot table and a line chart that examine the effect of launch date on the outcome of a Kickstarter campaign. The pivot table counts the number of theater campaigns that were either successful, failed, or canceled and groups the results by month of launch date. The table can be filtered by year and the parent category, in this case theater. Please see line chart below. 

![Please follow link](https://github.com/JeremyKRay/kickstarter-analysis/blob/2fc6842dfcbe0416a5ef6afc640d601199e9daf9/Theater_Outcomes_vs_Launch.png).

### Analysis of Outcomes Based on Goals
Our analysis of outcomes based on goals includes creating monetary ranges for fundraising goals and counting the number of successful, failed, and canceled projects for each of the ranges. The count requires the use of Excel's 'COUNTIFS()' function. An example of this function is '=COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays")'. A sum of the three outcomes is calculated in order to calculate a percentage for each outcome. This analysis is limited to examine data on plays, as you can see in the 'COUNTIFS()' statement above. These results are displayed in a line chart below.  

![Please follow link](https://github.com/JeremyKRay/kickstarter-analysis/blob/2fc6842dfcbe0416a5ef6afc640d601199e9daf9/Outcomes_vs_Goals.png).

### Challenges and Difficulties
These analyses did present a few challenges and difficulties. First, during previous analyses of the Kickstarter data, I had created a couple of additional data sheets that caused my spreadsheet to be abnormally large in size. In their creation, all empty cells below legitimate data cells were being considered data and therefore adding to the size of my file. After deleting them all, the spreadsheet is now a manageable size. I also had some difficulty using the 'COUNTIFS()' function in excel simply because I had never used it before, but the instructional video provided proved extremely helpful. Also, excel does do a pretty good job guiding you through building the command if you have at least some understanding of its logic, which the video provided. Lastly, when creating the line chart of outcomes based on goals, I initially simply hid the columns that I did not want included in my line chart in order to create the chart on the desired columns. However, I learned that doing this does not lock this data into your chart. Unhiding the columns subsequently adds them to your chart dataset. Fortunately, this actually proved to be a helpful exercise in adjusting data in your dataset for a chart that has already been created and formatted instead of having to delete and recreate the entire chart.
## Results
The analysis of theater outcomes by launch date draws two primary conclusions for Louise. 
1. Both Successful and Failed theater Kickstarter campaigns were highest when started in the month of May. Why? The total number of campaigns was also highest in May. This is not the most informative analysis.
2. Further analysis is required for Louise to be confident in the best month to begin a Kickstarter theater campaign. Perhaps an examination of the percentage of Successful campaigns and percentage of Failed campaigns for each month is in order. 

The analysis of outcomes based on goals is more conclusive. The percentage of successful campaigns was highest and the percentage of failed campaigns was lowest when the goal of a campaign was less than $1000. Also, a similar trend is evident when the goal of a campaign is within the range of $35000 and $44999. Obviously, anything less than $1000 is not a lot of money to start a theater project. This would explain the successful campaigns. Assuming Louise will be looking to raise more funding than this, she may want to focus on a goal that falls within the latter range.  

This dataset does present some limitations. It does not include any data on demographics or geographics, other than the country. The location of a theater or play project could have an effect on its success, as could the people who live in and around this location. 

Perhaps a table with location and demographic information could be joined with this kickstarter data and a chart showing the relationship between location data and certain demographic data to successful, failed, and canceled kickstarter campaigns could be created. Lastly, if this information could be mapped and a little more analyses are performed on outcomes based on launch date, Louise would have sufficient information on when to start a campaign, how much to set as a goal for her campaign, and where to start her campaign to ensure it is successful. 
