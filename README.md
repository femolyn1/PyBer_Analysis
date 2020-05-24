 # Project Overview
This is an exploratory analysis on data in some large csv files of a ride sharing app company. The analysis will showcase relationship between type of city and number of drivers and rides. 

## Resources:
Data Source: ride_data.csv & city_data.csv; Software: Python 3.7.6; Jupyter Notebook

# Challenge:
# PyBer Analysis
   The purpose of this analysis is to identify key ride sharing metrics by type of city and create a graphical representation of the total weekly fares based on the city types which will help improve access to ride sharing services and determine ride affordability for the city types. 
   ## Technical Analysis
  The total drivers, rides ,fares and average fare per ride were obtained using the groupby function along with the sum , count and mean functions while the average fare per driver was obtained by dividing the total fares per city type by the total drivers per city type.To obtain the right data for plotting the graph, the following tasks was performed:
  * Columns of the main data was renamed
  * Index was reset using the datetime function
  * Groupby function was used used to group the fares by city and date 
  * The groupby function above was placed into a data frame in one step 
  * Data frame's index was reset and used to create a pivot table
  * Pivot table was resampled using the resample and sum fucntions 
  * A five thrity eight style graph was plotted using the object oriented method 

  ### Results
   
   
   
 
  



  

  
  
  
