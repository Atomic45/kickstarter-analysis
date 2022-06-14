# Kickstarter-Analysis
### By Sandra Garza

## Purpose of Analysis
This analysis is to provide an overview of the outcomes versus goals for the theater subcategory according to the launch date. The analysis will focus on categorizing the different fundraising goals to compare with the campaign outcomes that had a successful, failed or canceled status, and using the launch dates to visualize the trends for each month according to the specified outcomes. 

## Analysis and Challenges
The Kickstarter analysis was created by using an Excel report with detailed information for each campaign. The analysis called for a visualization to see what month had the most outcomes ranging from successful, failed or canceled. This range required some filtering and adding functions such as, using the [Epoch & Unix Converter tool](https://www.epochconverter.com/) to confirm a timestamp matches the formula used to change the timestamp to a human date. The following steps were taken: 

- Created a new column next to the launch date column and named it Date Created Conversion.
- Added the formula =(((J2/60)/60)/24)+DATE(1970,1,1) to convert the timestamp to a human date. 
- Added the time stamp from the launch date column into the [Epoch & Unix Converter too](https://www.epochconverter.com/) to compare.
- Added the format to all the fields in that column by selecting the elipses and double clicking. 
- Changed the format from General to Date. 
The next item was to figure out the Percentage Funded. A new column was added and the following formula was used =ROUND(E2/D2*100,0). This formula was used to show the percentage funded from the goal to the pledged amount. 
