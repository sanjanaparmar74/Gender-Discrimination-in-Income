# Gender-Discrimination-in-Income
Programming Language: R


Objective:
Systematic gender discrimination can be a unconspicious yet serious problem for every society. In our analysis, we are hoping to answer the following question:
1. Is there a significant difference in income between men and women?
2.  Does the difference vary depending on other factors (e.g.education, marital status, criminal history, drug use, childhood household factors, profession, etc.)?

Task 1: Loading Data and Renaming Variables
The original dataset nlsy97.csv has 95 variable in total. Among them we pick out 12 (except PUB_ID) for further analysis. Given that the original name of these variables are raw codes, we renamed them into accessible ones using the NLSY97 codebook. 

Task 2: Get Descriptive Statistics
We obtain the basic summary of each variable. At this stage, negative values in some variable indicating some types of missing data are kept.

Task 3: Strategy on Top-coded Variables
For the observations that lie outside of top-2% of the distribution, average value of the top 2 percent of cases are applied to replace the original valid non-missing responses. We believe that the outliers in these two variables lie too far from the normal groups, and we can hence believe that it would cause significant over-estimations if we include them into our analysis.
According to the t-test on the mean difference of INCOME between men and women, though statistically significant in both scenarios, there are considerable differences in terms of the extent. If “top-coded” or top-truncated samples are dropped, the income difference between men and women would be $13028.52, while this figure is $17743.78 with these samples are included.
Hence all the top truncated observations were dropped from the analysis.

Task 4: Statistical Analysis
In this part, detailed analysis on selected variable is carried out. We mainly focus on eight topics that are believe to be huge influencing factors on the income disparity between men and women, such as 1) growing environment, 2) child-raising, 3) criminal history, 4) race, 5) drug use, 6) education, 7) marital status 8) hard times history, 9) family total income and 10) family relationship.

Conclusion:
From the ten section of analysis above, we made the following observations:

Growing environment has a mixed impact for the respondents’ future income. As for the feeling of campus safety, it displays a positive association between the income - the safer environment you are in, the better achievement you might probably get. But the urban/rural background does not have a significant impact on the respondents’ income. Both of these effects do not have a significant difference in terms of gender.

Child-raising has a strong and complecated impact on the respondents’ income. Generally speaking, the more child a person raises, the lower income he/she might get. But seeing from a gender’s standpoint, child-raising brings positive influence to men’s income, but has a significantly negative association to women’s income.

Crime history, measured by incarceration history in our analysis, has a significant effect on income. Specifically, there is statistically significant relationship between incarceration history and income - people with incarceration history earn $16205.59 less than those without incarceration history. But incarceration history has no significant impact on the income gap between men and women.

Race is also a huge factor that has significant impact on the income gap. For example, the income gap between black men and black women is the smallest ($6306.91), but the sex-related income gap for Hispanic is $14732.18 that for Non-Black/Non Hispanic groups is $14118.54.

We expect that people that never used drug will earn more than those that have ever used drug. But the statistical analysis indicates that whether using a drug or not does not significantly related to the income level.

While education level can have strong positive association to people’s income, there does not seem to be statistically significant relationship between education and sex-related income gap. Specifically, in the GED and master-level group, the income gaps between men and women are slightly narrower, while people in the high-school-diploma groups have a wider one. But these difference seems not significant statistically.

The marital status of respondents is an interesting factor to analyse with respect to its impact on income, and its interaction with sex. Generally, there are no significant difference in income among people in different marital status groups. But there was a statistically significant interaction between the effects of gender and marital status on income.

Hard time experience, measured by possible experience of living without water or electricity, or in a homeless shelter, has a negative impact on people income in general. And this effect does not show a significant gender-related difference.

According to our analysis, there is a positive association between gross family income and individual income. And we can also see that the interaction between gross family income of the respondent and his gender has a low but significant influence on the income of the respondent. Specifically, the positive association between family and individual income is observed to be smaller for female.

For people who answered different kinds of relationship to their parent, the income gaps between male and female does vary. For example, individuals with both biological parents which can we called a normal household, are the ones whose gender seems to have a significant interaction with their relationship to parents with respect to their income. But similar effects in other group do not seem to be significant.
