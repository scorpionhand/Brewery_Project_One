# Brewery_Project_One Analysis

[Team Reference Notes](https://onedrive.live.com/edit?id=85BF7DBA461D47A1!591&resid=85BF7DBA461D47A1!591&ithint=file%2cdocx&authkey=!AFe-S1QVE67xLmc&wdo=2&cid=85bf7dba461d47a1)<br/>
***
## Questions
<ul>
  <li>What is the number of breweries per state? </li> 
  <li>Is there a correlation in consumption rate to the number of breweries each state? </li>  
  <li>Is there a correlation of Average Income to the number of breweries per state? </li>  
  <li>What is the population of each state? </li>  
  <li>Is there a correlation to state population and number of breweries? </li>  
  <li>Show the consumption rate in the U.S. over the last x years? </li>  
  <li>Show the consumption rate over the years. Plot the head() and the tail().</li>   
</ul>


## Matt Resources and analysis:
<blockquote>
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
</blockquote>

## Austen Resource and Analysis:
2. Question: Is there a correlation in consumption rate to the number of breweries each state?
Data from https://beerinfo.com/beer-consumption-by-state-per-capita/

Analysis: 

o	Right off the bat, we can see that there is going to be an outlier in California. The # of breweries is drastically higher than almost all of the other states equaling 4, even 5 times the amount. While alcohol consumed by state is a little closer together. Although, a number of our highest producing states of breweries have actually some of the lowest #s of alcohol consumed when comparing inside our DF. 

o	Generating a basic scatter plot, we can see that our plot is pretty bundled together indicating little to no correlation. Plotting our line and printing our R Value, you can see that the scatter plot has an actual negative correlation between our two values, sitting at -.24. This means the states with most breweries are states that are drinking the least. This at the very least indicates that the # of Breweries Per State is driven by a separate factor.

 Challenges Austen experienced during project:
 1. Everything github, even though I feel much more comfortable with it after this project. Moving between branches, while pushing and pulling has been a struggle. The main problem being conflicting files. I talked to Ben and we were able to run through the solution. 
 2. Real basic problem but when I was trying to pull a simple CSV file in I was unable to work out what I was doing wrong. After a while, I happened to check the CSV and I had renamed it with a typo so I was pulling the wrong name the entire time. 