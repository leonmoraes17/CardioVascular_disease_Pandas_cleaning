# CardioVascular_disease_Pandas_cleaning
Using Pandas and Stats to gain insights

**View the Presentation.pdf to see insights about the project**

# (Healthcare)
# Increasing our understanding of Cardiovascular disease mortality risks and relationship with Social determinants.

In this project, our team chose two datasets namely USA 2018 census and Cardiovascular disease data.  We merged datasets using Jupyter Notebook, the The dataset was carefully cleaned and prepared  for deeper analysis and visualization.

Our main goal was to investigate the relation between social factors and the mortality rate from cardiovascular disease. Social determinants are elements that are known to affect health outcomes, such as income levels, education, employment, access to healthcare and more. We intended to identify any potential connections or patterns between these variables by combining the cardiovascular disease data, which contains mortality rates, with the census data, which has information on other social determinants.

In order to acquire understanding of the relationship between the mortality rate from cardiovascular disease (Coronary heart disease and Stroke) and social variables (i-e. income, age groups, education level) ,we used data analysis and visualization techniques in Jupyter Notebook. This involved performing statistical tests (Linear Regression & T-test), looking at relationships, and generating visualizations like histogram plots, bar charts and scatter plots. 

With the help of our exploratory analysis, we aimed to answer research questions such as: Does a higher income level correspond to a lower cardiovascular disease mortality rate? How does educational attainment relate to cardiovascular disease mortality within different age groups and states? Does insurance type affect the mortality rate of cardiovascular disease?

Our findings will help in advancing understanding regarding how social determinants affect cardiovascular health outcomes. Policymakers, healthcare workers, and researchers may be able to use the knowledge gathered from this project to design targeted interventions and policies that would lower mortality rates from cardiovascular disease as well as improve population health.


