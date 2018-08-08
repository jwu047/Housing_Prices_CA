# Factors Affecting Housing Prices in California
Danielle Rogacion, Jason Wu, Phuong Dong, Tiffany Chien, Xiyue Deng
##  Questions & Data
### Hypothesis: 
City demographics affects housing prices
### Questions: 
What are the major factors that determine home values? Do population, age, ethnicity, climate, latitude, income, poverty rate, employment rate and/or crime rate play a role?  
### Data Source
Census API - Population, Median Age, Ethnicity, Median Household Income, Median Home Value, Average Rent, Poverty Rate, Employment Rate by Zip Code  
* [Click here for Notebook](/Data/CA_Census_Data.ipynb)  
* [Census Data](/Data/census_data.csv)  
Zillow Data - Zipcodes’  City Name, County Name, 2016 Average Home Value  
* [Zillow Data](/Data/Zip_Zhvi_AllHomes.csv)
* [Click here for Notebook](/Data/Zillow_CA_ZipCode_HomeValue_2016.ipynb)  
Open Weather API - City Temperature, Latitude and Longitude
* [Weather and Coordinates Data](/Data/Combined_loc_CA.csv)  
FBI: Uniform Crime Report - City Offenses Count, City Law Enforcement Employees  
* [Offenses Data](/Data/City_Offenses.xls)  
* [Law Enforcement Data](/Data/City_Law_Enforcement.xls)  
Google Map API -  California Whole Foods Market and Walmart Coordinates  
* [Click here for Walmart Location Notebook](/Data/Walmart_Location_In_California.ipynb)
* [CA Walmart Data](/Data/Walmart%20CA%20Location.csv)  
* [Click here for Whole Foods Market Location Notebook](/Data/WholeFoods_Location_In_California.ipynb)
* [CA Whole Foods Market Data](/Data/Whole%20Foods%20CA%20Location.csv) 
## Analysis
* [Click here for Notebook](/CA_HomeValue_Analysis_Main.ipynb)  
  
Home Value vs Population  
![2016 Median Home Value vs population](/Images/2016%20Median%20Home%20Value%20vs%20population.png)  
P-value is 0.0006057986255214741  
  
Home Value vs Age  
![2016 Media Home Value vs Median Age and Population](/Images/2016%20Media%20Home%20Value%20vs%20Median%20Age%20and%20Population.png)  
P-value is 1.8119773237169143e-34  
![2016 Median Home Value by Age (Bar Chart)](/Images/2016%20Median%20Home%20Value%20by%20Age%20(Bar%20Chart).png)  
  
Home Value vs Ethnicity  
![MinorityPopulationInCounties_and_MedianHomeValues](/Images/MinorityPopulationInCounties_and_MedianHomeValues.png)  
p-value for %Hispanic population & Median home value: 0.5927314329741257, --> no correlation.  
p-value for %Black population & Median home value: 0.6564546628142199, --> no correlation.  
  
Home Value vs Temperature  
![City Temperature vs. Median Home Value](/Images/City%20Temperature%20vs.%20Median%20Home%20Value.png)  
P-value is 1.2547052677355456e-32  
  
Home Value vs Latitude  
![City Latitude vs. Median Home Value](/Images/City%20Latitude%20vs.%20Median%20Home%20Value.png)  
P-value is 0.005104750038080612   
  
Home Value vs Household Income  
![2016 Media Home Value vs Household Income and Population](/Images/2016%20Media%20Home%20Value%20vs%20Household%20Income%20and%20Population.png)  
P-value is 1.9569578295545415e-237  
![2016 Median Home Value by Income (Bar Chart)](/Images/2016%20Median%20Home%20Value%20by%20Income%20(Bar%20Chart).png)   
   
Home Value vs Poverty Rate   
![2016 Media Home Value vs Poverty Rate](/Images/2016%20Media%20Home%20Value%20vs%20Poverty%20Rate%20and%20Population.png)  
P-value is 8.081803490434749e-81  
   
Home Value vs Employment Rate  
![2016 Media Home Value vs employment rate](/Images/2016%20Media%20Home%20Value%20vs%20employment%20rate.png)  
P-value is 2.1184263274346533e-49  
   
Home Value vs Crime Rate  
![CA_City_Crime_Rate_vs_Home_Value](/Images/CA_City_Crime_Rate_vs_Home_Value.png)  
p-value is 2.9005656836394537e-13  
   
Based on the analysis we did, it shows home value does correlation with population, age, temperature, income, provety rate, employment rate and crime rate.   
But there is correlation with %Hispanic population and %Black population, based on the current data set.   
  
#### An interesting insight that came up during data exploration...  
Is there a relationship between business establishments, specifically grocery stores, and housing prices?   
Is Whole Foods, a high-end organic supermarket, located in more affluent areas?   
Is Walmart, a low-priced hypermarket, located in lower-income areas?  
  
#### Whole Foods Market and Walmart Locations on Home Value Heatmap  
Markers are Whole Foods Markets, bule dots are Walmarts.  
Based the heatmap below, we can see most of the whole foods markets locationed around High Home Value Area;  
Walmart has more stores in california, but the locations are around lower home value neiborhood.
![Whole_Foods_Walmart_Home_Value_Heat_Map](/Images/Whole_Foods_Walmart_Home_Value_Heat_Map.png) 
