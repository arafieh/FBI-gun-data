# FBI Gun data
### Analyzing gun data by each states based on 2016 census data and FBI's NICS data

## Project Overview

The data comes from the FBI's National Instant Criminal Background Check System. The NICS is used by to determine whether a prospective buyer is eligible to buy firearms or explosives. Gun shops call into this system to ensure that each customer does not have a criminal record or isn’t otherwise ineligible to make a purchase. The data has been supplemented with state level data from census.gov.

After wrangling datasets and fixed quality and tidiness issues, analysis process began to find answers for followings questions. All project done in jupyter notebook environment and use pandas, numpy and mathplotlib libraries.

	1. What is cooperation between population growth percentage from 2010 to 2016 and gun during this period? Which states have max and min in population growth and gun during 2010 to 2016 and 2016?
	2. What is relation between population diversity in different states with total gun in 2016: 
		2.1. White population
 		2.2. African American population
 		2.3. Hispanic population
	3. Does veteran population has meaning effect on gun, based on numbers of 2011 to 2015?
	4. Does education has meaning effect on gun, based on numbers of 2011 to 2015?
	5. What is relation between employee and payroll with number of gun in 2015?

	Note: for making easy analysis process, total data in FBI dataset had been used.
	Original datasets named: census_data & gun_data and datasets which used after cleaning are census_final & gun_final

## Project Finding

Here is a summary of finding questions:

	1. Question 1: Comparing population and Gun growth during years 2010 to 2016 
Percentage growth of gun in all states (but one, Utah), are much greater than population growth percentage in same time. So, it seems there are not any logical relation together. The population growth is like a line in front of gun growth from 2010 to 2016 in 50 states and up and down of population growth percent doesn't have any link to gun growth percent. So, let see does maximum and minimum in these two sets, population growth percent and gun growth percent from 2010-2016, has any state in common or not.

	2. Question 2 & 4: Race population and education percentage relation with Gun
White population in states, with biggest average of 'Low' with 0.151263, has less effect on gun per capita and Hispanic population, with biggest average of 'High' with 0.082, has biggest effect on gun per capita among four percentage variables: White, African American, Hispanic and Education.

	3. Question 3: Veteran population relation with Gun
Gun per capita quite related to veteran per capita, except one state, Kentucky, which has out of range gun per capita

	5. Question 5: Employee and Payroll relation with Gun
Interesting, average of gun per capita by payroll levels show in states with 'Moderately High' payroll per capita, there are more gun per capita, but average of payroll by gun per capita levels shows states with 'Medium' gun per capita have more payroll in dollar. So, these two variable coherent together but not strongly.

### Conclusions

Base on the analysis process and limitations, the results can be summarized as following:

	Veteran data has highest correlation with gun total statistic, between all other data that analyzed
	Employee and payroll have moderate effect on gun numbers
	Between race population, Hispanic population has stringer effect on gun numbers rather than white and African Americans population
	I couldn't find meaningful relation between population growth and gun growth.
