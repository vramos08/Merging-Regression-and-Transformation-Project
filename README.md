# Project 1 Overview
This project is composed of two parts. In part A, we focus on merging the two datasets given to us and addressing the missing data. We then are tasked to create a linear regression model to get a relationship between the independent and dependent variables. Part B's primary task is to analyze a dataset with repeated or nearly repeated data points, requiring data transformation and the application of the lack of fit test.
# Methods for Part A
To merge the data sets, I created objects for each file and used the merge function. The 'mice' package assisted in dealing with missing values, 'knitr' was used to create an ANOVA Table, and data visualization was performed to visualize the regression line.
# Results for Part A
The data set consisted of 685 data values with 577 subject IDs containing both independent and dependent values. The OLS estimate for the intercept was 31.3953 and 7.9710 for the independent variable (IV). The R-squared was 0.7359, and the ANOVA table is provided. The regression line model was DV = 31.3952 + 7.9710IV.
# Methods for Part B
I began by plotting the data to determine the required transformation. Data transformation (y^1/2) was applied to address the decreasing rate of y. Binning was performed using the 'cut' and 'ave' functions. The 'olsrr' package enabled the application of the LOF test.
# Results for Part B
The original data had an R-squared of 0.416, indicating a 41.6% variation in the dependent variable explained. The LOF test yielded a p-value of 0.2211199. After transformation, the new data model had an R-squared of 0.432, with the LOF test p-value indicating a good fit.

