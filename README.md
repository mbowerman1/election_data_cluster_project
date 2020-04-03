# Comparing Baltimore City Voter Turnout by Precinct in 2016 and 2018

## Business Question
What was voter turnout generally like in Baltimore City in 2016 and 2018? How could it be improved in 2020 and beyond?
1. Which precincts have better turnout? 
2. Do those rankings fluctuate between the primary and general elections and between years? 
3. Was there a visible change in turnout between 2016 and 2018, in light of the civil and social context of the 2018 election?

## Data Question
1. What are the general characteristics of the clusters for the four datasets (2016 Primary Election, 2016 General Election, 2018 Primary Election, and 2018 General Election)?
2. Which attributes signify the direction of voter turnout, based on the cluster nodes?
3. Is there any relationship between each political party's voter turnout per precinct and the cluster characteristics?

## Data Analysis Methodology
Baltimore City election data was found using the [Maryland State Board of Elections website](https://elections.maryland.gov/elections/2016/index.html "State Board of Elections").
I pulled the Baltimore City precincts data using the filter function. The numbers of votes cast and eligible voters for each precinct were grouped by political party, so I summed each attribute for each precinct to find total votes cast and voter turnout, regardless of party. I then did a three-node cluster analysis of each dataset.

After performing cluster analysis, I noticed that each cluster had a node with all attributes above the mean, a node with some attributes above and some below the mean, and a node with all attributes below the mean. I teaked the numbers such that the nodes described were #1, #2, and #3 respectively for each dataset, without changing the cluster distribution or minimized sum of the squared distances. This made the cluster characteristics nearly identical across the board, so I could analyze the significance of a precinct changing clusters from election to election. The characteristics of each node and cluster distribution are outlined in the tables below.

## Findings
![](Visualizations)
![](Visualizations)

As the tables show, a slight majority of precincts stayed in the same cluster, demonstrating either consistently above average, average, or below average voter turnout. Most of the remaining precincts fluctuated between two clusters with only three precincts fluctuating between all three clusters. Interestingly, the precincts of the two-cluster group never jumped between clusters 1 and 3, only ever fluctuating between 1 and 2 or 2 and 3, as seen in the "Visualizations and Final Clusters" dataset. In other words, only three precincts had both above average and below average voter turnout across the four elections surveyed; all other precincts either stayed in their lane (i.e. cluster) or fluctuated between above average and average, or below average and average.

![](Visualizations)

Additionally, the above data for Baltimore City average voter turnout was also retrieved. While it was no surprise that voter turnout is greater in general elections compared to primaries, I was very surprised to find how much voter turnout dropped from 2016 to 2018. In light of the civic and social context of the 2018 election, I had expected to see the opposite trend. In fact, Baltimore's voter turnout in the 2018 general election was markedly lower than the national average of 53.4%. Conversely in 2016, Baltimore was much closer to the national average of 61.4%. National turnout averages were retrieved from the United States Census Bureau and Pew Research Center websites: [2016 Primary](https://www.pewresearch.org/fact-tank/2016/06/10/turnout-was-high-in-the-2016-primary-season-but-just-short-of-2008-record/ft_16-06-08_primaryturnout/), [2016 General](https://www.census.gov/newsroom/blogs/random-samplings/2017/05/voting_in_america.html), [2018 Primary](https://www.pewresearch.org/fact-tank/2018/10/03/turnout-in-this-years-u-s-house-primaries-rose-sharply-especially-on-the-democratic-side/), and [2018 General](https://www.census.gov/library/stories/2019/04/behind-2018-united-states-midterm-election-turnout.html).

This data could be useful for targetting particular precincts in a bid to increase voter turnout, as it shows both precinct voter turnout and their consistency over different elections. However, it would benefit from further analysis of the factors impacting voter turnout, as well as a survey of any changes in eligible voter numbers between these elections. The fact that both national and Baltimore turnout dipped in 2016 is very interesting and worth further exploration.
