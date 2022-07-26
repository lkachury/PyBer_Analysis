# PyBer_Analysis

## Overview 
PyBer is a python based ride sharing app that operates in urban, suburban, and rural cities. The purpose of this analysis is to determine how the data differs by city type and how those differences can be used by decision-makers at PyBer. Python and Pandas functions will be used to create a summary DataFrame of the ride-sharing data by city type and then Matplotlib and new Pandas functions will be used to create a multiple-line graph depicting the total weekly fares for each city type. 

## Resources
### Data Source
- city_data.csv
- ride_data.csv

### Software
- Python 3.7.6
- Conda 4.13.0
- Jupyter Notebook 6.4.8
- Dependencies:
  - Python Pandas Library
  - Python MatPlotLib Library

## Results
The full Jupyter Notebook can be referenced here: 
<br /> https://github.com/lkachury/PyBer_Analysis/blob/main/PyBer_Challenge.ipynb

### Ride-Sharing Summary DataFrame By City Type
This DataFrame was created by using the Pandas groupby() function with the count() and sum() methods on PyBer DataFrame columns to get the total number of rides, total number of drivers, and the total fares for each city type and then calculating the average fare per ride and average fare per driver for each city type. 

1. The total number of rides for each city type is retrieved:
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867520-22addf8b-dd6d-476f-929c-b9bcdfb99c37.png)

2. The total number of drivers for each city type is retrieved: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867531-5291dd00-3fad-4f15-98fb-67db4ee6ceab.png)

3. The sum of the fares for each city type is retrieved: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867538-ddb738b1-8f8f-4009-b0e7-59dbb38b2d3b.png)

4. The average fare per ride for each city type is calculated: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867552-b2087c1e-af1a-4671-8e7a-bb4f21a64cc6.png)

5. The average fare per driver for each city type is calculated: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867566-986249e6-a002-492a-aa9c-f489a6921c9a.png)

6. A PyBer summary DataFrame is created: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867583-4024fb2b-b4cb-4cf3-ac81-f39e4ab9cea2.png)

7. The PyBer summary DataFrame is formatted: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181867605-54373de9-3ed7-46a0-b08f-3eb9524dc179.png)

According to the dataframe, urban cities experince 13 times more rides than rural cities and over 2.5 times more rides than suburban cities. There are almost 5 times more drivers in urban cities than suburban cities and almost 31 times more drivers in urban cities than in rural cities. Total fares in urban cities were double the total fares of suburban cities and almost 4 times as much as the total fares of rural cities. 

The average fare per ride among the three types of cities is about $30, which is the same as the average fare per ride in suburban cities. Rural cities have the highest average fare per ride as they have the lowest amount of rides and drivers while urban cities have the lowest average fare per ride since they have the largest amount of rides and drivers. 

Average fare per driver is much more varied than average fare per ride among the three city types. The average fare per driver among the three types of cities is about $37, which is very close to the average fare per driver in suburban cities. The average fare per driver in rural cities is over 3 times as much as the average fare per driver in urban cities and almost 1.5 times as much as the average fare per in suburban cities. 

### Multiple-Line Chart of Total Fares for Each City Type 
This multiple-line graph depicting the total fares for each week by city type was created by using the Pandas pivot() and andresample() functions. 

1. A DataFrame was created using the groupby() function on the "type" and "date" columns, and the sum() method is applied on the "fare" column to show the total fare amount for each date and time: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181872511-057566ea-42fb-4850-abba-31205de082de.png)

2. A DataFrame was created using the pivot() function where the index is the "date," the columns are the city "type," and the values are the "fare":
<br /> ![image](https://user-images.githubusercontent.com/108038989/181872529-b1ed0f07-a6a4-435f-adcb-82a1a589af29.png)

3. A DataFrame was created using the loc method on the date range: 2019-01-01 through 2019-04-28: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181872546-9d44c889-f595-4b5b-a01c-6bbe5c485a38.png)

4. A DataFrame was created using the resample() function in weekly bins and shows the sum of the fares for each week: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181872564-9bae335e-1c58-4087-ac34-02a781496b9c.png)

5. An annotated chart showing the total fares by city type is created and saved to the "analysis" folder. 
<br /> ![image](https://user-images.githubusercontent.com/108038989/181872572-5907201c-503c-4f9e-9319-802277e228a9.png)

## Summary
Rural cities have the lowest total fares but the highest average fare per ride and driver, it is recommended that the PyBer CEO allocate more drivers to rural cities in order to increase their profits. 

Total fares for all city types peaked around the end of February, perhaps due to an increased demand for rides with the start of Spring. It is also recommended that PyBer partner with local events in these cities in order to increase the demand for rides.

Lastly, it is recommended that Pyber offer some incentive for drivers in order to attarct and maintain drivers in rural and suburban cities.
