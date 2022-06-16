# Kickstarter-Analysis
### By Sandra Garza

## Purpose of Analysis
This analysis is to provide an overview of the outcomes versus goals for the theater category according to the launch date. The analysis will focus on categorizing the different fundraising goals to compare with the campaign outcomes specified as successful, failed or canceled. Also, the launch dates are used to visualize the trends for each month. Using certain functions in excel with excel tools will help create a pivot table to filter for the items needed in creating a visualization. The visualization will help determine how to approach the trends identified to use in setting successful goals within certain timelines. 

## Analysis and Challenges
The Kickstarter analysis was created by using an Excel report with detailed information for each campaign. The analysis called for a visualization to see what month had the most outcomes ranging from successful, failed or canceled. And how the average outcome compared to the average goal. This range required some filtering and adding functions such as, using the [Epoch & Unix Converter tool](https://www.epochconverter.com/) to confirm a timestamp matches the function used to change the timestamp to a human date. =(((J2/60)/60)/24)+DATE(1970,1,1)  Other functions include the following: 

- Adding a new column to calculate the Percentage Funded from the goal to the pledged amount by using the formula =ROUND(E2/D2*100,0). 
- retrieving the Year from the converted date. =YEAR(K2)
- Fixing errors for fields that contained 0 by using the =IFERROR function =IFERROR(ROUND(E2/M2,2),0).
- Separating the Category by its subcategory with the "Text to Column" tab in excel. This allowed for more options to use for the analysis. 

After the conversions and functions were created, a pivot table was created to filter the necessary items needed for this analysis. This analysis required the Category "theater" to be filtered. Also, the "Year" column was filtered to show each month only. The outcomes were, as mentioned, successful, failed, and canceled. 
![image](https://user-images.githubusercontent.com/30300621/173476912-9472a114-8c95-40de-8f6a-66c0001e2604.png)

## Analysis for Theater Outcomes Based on Launch Date
The pivot table allows for the creation of a line graph that helps identify trends and an overview of the average percentage of each outcome for each month. The visualization of the line graph is shown below.  
![image](https://user-images.githubusercontent.com/30300621/173481411-b942a09d-dbd5-406a-92fb-c44412630648.png)

The line graph shows that the highest number of successful outcomes happened in the month of May. The least successful was in December. Successful outcomes decreased by 65% from October to December. This shows that successful theater events were not popular during the winter season and that could be due to holiday shopping. The high increase from March to May, another two month period, shows a 55% increase. This is during the spring time, so a conclusion can mean weather plays a factor for the theater outcomes. 

## Analysis for Outcomes Based on Goals
The next item was to figure out the Outcome based on Goals. In the chart below, no pivot table was created. Filtering and the =COUNTIF function were used to create ranges according to the Goal amounts. 
