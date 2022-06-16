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
Next, in the table below, a pivot table was not created. Instead separate ranges of the goal amounts were created by filtering and using the =COUNTIF function. A count of the different outcomes was also used along with the percentage amounts included for each range and outcome. The data was filtered by the Theater Category and the Plays Subcategory. The percentage function used was =(B2/E2), but some fields included zeroes. This caused for an expansion of the function to include the IFERROR function. Here is what was used: =IFERROR(B2/E2,0), which places a 0 for any calculation that caused an error. 

![image](https://user-images.githubusercontent.com/30300621/173983793-2078e13c-df7c-4bde-937f-abe65462ace9.png)

This also shows us that none of the theater plays were canceled, which allows for a 50/50 chance a theater play will be successful or fail. The line graph created from the table shows a negative correlation between the Percentage Successful and the Percentage Failed. There are no canceled outcomes, again because none of the theater plays were canceled. 

![image](https://user-images.githubusercontent.com/30300621/173985940-1bc90502-0a9c-4cfe-808b-62c85c733c0c.png)

## Summary
It is difficult to give an accurate conclusion due to the data is limited. For example, the Outcomes based on Launch Date does not include other factors that may have given accurate reason why there were cancelations or why a theater outcome failed. Was it due to weather? Was it due to an incident with a theater? Was it the lack of popularity or lack of marketing? We can assume the seasons played a role if that is sufficient. 

For the Outcomes based on goal section, it is also difficult to assume the negative correlation can be based on the 50/50 chance. We do not have demographics, location or status to provide a more accurate analysis. If we used demographics, we can determine the popularity of some theater plays in certain areas or lack of popularity. 











