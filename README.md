 # Project Overview
This is an exploratory analysis on data in some large csv files of a ride sharing app company. The analysis will showcase relationship between type of city and number of drivers and rides. 

## Resources:
Data Source: ride_data.csv & city_data.csv; Software: Python 3.7.6; Jupyter Notebook

# Challenge:
# PyBer Analysis
The purpose of this analysis is to identify key ride sharing metrics by type of city and create a graphical representation of the total weekly fares based on the city types which will help improve access to ride sharing services and determine ride affordability.
   ## Technical Analysis
  The [total drivers](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L682-L684), [total rides](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R656-R658) ,[total fares](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L631-L632 ) and [average fare per ride](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R707-R711) were obtained using the groupby function along with the sum , count and mean functions while the [average fare per driver](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L733-L737 ) was obtained by dividing the total fares per city type by the total drivers per city type. To obtain the right data for plotting the graph, the following tasks was performed:
  * Columns of the main data was renamed using the rename column function
  * Index was set to date time using the date time index function 
  * A new dataframe was created with city type and fare colums using the copy function
  * The index of the new data frame was checked using the info function
  * Groupby function was used used to group the fares by city and date and this was placed in a data frame using the dataframe function
  * Data frame's index was reset using the reset index funtion
  * A pivot table was created using the pivot table function 
  * Loc function was used to reorganize the pivot table within a given date range
  * The pivot table was resampled using the resample and sum fucntions 
  * A multiple line graph was created using the Five Thirty Eight style and object oriented method
  
  ### Results
  ![](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/New%20Data%20frame.PNG)
     
   As shown in fig 1 above, the rural cities had the highest average fare per driver and ride while the urban cities had the lowest. The high fare per ride and driver observed in the rural cities is due to the low number of total rides and total drivers in those cities. Allocating more rides and drivers to the rural cities will reduce the high average fares in those cities and make rides more affordable. 
   ![](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Multiple%20line%20graph.png)
   
   As shown in the multiple line graph, the urban cities had the highest total fare within the months of January to April 2019 followed by the rural cities while the urban cities had the lowest fare. The data frame created using the loc function on the pivot data, shown below, helps to explain the reason for the low fares in the suburban and rural cities within the months of January to April 2019.
   
   [Fig 3]()
 
  As shown above,the rural cities had the most empty cells within the period under consideration followed by the suburban cities while the urban cities had the lowest empty cells.  We can infer from the multiline graph that allocating more rides to the urban cities within the months of  January to April will boost fare revenue and improve ride afordability in the urban cities within specified months.In summary, the drop in the number of ride usage in the rural cities within the months of January to April, 2019 could be due to the low number of available rides and drivers in those cities.Therefore, allocating more rides and drivers to the rural cities will reduce average fare per ride and avarage fare per driver which will invariably boost ride afordability. The Urban cities can also benefit from more ride allocation within the months of January to April as this will help meet the demands for rides, increase revenue and reduce affordability.
  
# Challenges during Analysis

 
 
   
 
  



  

  
  
  
