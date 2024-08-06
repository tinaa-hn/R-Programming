STAT 847: Midterm Project

Due Tuesday, Feb 28 at 11:59pm Eastern Time

PICK ONE Kaggle EDA

This is the Feb. 4 version of this assignment. Please check back on Learn over the next week

or so to make sure there are no updated versions with helpful clarifications.

Total Score: 100

Your midterm must be submitted by the due date listed at the top of this document, and it must be submitted
electronically in .pdf format via Crowdmark.


Choose one of the follow datasets to run an exploratory data analysis on, and write a report that answers
everything on the dataset-specfic checklist.

Several of these datasets are new to Kaggle (every one but the covid one). If you decide to get some exposure
on Kaggle, you could publish your midterm project there as a JuPyTer (Julia, Python, R) notebook and be
(one of) the first to do so, thereby being the analysis that gets read the most. At the end of this assignment
is optional notes on how to do so.


For plots, base R or GGplot is fine. Plot does not need to be up to Stat 842 standards, but proper titles
and axes are required. Also las=1 is a good setting. Have a look in the Week 02 version of the 2022 notes
for some basic plotting information if you need some, or ask on Piazza.


Compile the results from all your tasks into a Markdown file. Include your code and 500-1000
words worth of commentary (in total, not in addition to the answers to all the questions. Code
does not count towards word count. Plots are nice, but not worth 1000 words.)



-------



Airfares around Jakarta

https://www.kaggle.com/datasets/datasciencerikiakbar/tiketcom-best-price-for-flights-from-jakarta?
select=tiketcom_bestprice.csv

Q1) (15 points) Merge Datasets
Merge the distance between airports and the
Make sure every variable is of the proper type. (e.g., Numeric, Factor, Character)
Show the summary() or the glimpse() as well as your code (always show your code)


Q2) (15 points) Plot the average airfare by day.
The lubridate package may be useful.
Plot how the average price of a plane ticket changes from day to day. Check to see if the types of flights
change from day to day as well and comment on how flight patterns might confound the issue of airfare. A
simple line graph with day as the x-axis and line type has the sector is a good way to do this graph.


Q3) (10 points) Plot the average airfare by distance between airports.
Binning like we did with 50 Elo blocks for chess might help. Comment briefly.


Q4) (10 points) Plot the average number of flights by hour of day
Comment briefly. Consider a histogram.


Q5) (20 points) Pick a numerical variable to be a response, and build a LASSO model predicting
it


Make sure to use appropriate data (e.g. don’t use 2010 data to predict 2005). Explain why you chose this
variable to model, and why you chose the variables that you chose as candidates for the model. Examine
the variables that leave or enter the model at different values of the complexity/tuning/penalty parameter,
and give an explanation as to why you think your model chooses the variables that it does.


Q6) (30 points) Find at least two other interesting patterns in the data and comment on them.
These could be relationships between data, or interesting distributions, or interesting patterns in time, or
ways to split the data. You are allowed to use plots to make your point. Use this question to fill out the rest
of your word count on the project.
