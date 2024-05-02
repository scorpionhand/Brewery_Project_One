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

## Tyler
<blockquote>
Tyler Resources:
Census Data: https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_population
Brewery Count Data: State_Beer_Report_All.csv


Question 4: What is the population of each state? What is the ratio of Population per state to breweries per state?

Question 4 Analysis: The Top 10 most populated states are all located by a major body of water.
            Of those 10 only 4 have a population to brewery ratio over 10,000:1.

          The State with highest population to brewery ratio is Wyoming with a ratio around 32,835 citizens for every  1 brewery. 

          The State with the Lowest population to brewery ratio is Alabama with a ratio around 1,279 citizens for every 1 brewery.


Challenges:

GitHub: 
    At first I was struggling to comprehend how to add/delete/commit files and changes. I soon came to figure out that I was doing everything right, the only thing that I was forgetting was a git push command to push my changes to my branch. I soon figured out how to work github via the command line. 

Finding the data: 
    Finding the data was a struggle because not only I but the group as well was struggling to find accurate and reliable sources for a data without having to find a work around. We were able to find public information and data sets that were provided via government agencies and the always trusted source of wikipedia.

Writing the read_html() and actually getting the read_html syntax to work: 
    I was getting the table to pull up how I wanted but there was an extra header that was causing some headache. When I was creating the tables variable I specified that there was a header before the column headers began. This allowed me to remove the excess headers and then create a data frame with the table of data that I needed

Finding the sum of Brewery Count per state:
    At first I wasn't sure how to add the values without using a for loop. So that is the first place I started. I created a for loop that replaced every comma with a space so that I could write another for loop to add the brewery counts for the three quarters listed in the data set. 

Creating Graphs:
    In both graphs I struggled to call the correct column that was needed from each dataframe.
    I was able to fix this by reviewing my code making sure my data frames were correctly made and then I would copy the column header that was printed within the dataframe.
</blockquote>
