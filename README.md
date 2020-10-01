# Team-2-repo

This is the repository for Project 1 / Team 2 (Jordan Schafer and Steve Freeland).

Our project involved the analysis of consumer reviews of beer brands to discover insights around correlation between overall and various category review scores.

Project work included the gathering of relevant data, cleaning of data, generation of multiple scatter plots, conducting an ANOVA exercise, and generation of a heatmap. Further detail around each step follows:

Data:
Data was gathered from kaggle.com (specifically Beer Reviews) as well as the Google Maps Places / Geolocations API. 
Data cleaning steps included:
Grouping of data by beer_beerid, finding mean review scores and review count for each beer, filtering on those beers with greater than 50 reviews. Brewery information was extracted. Using the Google API a retrieval of latitude, longitude, and address for each brewery was performed; subsequently removed those breweries with no results. Country of origin detail was extracted from address data. Finally, beer review data was merged with brewery information, removing those beers with no brewery information.

While this project focused on U.S. brewery data, we did conduct a brief analysis around rest of world data.

Multiple questions were addressed in this study:
What is the best beer in each review category?
Is there a correlation between category review and Overall Review score? Several sub-questions were addressed:
  Is there a correlation between Aroma and Overall Review?
  Is there a correlation between Appearance and Overall Review?
  Is there a correlation between Palate and Overall Review?
  Is there a correlation between Taste and Overall Review?
  Is there a correlation between ABV (Alcohol by Volume) and Overall Review?
  Is there a correlation between Overall Review score and the number of reviews performed?
Perform ANOVA comparing most common beer types to see if significant differences exist across Overall Review score
Create heatmap of breweries (Where can I get a beer?)

Conclusions and Learnings:
Aroma, Appearance, Palate, and Taste highly correlate with Overall Review scores.
ABV (Alcohol by Volume) is not highly correlated with beer review scores, possibly indicating beer consumers do not care about this product aspect as much as others.
There is no linear correlation between Number of Reviews and Overall Review score. 
The most influential factor across these factors appears to be Aroma.  

Limitations of Data Set:
Results based on user response data
Only analyzed beer with >50 ratings
No sales data available
No pricing data available
No IBU ratings included in data set
The inclusion of such data would likely produce even more meaningful results.

ANOVA - Do Beer Styles make a significant difference in Overall Review scores?
Null Hypothesis: Beer styles do not make a significant difference in Overall Review score
Alternative Hypothesis: Beer styles do make a significant difference in Overall Review score
For ANOVA test we concentrated on the five most common styles
Running the ANOVA function yields a p-value of 0.00017
This is evidence that the alternative hypothesis of Beer styles do make a significant difference in Overall Review score is true
