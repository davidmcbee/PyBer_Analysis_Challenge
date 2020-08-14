# PyBer_Analysis_Challenge

you’ll submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.

## Analysis Overview
### Purpose
The purpose of this analysis is to provide insights that will allow for actions that will improve access and affordability for underserved neighborhoods.

### Overview
This analysis looks at drivers, number of rides, number of drivers, average fare by ride, and average fare by driver. The data is also segregated by city type. These are rural, suburban and urban.
### How the Analysis was Conducted
#### Data
This analysis was conducted based off the data provided in two files. The first file is the city_data.csv file which shows the city, the driver count for each city and the city type.
The second file is the ride_data.csv file which shows the city, date of the ride, the fare for that ride and the ride ID. Both files span the period from 1 Jan 2019 through 5 May 2019.
#### Steps Conducted
1. After some plotting practice the files were reviewed to make sure the data did not need to be cleaned, which it did not, both files were merged on city to get a combined view.
2. Using Pandas, the data was broken out into city type. The the number of rides per the city types was summed up, the driver count per city type was summed and the fares were
 summed by city type. Based o that information the average fare per ride and average fare per rider was calculated.  
3. Using this information the data was pivoted and the dates were set as the index in preparation to create a graph. A line chart raph was created that shows the fare amounts over the time frame by city type.
#### Tools used
Python was used within the Jupyter devevelopment environment. The Pandas, Matplotlib.pyplot and Matplotlib styles are libraries that were used to take advantage of data framing
 and data manipulation (the Pandas library), and to create various graphics using the tools available in the Matpolotlib.pyplot library and styles functionality.  
### Results
The results are based on the below summary statististics and graph.
#### Summary Statistics
In looking at the summary statistics shown in table 1 there is an increasing quanity of total rides, total drivers and and increasing amount in total fares from rural to suburban to urban city types.
 The highest average fare per ride was for the rural city type as is the average fare per driver. Though the rural total rides were the lowest of all three city types, the average fares per ride and per driver were the highest.
 An assumption at this point is that this is due to increased distances in rural areas, though this should be verified. Another variation worth noting is that the rural city type had the largest differnce bewteen average fare 
per rid and average fare per driver, $20.87. The differences for suburban and urban are $8.53 and $7.96 with the urban city type being the only type to have a higher avergae fare per ride then the average fare per driver. 
#### Total Fare by City Type Graph
This graph shows the fares in U.S. dolars for each fare  based on city type per week for the time frame of the data. Looking at it one can see a number of items of interest:
1. The difference in fares follows the sumamry statistices. The urban fares are the largest. the average is $2,037 dollars. The suburban average is $990 and the rural average fare for the week is $208.
2. The fares for all 3 city types follow the same pattern up until midway through. At the begining of April there is a significant dip for both the urban and suburban city types.
 This is born out in that the standard deviation for the rural fare by week, which is 88.65. Compare this to the standard devitation for the suburban city type, 256.9 and 422.32 for the urban city type.
3. This inconsistency between rural city type and the suburban and urban city types does not appear in late February. All three city types spiked fairly consistently.
### Summary and Recommendations
Keeping acccess and affordability in mind, the following recommendations and areas of further study are provided.
1. given the largest average fare per driver, and the largest difference between average fare per ride as compared to average fare per driver is in the rural area, we might want to do two things:
 a. conduct further analysis on rural cities to see if this is consistent across all rural cities.
 b. work to increase the number of drivers in the rural area.
Though the rurual city type is the least profitable, this could bring the average fare per ride down as well as increase rides, and hopefully profit, in the steadiest area of the thre.
2. Find out what caused the dip at the begining of April that affected the urban and suburban city types but not the rural city type. The hope is that this is controllable, at least to a degree.
3. Find out what caused the spike in late February. Again, if this is controllable we could promote this.
4. Further sensitivity analysis to compare driver saturation verses average fare per ride should be conducted to find the maximum quantity of drivers we should target in each of the three city types.

