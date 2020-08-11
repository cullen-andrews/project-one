# Project-One
# U.S. College Diversity’s Relationship with the Workforce
## *TEAM: Kristy Anderson, Cullen Andrews, Daniel Carter, and George Simon*
### SCOPE
Our project is to uncover insights surrounding education, diversity, and income changes in the United States. We will examine relationships between college graduate’s diversity data and income census data over the time periods of 2011-2014 and 2014-2018.
### HYPOTHESIS
Null Hypothesis -- States where the three largest public universities saw an increase proportion of students enrolled of (race) over the time periods of 2011-2014 and 2014-2018 had the same increase in median income for that race in states where the three largest public universities had no increase in enrollment.
Alternative Hypothesis -- Median income increase for (race) was different in states where enrollment for (race) increased at the three largest public universities.

Additional Hypothesis
Null Hypothesis -- changes in median income for (race) as a function of overall average state income are the same for all races.   
Alternative Hypothesis -- different races have different changes in income switching between states with different overall average income.

### DESCRIPTION
We will use data from the U.S. Department of Education, which is in the form of large .csv files. We will research documentation to interpret what the data represents. We will investigate the data set to identify which data pertains to diversity, loan payments, and graduate jobs. We may find that there is no useful data in the jobs category for this particular set, but the data must be cleaned to illustrate that this is the case.

### RESEARCH QUESTIONS
* Over the time periods of 2011-2014 and 2014-2018, is there noteworthy trends in median income and diversity enrollment universities?
* How has the racial population diversity in the U.S. changed from 2011-2014 to 2014-2018?
* Is there statistical significance between student diversity and median income in the U.S.?
* Is there a statistically significant difference in the proportion of students defaulting on their student loans between community colleges and colleges overall?
* What does diversity look like between the different categories of colleges? (e.g. 2-year vs 4-year, private vs public, etc)

### DATASETS
* [College Score Card Data](https://collegescorecard.ed.gov/data/) (columns labeled UGDS & C150)
* [U.S. Census Data API Guide](https://www.census.gov/content/dam/Census/data/developers/api-user-guide/api-guide.pdf) & [U.S. Census API Variables](https://api.census.gov/data/2018/acs/acs5/variables.html)

### DATA ANALYSIS ASSUMPTIONS
* Based on how the data was cleaned and from what was availabe four races were chosen for analysis
    * Hispanic & Latino
    * Black
    * Asian
    * White
* Data was pulled for the below three years in both the Census Data and College Score Card Data
    * 2011
    * 2014
    * 2018 

### PROJECT TASKS
* Data Sourcing/Research - Kristy & Cullen
* Data Cleaning - Cullen & Daniel
* Preliminary Analysis - Team
* Visualizations - Team
* Final Analysis/Write Up - Kristy & George
* Presenter - Team
* Github Merge Manger - Kristy

### FINAL ANALYSIS
#### How has the racial enrollment diversity in the U.S. changed from 2011-2014 to 2014-2018? 
The proportion of college students rose for 2 of the 4 races reviewed and fell for the other 2 races over 7 year span.
![Kristy Visual 1](/images/race_of_admitted_students.png)

#### Is there statistical significance between student diversity and median income in the U.S.? 
According to the data we evaluated, all races average annual household income increased over the 7 year period, whereas diversity of admitted college students varied. With that, there does not seem to be a significant statistical correlation between the two.

![Kristy Visual 2](/images/ave_household_inc_by_race.png)

#### How has the racial population diversity in the U.S. changed from 2011-2014 to 2014-2018?
The percent change of each of the analyzed races can be seen in the below graph. The bar chart highlights the two time spans: 2011-2014 and 2014-2018. The two fastest changing races the data showed were the Asian population (11.8%) and Hispanic & Latino (7.4%) increase from 2014-2018. It was also interesting to note that White is the lowest growing population with a (0.01%) increase from 2014-2018.
![George Visual 1](/images/barchart_pop_change_percent.png)

#### Is there statistical significance between student diversity and median income in the U.S.?
There is no statistically significant evidence that changes in median income of races was different in states where that race’s college enrollment percentage increased vs. states where the race’s enrollment decreased or stayed the same.
The only exception is the white race from 2014-2018, where there is evidence that income increased in states where college enrollment decreased, with a p-value of 0.038 (one-tailed).
![Cullen Visual 1](/visualize/white_14_18.png)

#### Is there a statistically significant difference in the proportion of students defaulting on their student loans between community colleges and colleges overall?
There is significant evidence that a greater proportion of community college students default on their student loans than college students overall.
![Cullen Visual 2](/visualize/two_vs_overall_default.png)

#### Over the time periods 2011, 2014, and 2018, is there a relationship between average household income of a state and the median income of each race looked at?
Yes, there is a relationship. Using a linear regression model we were able to determine the relationship based on what happened to the median income as the average household income increased. The model showed the amount each race can expect their median income to improve for every dollar that the average household income increased. Below are the graphs of the most recent data in 2018.

![Daniels Visual 1](/Linear_Regression_Models/2018_AfricanAmerican.png) ![Daniels Visual 2](/Linear_Regression_Models/2018_Asian.png)
![Daniels Visual 3](/Linear_Regression_Models/2018_HispanicorLatino.png) ![Daniels Visual 4](/Linear_Regression_Models/2018_White.png)

### CONCLUSION
Based on the analysis we conducted we failed to reject our first null hypothesis; *States where the three largest public universities saw an increase proportion of students enrolled of (race) over the time periods of 2011-2014 and 2014-2018 had the same increase in median income for that race in states where the three largest public universities had no increase in enrollment.* However, in analyzing the U.S. Census data we did discover statistical evidence as outlined in the linear regression graphs that median income for (race) as a function of overall average state income are not the same. With this we have successfully rejected or second null hypothesis; *Changes in median income for (race) as a function of overall average state income are the same for all races.*