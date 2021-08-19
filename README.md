# surfs_up
analysis of weather data for a future surf shop


## Overview of the analysis
### Purpose
The purpose of this analysis was to use SQL Alchemy to connect Pandas and SQL to perform an analysis of weather data for a future surf shop. By connecting to a database, we can store the data, while still being able to perform session queries mapped to a specific point in the data using Python with Pandas. 

## Results
After analyzing the temperatures for June and December, there are a few differences that will be outlined in the points below. 
* Point 1: The average temperature in June is 74.94 F, while the average temperature in December is 71.04 F, so the June average temperature is about 4 F higher than the December average temperature. 
* Point 2: The quartile markers are 73 F (for 25% or Q1), 75 F (for 50% or Q2) and 77 F (for 75% or Q3) for June, and 69 F (for 25% or Q1), 71 F (for 50% or Q2) and 74 F (for 75% or Q3) for December. Temperatures in June were, on average, 3-4 F warmer than the corresponding quartile marker temperatures for December.
* Point 3: There are about 2000 fewer temperature measurements taken in December (1517) than in June (1700). Upon further analysis, I discovered that measurements were taken from 2010 through 2017 in June, but only 2010 through 2016 for December. It would be helpful to also have the 2017 December temperatures for an accurate analysis for each year. The standard deviation of each set of temperatures (June and December) are relatively equal, however, the December standard deviation is a little larger, which could be affected by the smaller data set, which typically have more variance. 

### Deliverable 1: Determine the summary statistics for June temperatures

<img width="837" alt="Screen Shot 2021-08-17 at 12 50 36 PM" src="https://user-images.githubusercontent.com/85946042/129776450-fe5438a8-4299-41ca-9ae4-8e027f588ec2.png">
<img width="183" alt="Screen Shot 2021-08-17 at 12 50 51 PM" src="https://user-images.githubusercontent.com/85946042/129776462-8dbe834a-9704-45ab-a6e6-107c809ea97a.png">


### Deliverable 2: Determine the summary statistics for December temperatures

<img width="725" alt="Screen Shot 2021-08-17 at 12 51 39 PM" src="https://user-images.githubusercontent.com/85946042/129776495-b843497b-2e41-4804-ada0-ba3bae325a63.png">
<img width="173" alt="Screen Shot 2021-08-17 at 12 51 48 PM" src="https://user-images.githubusercontent.com/85946042/129776504-6f75aecf-92f6-4405-bbeb-78024641e848.png">


## Summary

There is a high-level summary of the results and there are two additional queries to perform to gather more weather data for June and December.

### Additional Query 1:
For the first additional query, I wanted to see how average temperature in each month is affected by date. For this query, I created a dataframe where I could see the average temperature for each day in the month. This is useful for graphing, where we could see if the temperatures tend to change as the month progresses. 
<img width="913" alt="Screen Shot 2021-08-17 at 3 05 38 PM" src="https://user-images.githubusercontent.com/85946042/129796350-68bc7855-3599-4274-b543-722570b537e4.png">

### Additional Query 2:
For the second additional query, I wanted to see how the average temperatures in each month differed from year to year. I created a dataframe where I could see the average temperature for each year for each of the months. Then, I graphed the temperature data over the years. This could be useful when studying climate change, or other difference in temperature over the years. If there was a natural disaster or another phenomena, we could see how the temperature was affected compared to other years' historical data. 
<img width="748" alt="Screen Shot 2021-08-17 at 3 29 12 PM" src="https://user-images.githubusercontent.com/85946042/129796391-b6f0f43c-9a87-4c44-b649-0937af5c6ec0.png">
<img width="740" alt="Screen Shot 2021-08-17 at 3 30 54 PM" src="https://user-images.githubusercontent.com/85946042/129796400-1ac51e7e-00b9-411c-8026-92359bf19eea.png">



