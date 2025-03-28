# Driver-Activity-Analysis

This repository contains data analysis projects that utilize two datasets: "Searches Data" and "Activity Data." The primary goal is to analyze the data to estimate the number of weekly trips based on various metrics, including Coverage Ratio, Unique Searches, and Finished Rides.

![](image1.jpg)


### Datasets
1. Searches Data
Description: This dataset contains information about user searches, including the number of unique searches and the coverage ratio.
Key Columns:
Date: The date of the search.
Hour: The hour of the search.
Unique Searches: The number of unique searches made during that hour.
Coverage Ratio (%): The percentage of users who saw at least one car.

2. Activity Data
Description: This dataset contains information about the activity of drivers, including the number of finished rides.
Key Columns:
Date: The date of the activity.
Hour: The hour of the activity.
Finished Rides: The number of rides completed during that hour.

### Analysis Methods
1. Estimating Weekly Trips with Maximum Coverage Ratio
Objective: To estimate the number of weekly trips that could have been completed based on the maximum Coverage Ratio.
Steps:
Find the Maximum Coverage Ratio: Use the MAX function to identify the highest coverage ratio from the "Searches Data" sheet.
Retrieve Unique Searches: Use VLOOKUP to find the corresponding unique searches for the maximum coverage ratio.
Calculate Estimated Finished Trips: Multiply the unique searches by the maximum coverage ratio to estimate finished trips.
Estimate Weekly Trips: Multiply the estimated finished trips by 7 to get the weekly estimate.
2. Creating a Combined Dataset
Objective: To create a new dataset that combines relevant columns from both datasets.
Steps:
Set Up a New Sheet: Create a new sheet named "Combined Data."
Copy Data: Copy the Date, Hour, and Unique Searches from the "Searches Data" sheet.
Use VLOOKUP: Use the VLOOKUP function to retrieve Finished Rides from the "Activity Data" sheet based on Date and Hour.
Instructions for Use
Open the Excel Workbook: Open the Excel file containing the "Searches Data," "Activity Data," and "Summary" sheets.
Navigate to the Summary Sheet: This sheet contains the analysis results and calculations.
Review the Combined Data: Check the "Combined Data" sheet for the merged dataset with Date, Hour, Unique Searches, and Finished Rides.
Modify as Needed: Feel free to adjust the formulas and ranges based on your specific data layout.
Conclusion
This repository provides a structured approach to analyzing user search data and driver activity data. By following the outlined methods, you can gain insights into the potential number of trips and the effectiveness of coverage ratios.