# EDA Analysis:
# Dataset Sources**
Link to Datasets: [https://drive.google.com/drive/folders/1ju45WJ4qb_7oCZBHP5NuQDp2pSb7mJfZ?usp=sharing](https://drive.google.com/drive/folders/1ju45WJ4qb_7oCZBHP5NuQDp2pSb7mJfZ?usp=sharing)


1- United States 2018 Census Tract Data2

2- Rates and Trends in Coronary Heart Disease and Stroke Mortality Data Among US Adults (35+) by County – 1999-20183
**Two Disease Types**

1- Coronary Heart Disease (CDH)

2- Stroke

**Two Age Groups**

1- Ages 35-64 years old

2- Ages 65 years and older

# Merging Datasets**

****Selected relevant columns**

**2018 Data only**

**Averaged income per state**
**Separated education into two levels:** **

-Above High School Degree

-High School Degree and Below

# Findings from Visualization of the distribution of income levels across different states:
From the visualization of the distribution of income levels across different states. We were able to do comparisons between states and reveal a pattern in income distribution across the dataset. The ascending bars showed the range of state average income values, indicating that different states had a varying income level. States with lower bars indicated relatively lower average incomes, while states with higher bars represented relatively higher average incomes. The New Jersey (NJ) and Connecticut (CT) states had the highest bars on the graph that indicated these states had highest average income levels. Whereas Mississippi (MS) state was with the lowest bar and represented that it had lowest average income levels. The differences in bar heights revealed the disparities in income distribution across the states within USA. A significant variation in bar heights suggested a larger income disparity between the highest and lowest average incomes among the states. This indicated the presence of income inequality within the dataset. The lowest average income level state MS had $38,350.88 as income and the highest average income level state NJ had $83,854.97 average income.

# Findings and Interpretation from Visualization of Degree Type:
We had categories the educaction level into two categories namely "HS degree and below" and "Above HS degree". The bar chart of degree type showed almost two equal ditribution. Data set had sample with almost equal percentage of people with High school degree & below comparison to people with who had above high school degree. We inferred that data was normally distributed among the these two degree types as the mean and median of each degree type is almost same.

# Findings and Interpretation from Visualization of the Stacked Barplot for Average Mortality per 100K by both Disease Types and Age groups:
The purpose of the stacked barplot visualization was to  better comprehend the pattern of average state mortality. The mortality count from both type of heart diseases (CHD and Stroke) and across all age groups in each state were graphically shown in the stacked barplot. Death rates in a state can be affected by a number of factors, and we learned more about these influences by analyzing the distribution.

The analysis makes use of a dataset detailing state-level mortality rates per 100,000 residents. The rows of the dataset reflect the 50 states and the columns represent the two type of heart diseases and age categories (35-64 years and 65+ years). Specifically, we used stacked barplots, where each bar represents a state and was further subdivided into segments for each disease category and age group. Upon visualizing the stacked barplot of average state mortalities, several key observations were made:

**Disease Type Contributions:** The vertical segments within each state's bar indicated the contributions of different disease types to overall mortality. The varying lengths of the segments reflected the relative impact of specific diseases in different states. The leading cause of mortality was by Coronoary heart disease (CHD) among 65+ years across all the states and followed by Stroke in the same age group.

**Age Group Patterns:** The color variations observed within each disease type category correspond to distinct age cohorts. Through an examination of the chromatic composition within individual segments, it was possible to gain insight into the variations in mortality rates among distinct age cohorts. The data visualization provided evidence that 65+ years age group people had more mortality by both heart disease type.This data had the potential to illuminate age-related vulnerability and inform focused interventions or healthcare measures. Hence, Centre of Disease control (CDC) should focus their research on how to prevent heart diseases among this group and what could be the possible causes other than age such as lifestyle, eating habits, finanical or emotional stress.

**State Mortality Comparisons:** The comparison of state mortalities can be made by analyzing the heights of the bars, which allowed for the identification of variations in average mortality rates across different states. States with higher overall mortality rates were represented by higher bars such as Arizona (AR), Oklahoma (OK) and Tennessee (TN); whereas lower bars of states such as Massachusetts (MA) and Colorado (CO) indicated relatively lower average mortalities. This comparative analysis offered valuable insights into the regional disparities in mortality rates, thereby indicating the need for targeted interventions and additional research in particular geographic regions.

# Findings and Interpretation from Visualization of Insurance Type:
The data visualization provided understanding on the distribution of insurance types in the US, specifically "Medicare Only," "Private Only," and "Uninsured." The bar chart showed the proportion of each insurance type, revealing coverage gaps and healthcare access issues. The bar chart illustrated the following:

**Medicare Only:** The height of the "Medicare Only" bar represented the percentage of people who used Medicare for health insurance. The bar's height showed population Medicare coverage which was very low as compared to other two types of insurance.

**Private Only:** The "Private Only" bar showed the percentage of people with private health insurance only. Employers, individuals, and organizations offered private insurance. The bar's height showed private insurance's involvement in healthcare was more popular among the people. 

**Uninsured:** The "Uninsured" bar showed the percentage of people without health insurance. These people lacked insurance. Understanding the uninsured population helps reveal healthcare gaps and needs support.

# Findings from the Linear Regression Equations, Visualizations,  & R-values:
In the Regression by Average state Income & Mortality-Coronary Heart Disease of Ages 35-64 years, the coefficient was -0.69217, which showed there was inverse (moderate negative) relationship betweem both the variables (i.e., as the average state income increases by $1, the mortality rate by Coronary heart disease declined by 0.00126 persons for the age group 35-64 years). Furthemore, the graph of regression also revealed the small error variance as the scatter dots were close to regression line. Moreover within the same disease category, similar results were found with a coefficient of -0.31189 with weak negative relationhsip and small error variance; here, as the average state income increased by $1, the mortality rate by CDH declines by 0.00284 persons for the age group 65+).

In the Regression by average state Income & Mortality-Stroke of Ages 35-64 years and 65+ years, the coefficinet was -0.64209 and -0.55624, respectively. The slope was downward slopping which showed there exist inverse relationship betweem both the variables; however, the relationship was moderate for both age groups. Specifically, for age groups 35-64 and 65+ years, as the median income increases by $1, the mortality rate by stroke declined by 0.0003 and 0.00178 persons, respectively. Further, the graphs of regression also revealed the large error variance as the scatter dots were away from to regression line.

# Findings from Comparing High/Low Levels of Income AND Education with OVERALL Mortality
**LOW INCOME-LOW EDUCATION:**
Individuals with lower educational attainment with lower average income states may experience higher mortality rates per 100K population.

**LOW INCOME-HIGH EDUCATION:**
Individuals with higher education levels are associated with lower mortality rates despite in the lower average income state.

**HIGH INCOME-HIGH EDUCATION:**
Individuals with higher educational attainment with higher average income states may experience lower mortality rates per 100K population.

**HIGH INCOME-LOW EDUCATION:**
Individuals having higher education levels with lower average income are associated with higher mortality rates
Hence, it can be concluded that education is important variable along side higher average income to understand the prevention of heart disease types and dietary suppliments.

