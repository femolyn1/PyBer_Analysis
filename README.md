 

# PyBer Analysis
The purpose of this exploratory data analysis is to identify key ride sharing metrics by type of city and create a graphical representation of the total weekly fares based on the city types which will help improve access to ride sharing services and determine ride affordability.
   ## Technical Analysis
  The [total drivers](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L682-L684), [total rides](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R656-R658) ,[total fares](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L631-L632 ) and [average fare per ride](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24R707-R711) were obtained using the groupby function along with the sum , count and mean functions while the [average fare per driver](https://github.com/femolyn1/PyBer_Analysis/commit/11c28c26eec3a73c17ddb678bb1126ff32b5a6c8#diff-8ca64d95e3c20e73e5f0833a72afef24L733-L737 ) was obtained by dividing the total fares per city type by the total drivers per city type. To obtain the data frame used for plotting the multiple line graph, the following tasks was performed:
  * Columns of the main data was renamed using the [rename column function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/column_remane.png)
  * Index was set to date time using the [date time index function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Set%20Index%20Function.png)
  * A new dataframe was created with city type and fare columns using the [copy function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Using%20copy%20function.png)
  * The index of the new data frame was checked using the [info function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Info%20function.png)
  * Groupby function was used used to group the fares by city and date and this was placed in a data frame using the [dataframe function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/groupby%20function%20for%20multiple%20columns.png)
  * A pivot table was created using the [pivot table function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Pivot%20Data%20frame%20function.png)
  * [Loc function](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Using%20loc%20function%20for%20a%20given%20time%20range.png) was used to organize the pivot table within the given date range
  * The pivot table was resampled using the [resample and sum functions](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Using%20resampling%20and%20sum%20functions.png)
   
  ### Results
  ![](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/New%20Data%20frame.PNG)
     
   As shown in the data frame above, the rural cities had the highest average fare per driver and ride while the urban cities had the lowest and the high fares observed in the rural cities was due to the low number of total rides and total drivers in those cities.
  
  ![](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/Multiple%20line%20graph.png)
   
   As shown in the multiple line graph above, the urban cities had the highest total fare within the months of January to April 2019 followed by the rural cities while the urban cities had the lowest fare and the low fares can be attributed to the empty cells observed in the rural cities column after arranging the data into the specified date range using the loc function. 
    In summary, the drop in the number of ride usage in the rural cities within the months of January to April, 2019 could be due to the low number of available rides and drivers in those cities and allocating more rides & drivers to the rural cities will most likely reduce average fare per ride & driver which will invariably boost ride affordability. In addition, although the available data is limited to 2019, the Urban cities might also benefit from more ride allocation within the months of January to April as this will help meet the demands for rides in those months , increase revenue and enhance affordability.
  
# Challenges Encountered during Analysis
Formatting the horizontal axis in the multiline plot to resemble the graph provided in the challenge question was a bit difficult. Upon plotting the graph, the date format on the horizontal axis had the format 2019-01-01, and the challenge question asked us to show the months and day format ( Jan 2019, Feb, Mar , Apr). 

## Resolution strategy
To resolve this issue, I used the plt.xticks() funtion to view the numerical format of the dates and then added the dates into the function along with the calender month format. See a screen shot showing the code used to format the horizontal axis below:
![](https://github.com/femolyn1/PyBer_Analysis/blob/master/Images/plt.xticks.png)

# Recommendation(s)

In addition to the above analysis, I would recommend obtaining more information about the demographics of those living the the three city types and additional two to five previous year city and ride data. 
## Recommended Future Analysis
With the demographic information such as  populutaion and age range, we can group the fares by age and city type or by population and city type. These information will shed more light on the reason why some of the city types had high average fare per driver and ride. Also, using the loc function on two to five previous year data might shed more light on the reason why thr rural and suburban cities had low fares within the month of January to April. 

# Resources:
Data Source: ride_data.csv & city_data.csv; Software: Python 3.7.6; Jupyter Notebook

 
   
 
  



  

  
  
  
