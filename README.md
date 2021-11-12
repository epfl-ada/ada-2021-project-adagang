# ada-2021-project-adagang

# Title: Black Lives Matter: How has the movement impacted the world?

# Abstract: 

  In 2013, the Black Lives Matter (BLM) movement emerged in response to the police brutality experienced by Black people in the United States. The movement has become increasingly popular, presumably due to the myriad protests that have been organized since its inception. However, its popularity has sparked mixed sentiment within America’s socio-political landscape. Thus, we analyze how select mediatized protests have impacted discourse and legislative action either in favor of or in opposition to the movement.
  
  To do so, we do a comparative analysis of BLM’s approval before and after each event by performing sentiment analysis over time on related quotes found in the Quotebank dataset. Further, we show how any potential attitude shifts differ by demographic group. We combine this analysis with data on what tangible socio-political change has been made as a result of these demonstrations. We hope our analysis serves to evaluate the efficacy of civic engagement. 


# Research Questions: 

Analyze the impact of events related to BLM/police brutality on discourse:
  - How does each event affect how often BLM/police brutality is talked about?
  - Do these events cause a positive or negative shift in how BLM is viewed?
  - How do demographics affect how each speaker reacts to an event?
  - What are the most impactful events and why? What are the characteristics of these events?

Analyze the impact of events related to BLM on legislation/politics
  - What type of police reform has occurred?
  - Police budgets (increase or decrease with calls to defund?) 
    - possible confounders here, budgets fluctuate for many reasons


# Proposed additional datasets (if any): 

We are still working through and deciding on which to use:
Police brutality data:
https://www.kaggle.com/ahsen1330/us-police-shootings
https://www.kaggle.com/washingtonpost/police-shootings → 2 different datasets to introduce the story, compare the proportion of people from different demographic groups killed by the police and show that there are significant problems with this.

https://www.kaggle.com/yash612/black-lives-matter-twitter-dataset → twitter dataset related to BLM with score depending if the tweet has a positive or a negative influence
https://www.kaggle.com/new-york-state/nys-hate-crimes-by-county-and-bias-type?select=hate-crimes-by-county-and-bias-type-beginning-2010.csv 
Library with different dataframes about BLM : policing and Incarceration


# Methods:

## Preliminary work
  - Pick 1 or 2 relevant events to analyze for each year
  - Establish a list of interesting keywords and interesting people to search in the quotations

## Data Wrangling
  - Quotebank dataset: explore data, extract all related quotes, visualization of amount of relevant quotes over time, are there any peaks? 
  - Speaker dataset: explore dataset, find relevant demographic information of all speakers in our related quotes dataset (race, ethnicity, gender identity, age,     political party affiliation, socioeconomic status?, occupation - politician, activist, other)

## Modeling
  - NLP
    - Sentiment Analysis of quotes
  - Clustering 
    - Cluster people into categories based on demographics and if their sentiment changed in positive or negative way (we will come up with a quantitative way to determine this) for each event 

## Data Visualization
  - Display demographics of our speakers to show who is active in the conversation surrounding the movement
  - Visualize clusters and change over time of both frequency and sentiment of quotes
  - Word maps of most frequent language used when talking about BLM (think positive might be “justice” negative might be “terrorist”, this could be impactful for the story aspect)


## Analysis
  - Make conclusions about our findings, figure out a way to present results
 
## Create Data Story



# Proposed timeline

By Friday November 19: Complete (a) in Methods. Complete (b) in Methods for the Quotebank dataset with final cleaned version.

By Friday November 26: Complete (b) in Methods for all external datasets we will use, decide more formally the role of each one in the project.

By Friday December 3: Have started (c) (i) and (ii) in methods. More specifically, find a model for sentiment analysis NLP (so we don’t have to train it all ourselves, not realistic) and begin setting up any functions needed for clustering and try some examples.

By Friday December 10: Finish modeling NLP and clustering (c)

By Friday December 17: Complete data visualization of our model and our findings on the datasets (d)

By Friday December 24: Discuss analysis of results and make final conclusions (e)

Over Break: Write Data Story (f)

# Organization within the team: 

## Preliminary work
  - Paula: Find events that are significant (I’m American so probably know best what were impactful events)
  - Clara: Establish list of keywords
 
## Data Wrangling
  - Paula & Danae: Speaker dataset: get it cleaned and have all important visualizations done, get it prepped for combining with Quotebank
  - Clara & Hugo: Quotebank Dataset: get it cleaned and have all important visualizations done, get it prepped for modeling
  - All: Additional datasets


## Modeling
  - Paula & Clara: NLP
  - Danae & Hugo: Clustering
  - All: How do we combine these techniques?


## Data Visualization
  - Paula & Hugo: time-series, visualize change in sentiment as a function of time
  - Danae & Clara: clustering visualizations


## Analysis
  - We do this together

## Create Data Story
  - We do this together and assign tasks when the time comes



# Questions for TAs (optional): Add here any questions you have for us related to the proposed project.

  - Is the use of keywords the best way to filter the quotations ? Aren’t we missing some quotations that talk about our subject but do not contain our keywords ?
  - On the opposite, are we including quotations that do contain the keywords but have nothing to do with police brutality ? 
  - If we therefore use groups of keywords, doesn’t it become too restrictive ? 
  - Finally what is the impact of those missing or extra quotations on our dataset given the huge number of quotations. 
