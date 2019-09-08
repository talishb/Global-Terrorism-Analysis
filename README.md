## Global Terrorist Dataset 

About the Dataset - Download from -https://www.kaggle.com/START-UMD/gtd

From Kaggle:

Information on more than 180,000 Terrorist Attacks

The Global Terrorism Database (GTD) is an open-source database including information on terrorist attacks around the world from 1970 through 2017. The GTD includes systematic data on domestic as well as international terrorist incidents that have occurred during this time period and now includes more than 180,000 attacks. The database is maintained by researchers at the National Consortium for the Study of Terrorism and Responses to Terrorism (START), headquartered at the University of Maryland. More Information

Content
Geography: Worldwide

Time period: 1970-2017, except 1993

Unit of analysis: Attack

Variables: >100 variables on location, tactics, perpetrators, targets, and outcomes

Sources: Unclassified media articles (Note: Please interpret changes over time with caution. Global patterns are driven by diverse trends in particular regions, and data collection is influenced by fluctuations in access to media coverage over both time and place.)

Definition of terrorism:

"The threatened or actual use of illegal force and violence by a non-state actor to attain a political, economic, religious, or social goal through fear, coercion, or intimidation."

See the GTD Codebook(http://start.umd.edu/gtd/downloads/Codebook.pdf) for important details on data collection methodology, definitions, and coding schema.

## Goal
While inspecting this data set, I realised there are so many things that can be done with it. 
However, since my goal is to practice various techniques I have learnt, I looked for some obvious issues that would be solved

1. Figure out a way to find/fill data for the year 1993

2. Which terror group is the deadliest in the world?

3. Predict the unknown terror groups using ML


## The Approach

1. EDA
Gain an understanding of the attacks, their distribution across the world, and their frequency.

Create Visualizations indexed by time, eg: the number of bombings that occurred by year over time.

2. Deadliest Terror group- Taliban or ISIS?

Terror attacks are a ripe area of research for Bayesian inference. Given their infrequency, it is (thankfully) difficult for us to assume a high number of samples that approach some normal distribution.
I'm going to be comparing the deadliness of Taliban attacks and ISIL attacks using Bayesian inference.
The goal is to know if the deadliness of one differs in a significant way than the other

3. Estimate terror attacks for the year 1993
The year 1993 is missing from our dataset. 
Given there is a wealth of information across different types of attacks,
The goal is to create a methodology that allows to impute in the missing values. Then, apply the methodology various attack categories.

4. Predict the Unknown Terror Groups
Construct a model using Machine Learning to predict which groups may have been responsible for an unknown terrorist incident.

## Methodologies used:
1. Pandas and Numpy used for data analysis and data wrangling.
2. Matplotlib and Seaborn for visualisation.
3. Naive Bayes and Logistic Regression to build Machine Learning models.
