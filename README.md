# Brewery_Project_One
Module 7 Challenge


Question 4: What is the population of each state? What is the ratio of Population per state to breweries per state?

Analysis: The Top 10 most populated states are all located by a major body of water.
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


