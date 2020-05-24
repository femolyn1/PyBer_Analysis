 # Project Overview
This is an exploratory analysis on data in some large csv files of a ride sharing app company. The analysis will showcase relationship between type of city and number of drivers and rides. 

## Resources:
Data Source: ride_data.csv & city_data.csv; Software: Python 3.7.6; Jupyter Notebook

# Challenge:
# PyBer Analysis
   The purpose of this analysis is to identify key ride sharing metrics by type of city and create a graphical representation of the total weekly fares based on the city types which will help improve access to ride sharing services and determine ride affordability for the city types. 
   ## Technical Analysis
  The [total drivers](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L682-L684), [total rides](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R656-R658) ,[total fares](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L631-L632 ) and [average fare per ride](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R707-R711) were obtained using the groupby function along with the sum , count and mean functions while the [average fare per driver](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L733-L737 ) was obtained by dividing the total fares per city type by the total drivers per city type. To obtain the right data for plotting the graph, the following tasks was performed:
  * Columns of the main data was renamed
  ![](https://github.com/femolyn1/PyBer_Analysis/blob/master/column_remane.png)
  * Index was reset using the datetime function
  * Groupby function was used used to group the fares by city and date 
  * The groupby function above was placed into a data frame in one step 
  * Data frame's index was reset and used to create a pivot table
  * Pivot table was resampled using the resample and sum fucntions 
  * A five thrity eight style graph was plotted using the object oriented method 
  ### Results
   [Data Frame]()
   
   As shown in the above table , the rural cities has the highest average fare per driver and ride while the urban cities has the lowest. The high fare per ride and driver observed in the rural cities is due to the low number of total rides and total drivers in those cities and allocating more rides and drivers to the rural cities will reduce the high fares in those cities.
   
   
   [Total Fare by City Type]()
   
 
   
 
  



  

  
  
  
