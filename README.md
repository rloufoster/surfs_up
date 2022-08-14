# Surfs Up!

## Purpose

### Investing in a North Shore Dream

   ![NorthShoreGraphic](https://github.com/rloufoster/surfs_up/blob/main/Resources/NorthShoreGraphic_Resized.png?raw=true)      

The purpose of this analysis is to explore weather data stored in a SQLite database in order to inform a potential investor on weather patterns on Oahu, Hawaii.  While visiting Oahu's North Shore last year, I had the idea to create a business that would allow me to live out my dream of owning a surfboard and milkshakes operation on Oahu. I have some savings but will need additional investors to get the business off the ground. I put together a strong business plan and reached out to a successful surfing entrepreneur, W. Avy. Mr Avy is very impressed with my proposal and initial analyses, but wants more information about temperature trends. Specifically, he wants temperature data for the months of June and December on Oahu, in order to determine if the surf and shakes business is sustainable year-round. W Avy has asked that I submit these additional insights before coming "onboard"- no pun intenteded.


## Method

In order to explore the data stored in SQLite , SQLAlchemy was used to connect and generate queries in order to capture the necessary data for the analysis. Throughout this exploration process, both Jupyter Notebook and VS Code were used to import dependencies and write and run the code.  Two specific descriptive analyses were requested:

 * 1.) Determine the Summary Statistics for June weather patterns based on the hawaii.sqlite database 
 * 2.) Determine the Summary Statistics for December weather patterns based on the hawaii.sqlite database


### Resources:

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

   

## Results


* When we pulled the data, we first looked at the the precipitation for a one year timeframe. We reviewed the activity from August 23, 2016 -   August 23, 2017. The average was 18% based on 2,021 observations. This tells us that throughout the year, Oahu was mostly sunny throughout     the day and experienced low rainfall.
 
   
   ![Precip_Graph](https://github.com/rloufoster/surfs_up/blob/main/Resources/Precipitation_1yr_graph.png?raw=true)


   ![Precip_Stats](https://github.com/rloufoster/surfs_up/blob/main/Resources/Precipitation_1yrAug.png?raw=true) 
   
   

* We also looked at the number of weather stations that were actively collecting precipitation data and focus on one station that had the most   observations recorded. In total, there were (9) stations with USC00519281 showing the highest amount of observations at 2,772 entries. We     used the information from this station to review the temperature for the same time period. The results showed that the average temperature     throughout the year was 72°F with a low of 54°F and a high of 85°F.


  ![Weather_Stations](https://github.com/rloufoster/surfs_up/blob/main/Resources/weather_stations_graph.png?raw=true)
  

* Temperature Descriptive Stats:

**June Temps**

![June_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_TempDescriptiveStats_Del1.png?raw=true)

**December Temps**

![Dec_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_TempDescriptiveStats_Del2.png?raw=true)

* The average recorded temperature in June is approximately 75 degrees F, 4 degrees higher than the average temp in December.
    
* Both June and December showed similar max temperatures, however December min temp was 8 degrees lower than June.

* The December temperatures are only slightly more variable than those in June. 


## Summary

In summary, the temperature in Oahu is relatively the same throughout the year and the chances of continuous rainfall is low. When we rewrite the queries to add precipitation to the results for June and December, the average precipitation in those months showed:

