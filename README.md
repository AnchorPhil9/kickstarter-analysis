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

![Theater Outcomes vs Launch](/resources/Theater_Outcomes_vs_Launch.png)

The most eyegrabbing part of the results is how successful the summer / late spring months are for theaters. Certainly, the data seems to correlate with the influx of students finishing their spring semesters and gearing up for summer break activities. With success, though, comes failure, which is also pronunced in the summer/late spring monthsElsewhere, there are notably fewer canceled projects, though January does have the most canceled projects, maybe because January tends to be when students and working adults come back from winter break to return to school or work respectively, during which they are less interested in going out to see theater productions.

### Analysis of Outcomes Based on Goals

### Other Challenges and Difficulties Encountered

## Results

## Works Cited
1.0.4 Kickstarting with Excel. (2021). Bootcamp Spot. Retrieved April 24, 2021, from 
    https://courses.bootcampspot.com/courses/577/pages/1-dot-0-4-kickstarting-with-excel

1.1.3 Download the Kickstarter Data. (2021). Bootcamp Spot. Retrieved April 25, 2021, from 
    https://courses.bootcampspot.com/courses/577/pages/1-dot-1-3-download-the-kickstarter-data

1.2.2 Initial Look at the Data. (2021). Bootcamp Spot. Retrieved April 25, 2021, from 
    https://courses.bootcampspot.com/courses/577/pages/1-dot-2-2-initial-look-at-the-data

1.3.1 Pivoting Towards Success. (2021). Bootcamp Spot. Retrieved April 25, 2021, from 
    https://courses.bootcampspot.com/courses/577/pages/1-dot-3-1-pivoting-toward-success

1.3.3 Timing Success. (2021). Bootcamp Spot. Retrieved April 25, 2021, from 
    https://courses.bootcampspot.com/courses/577/pages/1-dot-3-3-timing-success

Module 1 Challenge. (2021). Bootcamp Spot. Retrieved April 25, 2021, from 
    https://courses.bootcampspot.com/courses/577/assignments/11823
