# Kickstarter-Analysis
### By Sandra Garza

## Purpose of Analysis
This analysis is to provide an overview of the outcomes versus goals for the theater subcategory according to the launch date. The analysis will focus on categorizing the different fundraising goals to compare with the campaign outcomes that had a successful, failed or canceled status, and using the launch dates to visualize the trends for each month according to the specified outcomes. 

## Analysis and Challenges
The Kickstarter analysis was created by using an Excel report with detailed information for each campaign. The analysis called for a visualization to see what month had the most outcomes ranging from successful, failed or canceled. This range required some filtering and adding functions such as, using the [Epoch & Unix Converter tool](https://www.epochconverter.com/) to confirm a timestamp matches the function used to change the timestamp to a human date. =(((J2/60)/60)/24)+DATE(1970,1,1)  Other functions include the following: 

- Adding a new column to calculate the Percentage Funded from the goal to the pledged amount by using the formula =ROUND(E2/D2*100,0). 
- retrieving the Year from the converted date. =YEAR(K2)
- Fixing errors for fields that contained 0 by using the =IFERROR function =IFERROR(ROUND(E2/M2,2),0)and  T

After the conversions and functions were created, a pivot table was created to filter the necessary items needed for this analysis. 

![image](https://user-images.githubusercontent.com/30300621/173476912-9472a114-8c95-40de-8f6a-66c0001e2604.png)


The next item was to figure out 
