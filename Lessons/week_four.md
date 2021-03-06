##### Week 4:
Exploratory Data Analysis
- Understanding variable types and assessing missingness
- Visualization as a tool for exploration
- Introduction to `matplotlib.pyplot` and `seaborn`
- Coding tasks:  
  * Find which columns have missing values? How many? What should you do about it? 
  * Find the average death rate from cancer for counties in TN?
  * What does the distribution of the `recent_5year_trend` of deaths from cancer look like for TN counties?
  * What does the distribution of counties **meeting** and **not meeting** the 2020 Healthy People Objective target of 161.4 cancer deaths per 100,000 people look like?
   * Find the 4 counties that have more than 2 hospice facilities? Any surprises?
    * Find the 5 counties with the highest death rate per 100K people.
  * Create 3 new features in `pop_and_cancer`:  `percent_pop_over_50_2010`, `percent_pop_over_50_2014`, `percent_pop_over_50_2017` by dividing each county's over 50 population for 2010, 2014, and 2017 by that year's total population. After you've verified that these columns were created correctly, drop the 24 columns (8 for each year) that you used to create the new buckets: 'pop2010_50to54',
  'pop2014_50to54', 'pop2017_50to54', 'pop2010_55to59', 'pop2014_55to59', 'pop2017_55to59', 'pop2010_60to64', 'pop2014_60to64', 'pop2017_60to64', 'pop2010_65to69', 'pop2014_65to69', 'pop2017_65to69', 'pop2010_70to74', 'pop2014_70to74', 'pop2017_70to74', 'pop2010_75to79', 'pop2014_75to79', 'pop2017_75to79', 'pop2010_80to84', 'pop2014_80to84', 'pop2017_80to84', 'pop2010_85over', 'pop2014_85over', 'pop2017_85over',
     - in 2017, for which two counties was the population over age 50 **greater than half** of the total population?
     - in 2017, for which five counties was the population over age 50 **less than a third** of the total population?

  * create a scatterplot to show the relationship between cancer deaths and the percentage of population over age 50 in TN counties. Use the 2017 population data. Be sure to label axes and add a title.
  * create another new feature, `normalized_hospice_rate` in `pop_and_cancer`. Divide the count of hospices by the 2017 total population and multiply the result by 100,000.
  * create a scatterplot to examine the relationship between population over 50 and the normalized hospice rate in TN counties.
  * Use seaborn to create a boxplot normalized hospice rates, with nested grouping by the Healthy People cancer goal categories.
  