# texas-political-shifts
Investigating political shifts in Texas with election data from 2000-2024 with R

# INTRODUCTION
The topic under study for our Exploratory Data Analysis is the political shifts of Texas in Presidential elections from 2000 to 2024. Specifically, we want to see how the trend of Texas getting more competitive changed in 2024. Using this data, we may learn what key areas of Texas may have resulted in the reversing of trends in the 2024 Presidential election.

# BACKGROUND
IMPORTANT INFORMATION TO KNOW: For context, Presidential elections are held every 4 years in the United States. Since 2000, 7 Presidential elections have occurred (including 2024). In each of these elections, Texas voted for the Republican candidate for the Presidency, but has become more and more competitive as Texas was shifting closer and closer to the Democratic Party from 2000 to 2020. This trend reversed in 2024 when the Republican candidate for President won Texas by nearly 14%. Additionally, it is important to know that in American politics, the two major parties are the Democratic (typically denoted with the color blue) and the Republican parties (typicalled denoted with the color red). These are not the only parties that ran presidential candidates, but for the purpose of this analysis, they will be the two parties of focus.

# DATASETS
We used three datasets for this project. The first one is from MIT Election Lab which includes Presidential election results for every county in the U.S. from 2000-2020. After having filtered the dataset for Texas, we awaited the results of the 2024 Presidential election in Texas. After the election, we found a dataset from the Texas Secretary of State. We then joined the two datasets so that we could have a full set of data for Presidential election results from 2000 to 2024. The final dataset we used was a shapefile dataset from the Texas Department of Transportation for making the map of Texas.

DATASET 1 (MIT ELECTION LAB): The dataset from the MIT Election Lab has 72617 observations of 6 variables with 4572 of those observations pertaining to Texas. Some important variables included are year, state, county_fips, county_name, party, candidatevotes, and totalvotes. For the purpose of this analysis, all these variables are important except totalvotes because they will be used in generating visualizations.

DATASET 2 (TEXAS SECRETARY OF STATE): The dataset from the Texas Secretary of State has 254 observations of 7 variables. The important variables for this analysis are county_name, REPUBLICAN, DEMOCRAT, and OTHER. The other variables are not necessary for our analysis. This dataset was then joined to DATASET 1 so that we could have the Presidential election results for all counties in Texas from 2000 to 2024.

DATASET 3 (TEXAS DEPARTMENT OF TRANSPORTATION): The dataset from the Texas Department of Transportation was a shapefile, so it was mainly used for mapping. We joined this file to our other datasets to create the maps.

# VISUALIZATIONS
Total Votes Cast Visualization

This plot shows the total number of votes cast in Texas Presidential elections from 2000 to 2024. We thought this may be interesting to see whether voter turnout affected the results of the race.


Number of Competitive Counties Chart

This plot shows the total number of counties in Texas in which one of the major political parties won >45% of the vote or <55% of the vote. We created this to try to see if there was a trend in Texas where the number of competitive counties corresponded to te competitiveness of the statewide race.


Number of Votes Cast for Each Major Party Visualization

This plot shows the number of votes each party received in Texas Presidential elections from 2000 to 2024. This visualization is important to understanding the political trends in Texas' voting behavior.


Faceted Histogram Showing Democrat, Competitive, and Republican Counties over Time

This plot shows the shifts in county competitiveness in Texas Presidential elections from 2000 to 2024. As seen in the visualization, concentration of non-competitive counties won by the Republican party has shifted rightward over time, meaning that these Republican counties have voted for the Republican candidate by larger margins over time. This visualization may be valuable in understanding the polarization of Texans between the two major parties.


Texas Presidential Election Results Maps

This plot shows 7 maps detailing the results of Texas Presidential elections by county from 2000 to 2024. We created this to try to see where political shifts are happening within the state.


Competitive Counties Maps

This map will highlight counties classified as "COMPETITIVE" (where the difference between the Democratic and Republican vote percentage is ≤5%) for each election year. This will give us a glimpse into whether Texas has gotten more or less competitive.
