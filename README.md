# Comparing Baltimore City Voter Turnout by Precinct in 2016 and 2018

## Business Question
What was voter turnout generally like in Baltimore City in 2016 and 2018? How could it be improved in 2020 and beyond?
1. Which precincts have better turnout? 
2. Do those rankings fluctuate between the primary and general elections and between years? __Consistently or inconsistently with eligible voter numbers?__
3. Was there a visible change in turnout between 2016 and 2018, in light of the civil and social context of the 2018 election?

## Data Question
1. What are the general characteristics of the clusters for the four datasets (2016 Primary Election, 2016 General Election, 2018 Primary Election, and 2018 General Election)?
2. Which attributes signify the direction of voter turnout, based on the cluster nodes?
3. Is there any relationship between each political party's voter turnout per precinct and the cluster characteristics?

## Data Analysis and Findings
Baltimore City election data was found using the [Maryland State Board of Elections website](https://elections.maryland.gov/elections/2016/index.html "State Board of Elections).
[Maryland State Board of Elections website](https://elections.maryland.gov/elections/2016/index.html "State Board of Elections")
I pulled the Baltimore City precincts data using the filter function. The numbers of votes cast and eligible voters for each precinct were grouped by political party, so I summed each attribute for each precinct to find total votes cast and voter turnout, regardless of party. I then did a three-node cluster analysis of each dataset.

_Findings in 250 words __or less___

__Findings in 250 words or less: What are the characteristics of each cluster node? How consistent was precinct voter turnout? What do these two answers mean for how this information can/should be used? What additional data might be useful for further analysis?
Include _visualization_ of groupings of cluster analysis (list of data for each cluster) and/or characteristics of cluster nodes__