# **STATISTICAL ANALYSIS: Findings from T-TEST**
# Findings (Relationship between Mortality by CHD and Lower & Higher Average Individuals Aged 35-64 years)
In this case, we are conducting a t-test to compare the mean mortality rate by Coronary Heart Disease between two groups: individuals aged 35-64 years in the lower average income group and individuals aged 35-64 years in the higher average income group. The null hypothesis assumes that there is no significant difference in the mean mortality rate between these two groups, while the alternative hypothesis suggests that there is indeed a significant difference in the mean mortality rate between the groups. Hypothesis are presented below:

**Null Hypothesis (H₀):** There is no significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 35-64 years in the lower and higher average income groups.

**Alternative Hypothesis (H₁):** There is a significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 35-64 years in the lower and higher average income groups.

The results show the p value is significant, therefore we reject the null hypothesis "There is no significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 35-64 years in the lower and higher average income groups". It means that average income does play siginificant role on the mortality rate.

# Findings (Relationship between Mortality by CHD and Lower & Higher Average Individuals Aged 65+ years)
In this case, we are conducting a t-test to compare the mean mortality rate by Coronary Heart Disease between two groups: individuals aged 65+ years in the lower average income group and individuals aged 65+ years in the higher average income group. The null hypothesis assumes that there is no significant difference in the mean mortality rate between these two groups, while the alternative hypothesis suggests that there is indeed a significant difference in the mean mortality rate between the groups.

**Null Hypothesis (H₀):** There is no significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 65+ years in the lower and higher average income groups.

**Alternative Hypothesis (H₁):** There is a significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 65+ years in the lower and higher average income groups.

The results show the p value is significant, therefore we reject the null hypothesis "There is no significant difference in the mean mortality rate by Coronary Heart Disease among individuals aged 65+ years in the lower and higher average income groups". It means that average income does play siginificant role on the mortality rate among individuals aged 65+ years.

# Findings (Relationship between Mortality by Stroke and Lower & Higher Average Individuals Aged 35-64 years)
The null hypothesis assumes that there is no difference in the mortality rate by stroke between the two income groups, while the alternative hypothesis suggests that there is a significant difference.

**Null Hypothesis (H0):** There is no significant difference in the mortality rate by stroke between individuals aged 35-64 years in the lower and higher average income groups.

**Alternative Hypothesis (H1):** There is a significant difference in the mortality rate by stroke between individuals aged 35-64 years in the lower and higher average income groups.

The t-test was used to determine whether the observed difference in mortality rates is statistically significant. And test results reveal the p value is significant, therefore we reject the null hypothesis. There is a significant difference in the mortality rate by stroke between individuals aged 35-64 years in the lower and higher average income groups.

# Findings (Relationship between Mortality by Stroke and Lower & Higher Average Individuals Aged 65+ years)
In this case, the null hypothesis assumes that there is no difference in the mortality rate by stroke between the two income groups, while the alternative hypothesis suggests that there is a significant difference between the two groups. Hypothesis are presented below:

**Null hypothesis (H0):** There is no significant difference in the mortality rate by stroke between individuals aged 65+ years in the lower average income group and individuals aged 65+ years in the higher average income group.

**Alternative hypothesis (H1):** There is a significant difference in the mortality rate by stroke between individuals aged 65+ years in the lower average income group and individuals aged 65+ years in the higher average income group.

By conducting a t-test, we analyzed the data and evaluate whether the evidence supports rejecting the null hypothesis in favor of the alternative hypothesis. As the results shows the p-value is less than or equal to the specified significance level of 0.05, the null hypothesis is rejected. It means that average income does play siginificant role on the mortality rate by stroke among individuals aged 65+ years and there is a significant difference in the mortality rate by stroke between individuals aged 65+ years in the lower average income group and individuals aged 65+ years in the higher average income group. There is a significant difference in the mortality rate by stroke between individuals aged 65+ years in the lower average income group and individuals aged 65+ years in the higher average income group.

# BIBLIOGRAPHY
National Center for Health Statistics. Multiple Cause of Death 2018–2021 on CDC WONDER Database. Accessed February 2, 2023.

Tsao CW, Aday AW, Almarzooq ZI, Beaton AZ, Bittencourt MS, Boehme AK, et al. Heart Disease and Stroke Statistics—2023 Update: A Report From the American Heart Association. Circulation. 2023;147:e93–e621.

National Center for Health Statistics. Percentage of coronary heart disease for adults aged 18 and over, United States, 2019—2021. National Health Interview Survey. Accessed February 17, 2023.
