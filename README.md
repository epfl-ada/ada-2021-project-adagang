# ada-2021-project-adagang

# Title: Black Lives Matter: How has the movement impacted the world?

# Abstract: 

  In 2013, the Black Lives Matter (BLM) movement emerged in response to the police brutality experienced by Black people in the United States. The movement has become increasingly popular, presumably due to the myriad protests that have been organized since its inception. However, its popularity has sparked mixed sentiment within America’s socio-political landscape. Thus, we analyze how select mediatized protests have impacted discourse and legislative action either in favor of or in opposition to the movement.
  
  To do so, we do a comparative analysis of BLM’s approval before and after each event by performing sentiment analysis over time on related quotes found in the Quotebank dataset. Further, we show how any potential attitude shifts differ by demographic group. We combine this analysis with data on what tangible socio-political change has been made as a result of these demonstrations. We hope our analysis serves to evaluate the efficacy of civic engagement. 


# Research Questions: 

Analyze the mediatization of BLM after a police officer killed a black person:
  - How does each kill affect and how often BLM is talked about?
  - Do these events cause a positive or negative shift in how BLM is viewed?
  - How do demographics affect how each speaker reacts to an event?
  - What are the most impactful events/crime and why?

[comment]: <> ( Analyze the impact of events related to BLM on legislation/politics ) 
[comment]: <> (  - What type of police reform has occurred? )
[comment]: <> (  - Police budgets, increase or decrease with calls to defund?) 
[comment]: <> (    - possible confounders here, budgets fluctuate for many reasons  )


# Additional datasets used: 

[comment]: <> (We are still working through and deciding on which to use:)
[comment]: <> (Police brutality data:)
[comment]: <> (https://www.kaggle.com/ahsen1330/us-police-shootings)
[comment]: <> (https://www.kaggle.com/washingtonpost/police-shootings → 2 different datasets to introduce the story, compare the proportion of people from different demographic groups killed by the police and show that there are significant problems with this.)

[comment]: <> (https://www.kaggle.com/yash612/black-lives-matter-twitter-dataset → twitter dataset related to BLM with score depending if the tweet has a positive or a negative influence)
[comment]: <> (https://www.kaggle.com/new-york-state/nys-hate-crimes-by-county-and-bias-type?select=hate-crimes-by-county-and-bias-type-beginning-2010.csv 
Library with different dataframes about BLM : policing and Incarceration)

We finally used only 1 extra dataset to introduce and motivate the project. The dataset was found on the Washington Post website: https://www.washingtonpost.com/graphics/investigations/police-shootings-database/ .
It contains all the persons shoot by US police between 2015 and today. 


# Methods:

## Preliminary work
 [comment]: <> ( - Pick 1 or 2 relevant events to analyze for each year)
  - Establish a list of interesting keywords and interesting people to search in the quotations

## Data Wrangling
  - Quotebank dataset: explore data, extract all related quotes, visualization of amount of relevant quotes over time, are there any peaks? 
  - Speaker dataset: explore dataset, find relevant demographic information of all speakers in our related quotes dataset (race, ethnicity, gender identity, age,     political party affiliation, socioeconomic status?, occupation - politician, activist, other).
  - Pick the most cited black persons who were killed by US police to perform some correlations with the found peaks of relevant quotes.

## Modeling
  - NLP
    - Sentiment Analysis of quotes
  - Sementic analysis based on lexical categories and topic detection
    - Find relevant topics, keywords and relevant people to analyze and correlate with the quotes dataset 
  - Clustering
    - Cluster people into categories based on demographics and if their sentiment changed in positive or negative way (we will come up with a quantitative way to determine this) for each event 

## Data Visualization
  - Display demographics of our speakers to show who is active in the conversation surrounding the movement.
  - Visualization to introduce the datastory (map and some facts)
  

 [comment]: <> (  - Visualize clusters and change over time of both frequency and sentiment of quotes)
 [comment]: <> (  - Word maps of most frequent language used when talking about BLM, think positive might be “justice” negative might be “terrorist”, this could be impactful for the story aspect)


## Analysis
  - Make conclusions about our findings, figure out a way to present results
 
## Create Data Story



# Initial proposed timeline from P2 to the final deliverable

By Friday November 19: Complete (a) in Methods. Complete (b) in Methods for the Quotebank dataset with final cleaned version.

By Friday November 26: Complete (b) in Methods for all external datasets we will use, decide more formally the role of each one in the project.

By Friday December 3: Have started (c) (i) and (ii) in methods. More specifically, find a model for sentiment analysis NLP (so we don’t have to train it all ourselves, not realistic) and begin setting up any functions needed for clustering and try some examples.

By Friday December 10: Finish modeling NLP and clustering (c)

By Friday December 17: Complete data visualization of our model and our findings on the datasets (d)

By Friday December 24: Discuss analysis of results and make final conclusions (e)

Over Break: Write Data Story (f)

# Organization within the team during the project: 

## Preliminary work
  - Together: Find preliminary set of significant events/people
  - Clara & Danae: Establish list of keywords, first by ourselves, an then by topic detection but it didn't get us anywhere...
 
## Data Wrangling
  - Paula & Danae: Speaker dataset: get it cleaned and have all important visualizations done, get it prepped for combining with Quotebank
  - Clara & Hugo: Quotebank Dataset: get it cleaned and have all important visualizations done, get it prepped for modeling
  - Hugo & Paula: Analyze if the extra dataset can be useful and make some visualizations with to introduce the data story


## Modeling
  - Paula & Danae: NLP, obtain a usable sentiment analysis. After many iterations to improve the model, it wasn't accurate enough and we were not able to make conclusion
  - Danae: Sementic analysis based on lexical categories in order to improve the selected keywords
  - Clara & Danae & Hugo : Name entity recognition to select by hand most relevant cited names associated with BLM in order to perform correlations between the death of some of these people and the occurence of our quotations
  - Hugo & Clara: Perform clustering on speakers but it did not yield anything interpretable...

## Data Visualization
  - Paula & Clara & Danae: time-series, visualize change in sentiment as a function of time
  - Hugo & Clara: Make visualizations with the speakers attributes and the total generated quote dataset


## Analysis
  - All together

## Create Data Story
  - All together

# Main issue:
Unfortunately we were not able to carry out our project as initially hoped. Our analysis had to be based on sentiment analysis and we tried different methods to make it work but event after several iterations, we could not find a solution. Indeed, we realized that our keywords like "BLM", "police brutality" had very often a negative connotation. Some quotations that had a positive meaning for us, also gave a negative sentiment score, depending on how the sentence was turned. This completely skewed our results and we were not able to perform certain methods and analyses correctly.

[comment]: <> (# Questions for TAs optional: Add here any questions you have for us related to the proposed project.)

[comment]: <> (  - Is the use of keywords the best way to filter the quotations ? Aren’t we missing some quotations that talk about our subject but do not contain our keywords ?)
[comment]: <> (  - On the opposite, are we including quotations that do contain the keywords but have nothing to do with police brutality ? )
[comment]: <> (  - If we therefore use groups of keywords, doesn’t it become too restrictive ? )
[comment]: <> (  - Finally what is the impact of those missing or extra quotations on our dataset given the huge number of quotations. )
