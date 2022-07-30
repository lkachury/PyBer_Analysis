# PyBer_Analysis

## Overview 
Explain the purpose of the new analysis.

Background
V. Isualize has given you and Omar a brand-new assignment. Using your Python skills and knowledge of Pandas, you’ll create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, you’ll create a multiple-line graph that shows the total weekly fares for each city type. Finally, you’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.


## Results
Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types. There is a description of the differences in ride-sharing data among the different city types. Ride-sharing data include the total rides, total drivers, total fares, average fare per ride and driver, and total fare by city type.

Deliverable 1: A ride-sharing summary DataFrame by city type
Using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns, get the total number of rides, total number of drivers, and the total fares for each city type. Then, calculate the average fare per ride and average fare per driver for each city type. Finally, add this data to a new DataFrame, then format the columns.

1. The total number of rides for each city type is retrieved. 
> In Step 1, use the groupby() function to create a Series of data that has the type of city as the index, then apply the count() method to the "ride_id" column.



3. The total number of drivers for each city type is retrieved. 
4. The sum of the fares for each city type is retrieved. 
5. The average fare per ride for each city type is calculated. 
6. The average fare per driver for each city type is calculated. 
7. A PyBer summary DataFrame is created. 
8. The PyBer summary DataFrame is formatted as shown in the example. 



Deliverable 2: A multiple-line chart of total fares for each city type (45 points)
Using your Pandas skills and two new functions, pivot() andresample(), create a multiple-line graph that shows the total fares for each week by city type.

1. A DataFrame was created using the groupby() function on the "type" and "date" columns, and the sum() method is applied on the "fare" column to show the total fare amount for each date and time. 
2. A DataFrame was created using the pivot() function where the index is the "date," the columns are the city "type," and the values are the "fare." 
3. A DataFrame was created using the loc method on the date range: 2019-01-01 through 2019-04-28. 
4. A DataFrame was created using the resample() function in weekly bins and shows the sum of the fares for each week. 
5. An annotated chart showing the total fares by city type is created and saved to the "analysis" folder. 



## Summary
Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
