# Kickstarting with Excel

## Overview of Project

Working with Kickstarter data on an Excel spreadsheet has been an worthwhile exercise of several Microsoft Excel techniques. Reading the raw Kickstarter figures at face value presented us with several difficulties of interpreting what the data was saying. With the use of Excel formulas and pivot tables, we were able to clarify our target data’s information for use in our analysis of Kickstarter outcomes. 

### Purpose

As the inspiration for Module 1, Louise is a playwriter who wants to fund her newest play "Fever" via Kickstarter (“1.0.4”, 2021). Over a short period of time, Louise’s Kickstarter manages to secure most of her goal funding, though she is curious about how well other Kickstarters performed relative to their launch dates and funding goals (“Module 1 Challenge”, 2021). Fortunately, we have an Excel spreadsheet chock full of Kickstarter project data (“1.1.3”, 2021), with which we will use our Microsoft Excel techniques to help satisfy Louise’s curiosity.

## Analysis Outline and Initial Challenges

Based on Louise’s aforementioned needs, we will be paying attention to data pertaining to goals, outcomes, and launch dates. Since Louise’s “Fever” is a play (“1.0.4”, 2021), it would behoove us to look specifically at data from theater Kickstarter projects, especially plays. Before jumping into analysis, however, we have several obstacles to address: formatting launch time data, isolating play data from other theater data, and framing our target data without significantly altering the table of raw data. 

### Overcoming Aforementioned Challenges

First, regarding the launch time data format issue, it turns out the launch data numbers are actually Unix-time dates, which we can convert to a day-month-year format (“1.2.2.”, 2021). First, though, to preserve the integrity of the raw data itself, we will simply copy the raw launch date data in Unix to a new column and then converting each entry by dividing them by 86400 seconds (or 60 seconds multiplied by 60 minutes multiplied by 24 hours) and adding the DATE formula ‘DATE(1970,1,1)’ (“1.3.3.”, 2021). Second, for separating plays from theater data, we can use Excel’s ‘Text to Columns’ option with `Delimited` checked, `Tab` checked, `Other` checked, and `/` specified in the `Other` blanks space (“1.3.1.”, 2021). Finally, to frame our desired data without messing with the raw spreadsheet data, we can make a pivot table of that raw data that focuses on data relevant to Louise’s circumstances, which will be made easier now that we have separate theater and play data as well as launch dates in a more readable format.

### Analysis of Outcomes Based on Launch Date

Setting up our pivot table, we will be filtering raw data by Parent Category “theater”, label our row labels by converted date launches, label our columns by outcome, and take the sum value of all outcomes for each date (“Module 1 Challenge”, 2021). Ultimately, we get the below result:
```
!Theater_Outcomes_vs_Launch.png (kickstarter-analysis/resources/Theater_Outcomes_vs_Launch.png)
```


### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

## Works Cited
