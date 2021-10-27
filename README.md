# Kickstarting with Excel

## Overview of Project
This project focusses on the analysis of outcomes based on goals and outcomes based on launch date using the Kickstarter dataset to assist Louise's play fever in achieving its fundraising project.

### Purpose
The purpose of this analysis is to create a visualization campaign outcomes based on launch dates and funding goals for Louise's play fever to assists with its fundraising project.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
This analysis was performed to determine fundraising outcomes on successful, failed and canceled projects with respect to launch date.
 * During this analysis, a Years columm was added to the Kickstarter_Challenge workbook using the `Year()` function 
 * A  pivot table was created from the  "KickStarter worksheet" to visualize the relationship between outcomes and launch month using "Parent Category" and "Years" columns. 
 * The pivot table was filtered to enable Louise's play fever determine theater outcome performances of theater for various months
 * Chart was saved as `Theater_Outcomes_vs_Launch.png`. ![Theater_Outcomes_vs_Launch.png](https://github.com/charleside2001/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
This analysis was performed to assist Louise's play fever in visualizing the relationship between the percentage of project outcomes based on goals for "plays" criteria from Subcategory column of the KickStarter sheet.
 * During this analysis, a new sheet named "Outcomes Based on Goals" was created with the following columns:
   * Goal
   * Number Successful
   * Number Failed
   * Number Canceled
   * Total Projects
   * Percentage Successful
   * Percentage Failed
   * Percentage Canceled
 * The Project Goal column was populated with the following value ranges
   * Less Than 1000
   * 1000 to 4999
   * 5000 to 9999
   * 10000 to 14999
   * 15000 to 19999
   * 20000 to 24999
   * 25000 to 29999
   * 30000 to 34999
   * 35000 to 39999
   * 40000 to 44999
   * 45000 to 49999
   * Greater than 50000

 3. `COUNTIFS()` and `SUM()` functions were used to populate the Successful, Failed and Canceled projects columns in order to to be able to calculate the Total Projects and Percentages for Successful, Failed and Cancelled projects
 4. A line chart was created with goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis and saved as `Outcomes_vs_Goals.png`. ![Outcomes_vs_Goals.png](https://github.com/charleside2001/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered

 1. The funtion to calcaulated the percentage equation resulted in error on column "H" of  tab "Outcomes Based on Goals".
    * This was resolved using the `IFEROR()` function
 2. Being the first time using github and markdown for Readme.md file editing, it was challenging, however, with the help of youtube vidoes, I was able to figure it out.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
   1. The most successful projects from parent category "theater" occured in the month of May 
   2. Trend show that fundraising goal outcome from parent category "theater" was a success 
 
- What can you conclude about the Outcomes based on Goals?
   1. There were no successful projects between $45000 and $49999 goal target
   2. There were no cancelled projects.The outcome from parent category "play" was either successful or failed. 

- What are some limitations of this dataset?
   1. Excel ran slow and crashed due to so much equation and pivot table images.

- What are some other possible tables and/or graphs that we could create?
   * Outcomes based on Launch Date with respect to Country
   * Outcomes based on Goals with respect to Country
   * Outcomes based on Pledged 
   * Outcomes based on Pledged with respect to Country
   * Outcomes based on Goal and Pledged with respect to Country
   * Outcomes based on Goal with respect to Category and Subcategory
   * Outcomes based on Pledged with respect to Category and Subcategory

 [Kickstarter analysis link on Github](https://github.com/charleside2001/kickstarter-analysis)

