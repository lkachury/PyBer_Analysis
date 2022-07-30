# PyBer_Analysis

## Overview 
Explain the purpose of the new analysis.

Background
V. Isualize has given you and Omar a brand-new assignment. Using your Python skills and knowledge of Pandas, you’ll create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, you’ll create a multiple-line graph that shows the total weekly fares for each city type. Finally, you’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.


## Results
Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types. There is a description of the differences in ride-sharing data among the different city types. Ride-sharing data include the total rides, total drivers, total fares, average fare per ride and driver, and total fare by city type.

The full Jupyter Notebook can be referenced here:

### Ride-Sharing Summary DataFrame By City Type
This DataFrame was created by using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns to get the total number of rides, total number of drivers, and the total fares for each city type and then calculating the average fare per ride and average fare per driver for each city type. 

1. The total number of rides for each city type is retrieved:
![image](https://user-images.githubusercontent.com/108038989/181867520-22addf8b-dd6d-476f-929c-b9bcdfb99c37.png)

2. The total number of drivers for each city type is retrieved: 
![image](https://user-images.githubusercontent.com/108038989/181867531-5291dd00-3fad-4f15-98fb-67db4ee6ceab.png)

3. The sum of the fares for each city type is retrieved: 
![image](https://user-images.githubusercontent.com/108038989/181867538-ddb738b1-8f8f-4009-b0e7-59dbb38b2d3b.png)

4. The average fare per ride for each city type is calculated: 
![image](https://user-images.githubusercontent.com/108038989/181867552-b2087c1e-af1a-4671-8e7a-bb4f21a64cc6.png)

5. The average fare per driver for each city type is calculated: 
![image](https://user-images.githubusercontent.com/108038989/181867566-986249e6-a002-492a-aa9c-f489a6921c9a.png)

6. A PyBer summary DataFrame is created: 
![image](https://user-images.githubusercontent.com/108038989/181867583-4024fb2b-b4cb-4cf3-ac81-f39e4ab9cea2.png)

7. The PyBer summary DataFrame is formatted: 
![image](https://user-images.githubusercontent.com/108038989/181867605-54373de9-3ed7-46a0-b08f-3eb9524dc179.png)

Deliverable 2: A multiple-line chart of total fares for each city type (45 points)
Using your Pandas skills and two new functions, pivot() andresample(), create a multiple-line graph that shows the total fares for each week by city type.

1. A DataFrame was created using the groupby() function on the "type" and "date" columns, and the sum() method is applied on the "fare" column to show the total fare amount for each date and time. 
2. A DataFrame was created using the pivot() function where the index is the "date," the columns are the city "type," and the values are the "fare." 
3. A DataFrame was created using the loc method on the date range: 2019-01-01 through 2019-04-28. 
4. A DataFrame was created using the resample() function in weekly bins and shows the sum of the fares for each week. 
5. An annotated chart showing the total fares by city type is created and saved to the "analysis" folder. 



## Summary
Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
