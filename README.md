# Brewery_Project_One

## Data Sources:
[Brewery API](https://www.openbrewerydb.org/documentation/)<br/>
[Consumption Rate List](https://beerinfo.com/beer-consumption-by-state-per-capita/)<br/>
[Geoapify](https://www.geoapify.com/)<br/>
[Census Dat](https://www.census.gov/popclock/data_tables.php?component=pyramid)<br/>
[Income Data](https://apps.bea.gov/itable/?ReqID=70&step=1&_gl=1*hwmef0*_ga*MjAyODIxNjI2My4xNzEzO[…]k1*_ga_J4698JNNFT*MTcxMzkyMzA1Ny4yLjAuMTcxMzkyMzA1Ny42MC4wLjA.)<br/>
https://github.com/scorpionhand/Brewery_Project_One.git<br/>
[TTB (Alcohol and Tobacco Tax and Trade Bureau)](https://www.ttb.gov/regulated-commodities/beverage-alcohol/beer/statistics)<br/>

## Roles: 

| Name  | Title               | Tasks            |
| ----- |:-------------------:| ----------------:|
|John   | Repository Manager  | Question 1 <br/> |
|Austen | Presenter           | Question 2 <br/> |
|Matt   | Data Collector      | Question 3<br/>  |
|Tyler  | Question Master     | Question 4 <br/> |
|Daryn  | Presentation        | Question 5 <br/> |
|Group  |                     | Question 6 & 7 <br/>|

[Reference Notes](https://onedrive.live.com/edit?id=85BF7DBA461D47A1!591&resid=85BF7DBA461D47A1!591&ithint=file%2cdocx&authkey=!AFe-S1QVE67xLmc&wdo=2&cid=85bf7dba461d47a1)<br/>
***
## Questions
  1. What is the number of breweries per state? 
  2. Is there a correlation in consumption rate to the number of breweries each state? 
  3. Is there a correlation of Average Income to the number of breweries per state? 
  4. What is the population of each state? 
  5. Is there a correlation to state population and number of breweries? 
  6. Show the consumption rate in the U.S. over the last x years? 
  7. Show the consumption rate over the years. Plot the head() and the tail(). 


Matt Resources and analysis:
  1. Brewery per state info brought in via API from openbrewerydb.org
  2. Geoapify plotted brewery/pub and micro brewery on map
  3. average income CSV received from https://worldpopulationreview.com/state-rankings/average-income-by-state
  
  Analysis:
  Looking at the data, there were more breweries, and brewery types, then originally thought by myself.  We brought in over 8000 per openbrewerydb and then removed all other countries bringing the total to 5736.  Some of the data didn't have Lat/long so those were removed to bring the dataset to 5524 breweries.  California leaded the most with this dataset with 904 with second being Washington at 423.  When the data was mapped, it appears that majority of the breweries are near a body of water.  Either being on a coast or near a large lake body.  Import/Exports would have been the next step to look for and compare with ports and brewery locations, but unable to find necessary data in timeframe.

  We had an initial question of average income per state with breweries and if there was a correlation.  After bringing in the income and merging the files, the data was placed onto a scatter plot.  The correlation was a .07 and the graph indicated there was no correlation.  

  Challenges Matt experienced during project:
  1. Github, merging caused some confusion and I was pushing stuff up but after the merge I thought I lost some of my data and started over at one point.  Ben had to assist with merging, and pulling within github and my computer.
  2. API Call, My api call weren't working and John on our team found a solution and we used his coding solution and that ultimately worked.
  3. GeoApify plotting, Used same code segment from last homework assignment and it gave an error indicating that longitude and latitude were unreadable.  Benjamin came in and assisted with casting longitude and latitude into integers.  John found solution by using pd.to_numeric function.
  