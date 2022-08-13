# surfs_up
Using SQLite, SQLAlchemy, Flask and Python in Jupyter Notebook to analyze climate data to guide in a surf shop investment decision making

## Purpose

### Investing in a North Shore Dream

 ![NorthShoreGraphic](https://github.com/rloufoster/surfs_up/blob/main/Resources/NorthShoreGraphic_Resized.png?raw=true)      

While visiting Oahu last year,  I had the idea to create a business that would allow me to live out my dream of living, and surging on Oahu permantently. A shop that would serve surfboards and ice cream to tourists.  I had some savings, but would need additional investors to get business off the ground.  I have put together a strong business plan and reached out to a successful surfing entrepreneur who is famous for his love of surfing, W. Avy. Mr Avy likes your business plan and initial analysis, but he wants more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round. W Avy, therefore has asked that, along with my business plan, I put together a weather analysis of Oahu before he will agree to come "onboard"- no pun intenteded.



## Method

This new assignment consists of two technical analysis deliverables and a written report. You will submit the following:

#### Resources:

* **Data File:** hawaii.sqlite
* **Programming Files:** Surfsup_Challenge.ipynb which includes an earlier analysis, climate_analysis.ipynb
* **Data Tools:** Matplotli 3.2.2, Python 3.9, Visual Studio Code 1.50.0, Anaconda 4.8.5, Jupyter Notebook 6.1.4, Pandas, Numpy, Sqlalchemy,       Flask 

-Deliverable 1 Code 

Query Code for June
![June_Query_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_Query_Del1.png?raw=true)

Temps List Code for June
![June_TempsList_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_TempsList_Del1.png?raw=true)

List to DF code for June
![June_LSTODF_Del1](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_LSTODF_Del1.png?raw=true)

June Dataframe
![June_Dataframe](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_Dataframe_Del1.png?raw=true)

-Deliverable 2 Code 

Query Code for December
![Dec_Query_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_Query_Del2.png?raw=true)

Temps List Code for June
![Dec_TempsList_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_TempsList_Del2.png?raw=true)

List to DF code for Dec
![Dec_LSTODF_Del2](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_LSTODF_Del2.png?raw=true)

Dec Dataframe
![Dec_Dataframe](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_Dataframe_Del2.png?raw=true)


## Results

Key Differences in Weather: Oahu, Hawaii

Descriptive Stats:

June
![June_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/June_DescriptiveStats_Del1.png?raw=true)

December
![Dec_DescriptiveStats](https://github.com/rloufoster/surfs_up/blob/main/Resources/Dec_DescriptiveStats_Del2.png?raw=true)


* The average recorded temperature in June is about 75 degrees F, 4 degrees higher than the average temp in December.
  * This represents a -5% change in average temperature from June to December
  
* The frequency of temperatures recorded in June tends to have a much more normal, tight bell curve distribution, cooroborated by the smaller   std measure of June temps vs December temps

* The December temperatures seem to be more variable than those in June given its larger range in recorded temperatures (comparing the max vs   min temp of each month)

  * However, when looking at the plotted distribution of Dec Temps, we can see that the median temperature in Dec is more inline with the         average, and there are not many outliers skuing the average temperature higher or lower than the actual recorded frequency.



## Summary

Summarize the results and include two additional queries to perform to gather more weather data for June and Dec.

