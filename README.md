# **Analysis of Kickstarter Campaign Data**

  

## **Overview of Project**

### Kickstarter Analysis for Louise's Theater Project.

This project further explores data taken from Kickstarter. It is an attempt to explore possible relationships between theater campaigns 'launch date' and 'goal amount' with their outcomes (success/failure). These trends may lead us to a better understanding of when it is best to launch a campaign and how high our goal should be.  We will visualize these relationships with line charts, analyze the data, and draw conclusions.

[Kickstarter Data](Kickstarter_Challenge.xlsx)


## **Analysis and Challenges**

### Analysis of Outcomes Based on Launch Date
We are looking at the outcomes of success, failure, and cancellations.  From the data provided, we first created a new column "Years" and populated it with the year parsed from the start date. This allowed our data to be filtered by year of the launch date.  We are then able to use a pivot table to compare outcomes of campaigns, to launch dates by month, with the further option to look at each year individually. We have filtered the data by category to look specifically at Theater campaigns. The relationship between outcome and launch date by month is visualized in the line chart below.

![Outcomes_Based_on_Launch](Resources/Theater_Outcomes_vs_Launch.png)

 

### Analysis of Outcomes Based on Goals
In order to examine the relationship between goals and outcome, we have created a table with 12 new ranges for goal amounts. Then, looking at the subcategory "plays", to pinpoint similar Kickstarters, we found the count of success, failure and cancelled outcomes for each of these new goal ranges. We have used these counts to calculate the percentage of success, failure, and cancellations for each of our new goal ranges. The results are visualized in the line chart below.

![Outcomes_Based_on_Goals](Resources/Outcomes_vs_Goals.png)

 

### Challenges and Difficulties Encountered
While working in Excel it is easy to accidently make an error in a cell.  In order to help spot these errors we can cross check totals. For the 'outcome' totals at the bottom of my “Outcomes by Goal Table”, I calculated using *=sum(column)* and crosschecked in the cell below using a *countifs* for all occurrences of the desired 'outcome' with a goal greater than zero. This helped highlight any errors in Outcome columns cell.




## **Conclusions**
### Outcomes based on Launch Date

- At a glance we can see that May is the best time to launch a Kickstarter theater campaign. Campaigns launched in at the beginning of summer have the highest success rate with May being the peak with 111 successes to 52 failures.
- December is the worst time to launch. We can see that theater Kickstarters launched in December are the least successful, 37 successes to 35 failures.  Perhaps, donors have too many other expenses around the holiday period.



 
### Outcomes Based on Goals
- More modest Kickstarter campaigns for plays are the most successful and most common. Percentage success rate is highest for campaigns of less than $1000 and remains high for campaigns under $5000.
- Goals set at $45,000 and above are least successful and success rate remains poor for higher goals. Higher goals are also far less common. It may be that the backers cannot accept a cost this high for crowd funded drama.

  
  


### Dataset Limitations

- Lacking data. The lack of campaigns for plays with high goals limits this dataset. We have only one campaign in the $45-50k and three in $40-45k. Most Kickstarter play campaigns set a goal of less than $10k.
- We can see when filtering by years that although we have Kickstarter data dating back to 2009, most of the theater campaigns are from 2014 through 2016. Adding more years of data will improve data quality.




### Possible Further visualizations 
 - A box and whisker graph could be created to show us the amounts requested for campaigns, allowing us to see the median, IQR, and spot outliers.
- Further breakdown of goal range categories to focus on the lower end range goals.
- We can calculate length of campaign from the start and end dates, then look for effects of campaign length on outcome.
- We can look at the effect of being a "staff pick" on outcomes.


