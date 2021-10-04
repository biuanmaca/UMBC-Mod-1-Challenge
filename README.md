# Kickstarting with Excel

## Overview of Project

### Purpose

This project was designed to analyze kickstarter outcomes of theater projects (plays in particular) compared to their launch dates and goals
in order to better plan for future projects and improve success rates.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In analyzing the data for outcomes based on the launch date, I created a pivot table from the raw kickstarter data.  Columns were the outcomes: 
successful, failed, and canceled (live outcomes were excluded).  Rows were the months in which the project was started.  The pivot table was filtered
based on the kickstarter parent category of "theater".  All theater subcategories were included. When visualizing the data in a line graph month-by-month
to see the trends of successful, failed, and canceled, we get the following chart:

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/91292960/135783620-4114e317-adf2-4550-89b7-67b37ea7c036.png)

### Analysis of Outcomes Based on Goals

In analyzing the data for outcomes based on goals, I created an new table pulling data from the raw kickstarter data.  This new table bucketed the goals
in $5,000 increments from $1,000 to $50,000 and a bucket each for less than $1,000 and greater than $50,000.  In those buckets, I counted the number of
projects for each outcome:  successful, failed, and canceled (excluding live projects) that were in the kickstarter subcategory plays.  The totals per
bucket were calculated as well as the percentage for each outcome.  This data was then plotted to a line graph based on buckets in the x-axis, percentages
in the y-axis and lines for each outcome.  The result is shown below:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/91292960/135783564-1cc96712-4b30-4b9b-aa57-0a256feb3419.png)

### Challenges and Difficulties Encountered

The analysis for this was straightforward, but we needed to exclude the projects that were live as the results of those projects were not yet known.  It
should also be noted that prior to 2014, all projects succeeded without any failed or canceled outcomes. While these numbers could skew the results, they
were very few compared to the total projects.  It was determined that the effect would be minimal and so were included in the analysis. 

## Results

In looking at the results of the outcomes by launch date, you can see that the most successful month for projects to be launched in was May and the least
successful was in December.  While some success can be acquired in quarter 1 and early quarter 3, it is most advisable to lauch projects in mid- to late
quarter 2 or early quarter 3.  

In looking at the results of the outcomes based on goals, we can see ranges where there were clear successes.  Less that $1,000 projects achieved near 80%
success rates however that trailed off as you approached the $15,000-$19,999 bucket where the percentages for successes and failures are effectively even.
Between $35,000 and $44,999 projects achieved a 66.67% success rate but quickly bottomed out when going higher.  The analysis suggests that to get the most
bang for your buck, it would be advisable to set your goal between $35,000 and $44,999.

It is tempting to conclude that one should start a project in May with a a goal between $35,000 and $44,999 however the datasets are dissociated from one
another.  To determine if that is truly the best course of action, one would need to compare the two datasets to ensure that the ranges also get positive
results in June (or whatever month one would choose).  It may be that June is good for low goals and August is better for higher goals.  Charts combining
the datasets to determine those results would be needed.  It should also be pointed out that the launch date data filtered for the broader parent category
of theater whereas the goals data filtered for the narrower subcategory of plays. 
