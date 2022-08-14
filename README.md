# Surfs-Up Weather Analysis

## Purpose:

### Investing in a North Shore Dream
<p align="center">
    <img width="500" height="300" src= "https://github.com/rloufoster/surfs_up/blob/main/Resources/NorthShoreGraphic_Resized.png?raw=true">
</p>    
   
The purpose of this analysis is to explore weather data stored in a SQLite database in order to inform a potential investor on weather patterns on Oahu, Hawaii.  While visiting Oahu's North Shore last year, I had the idea to create a business that would allow me to live out my dream of owning a surfboard and milkshakes operation on Oahu. I have some savings but will need additional investors to get the business off the ground. I put together a strong business plan and reached out to a successful surfing entrepreneur, W. Avy. Mr Avy is very impressed with my proposal and initial analyses, but wants more information about temperature trends. Specifically, he wants temperature data for the months of June and December on Oahu, in order to determine if the surf and shakes business is sustainable year-round. W Avy has asked that I submit these additional insights before coming "onboard"- no pun intenteded.


## Method:

In order to explore the data stored in SQLite , SQLAlchemy was used to connect and generate queries in order to capture the necessary data for the analysis. Throughout this exploration process, both Jupyter Notebook and VS Code were used to import dependencies and write and run the code.  Two specific descriptive analyses were requested:

 * 1.) Determine the Summary Statistics for June weather patterns based on the hawaii.sqlite database 
 * 2.) Determine the Summary Statistics for December weather patterns based on the hawaii.sqlite database


### Resources:

.
* **Data File:** hawaii.sqlite
* **Programming Files:** Surfsup_Challenge.ipynb which includes an earlier analysis, climate_analysis.ipynb
* **Data Tools:** Matplotli 3.2.2, Python 3.9, Visual Studio Code 1.50.0, Anaconda 4.8.5, Jupyter Notebook 6.1.4, Pandas, Numpy, Sqlalchemy,       Flask 

### The following are the steps taken to capture the June Analysis: 

   **Write a query to retrieve June temps**
   
   ![June_Query_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_Query_Del1.png?raw=true)

   **Convert June temps to list**
   
   ![June_TempsList_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_TempsList_Del1.png?raw=true)

   **Create DataFrame from the list of temps for the month of June**
   
   ![June_LSTODF_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_LSTODF_Del1.png?raw=true)

   

### The following are the steps taken to capture the December Analysis:

   **Write a query to retrieve December temps**
   
   ![Dec_Query_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_Query_Del2.png?raw=true)

   **Convert December temps to list**
   
   ![Dec_TempsList_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_TempsList_Del2.png?raw=true)

   **Create DataFrame from the list of temps for the month of June**
   
   ![Dec_LSTODF_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_LSTODF_Del2.png?raw=true)

   

## Results:


* Precipitation insights were captured by looking at precipitation data collected by the weather stations from August 23, 2016 - August 23, 2017. Average precipitation for June is 14% and December is 22%.   
 
   
   ![Precip_Graph](https://github.com/rloufoster/surfs_up/blob/main/Resources/Precipitation_1yr_graph.png?raw=true)


   ![Precip_Stats](https://github.com/rloufoster/surfs_up/blob/main/Resources/Precipitation_1yrAug.png?raw=true) 
   
   

* I also looked at the number of weather stations that were collecting precipitation data.  There were 9 stations with USCOO519281 showing the highest amount of reported observations with 2,772. I used the information from this station to review the temperature for the same time period. The results showed that the average temperature throughout the year was 72°F with a low of 54°F and a high of 85°F.


  ![Weather_Stations](https://github.com/rloufoster/surfs_up/blob/main/Resources/weather_stations_graph.png?raw=true)
  

* Temperature Descriptive Stats:

**June Temps**

![June_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_TempDescriptiveStats_Del1.png?raw=true)

**December Temps**

![Dec_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_TempDescriptiveStats_Del2.png?raw=true)

#### Key Differences on Weather in Oahu

* The average recorded temperature in June is approximately 75 degrees F, 4 degrees higher than the average temp in December.
    
* Both June and December showed similar max temperatures, however December min temp was 8 degrees lower than June.

* The December temperatures are only slightly more variable than those in June with a std of 3.74 compared to that of June at 3.25. 


## Summary

Even though temperatures recorded in December are slightly more variable than in June, December would still provide optimal weather conditions for both surfing and ice cream.  The average temperatures in June and December only differ by 4 degrees. In addition, precipitation is very moderate year round, only 14% in June and 22% in December.  

Future analyses might investigate other variables that influence optimal surfing conditions such as the wind and wave swells. It's no mystery that Oahu is know to be one of the prime surfing locations in the world, but are there specific locations on Oahu that are better than others. Also, a more thorough dive into the temperature and precipitation might reveal more variance in climate if it filtered for a longer timeframe.  Say 10 years. I would also want to include a seasonal analysis. Most variable weather patterns happen at the changes of the seasons.  Instead of capturing only June and December precipitation and temperature, I would include March and September.  



