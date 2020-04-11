<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100" align="right"/>


#   Project Ironhack Data Bootcamp

KRISTINA KUNCEVICIUTE

*Data Part Time Barcelona Dic 2019*


## Content
- [Project Description](#project)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Results](#results)

<a name="project"></a>

## Project Description

The goal of this project is to practice statistical analysis. 
Using the Amazon and Brazilian E-Commerce datasets discover if there are particular attributes of the products that may impact their success.

Note: 
- The first dataset analyzed was Amazon dataset, after investigating, it appeared that there is almost no correlation between the variables.
- Second analysis is done with the Brazilian E-Commerce data.

<a name="dataset"></a>

## Datasets

Datasets:
- [Amazon_co-ecommerce_sample](https://data.world/promptcloud/fashion-products-on-amazon-com/workspace/file?filename=amazon_co-ecommerce_sample.csv).
- [Brazilian E-Commerce data](https://www.kaggle.com/olistbr/brazilian-ecommerce).

<a name="workflow"></a>

## Workflow

 - Select a dataset from a public source.
 - Create a Jupyter notebook to analyze the data
 - Data cleaning
 - Exploratory analysis
 - Correlation
 - Hypothesis testing
 - Calculating Bayesian Average
 - Confidence intervals
 - Linear regression

 
<a name="results"></a>

## Results

Brazilian E-Commerce dataset:

Results from the Exploratory Data Analysis:
 - Have 2 years of transactional data between 2016-10 and 2018-08
 - In both cases, the usage and the total value, credit card payment type is the clear leader
 - The majority of customers buy up to 2 products
 - Revenue differ a lot depending on the state, SP generates most revenue
 - We can see a big increase in sales in November 2017 (due to Black Friday), something that could be expected to repeat in 2018
 - Identified top 3 selling categories that generate the biggest part of revenue
 - Identified top voted categories

Results from the Correlation analysis:
 - Identified the most correlated variables with the payment value

Results of the hypothesis testing:
 - The average payment value in two selected groups (2 categories that have the highest average payment value) is significantly different
 - We saw that the average ratings were similar, but thanks to the test we realized that there is actually a significant difference between the 3 top scored categories
 
Results from the confidence intervals analysis:
 - We are 95% sure that the population mean of payment value lies within the range of lower 4.596 and upper 4.798 limit.

Results form the Linear Regression model:
 - R-squared value of 0.356, meaning that this model explains 35,6% of the variance in our dependent variable.
 - The pvalue is lower than 0.05, meaning we can reject the Null hypothesis and accept the alternate hypothesis. There is a statistically significant impact on the payment value from our selected independent variables.
- The biggest impact on the payment value is coming from:
  - payment_sequential(several payment methods), increasing by one it decreases the payment value by -0.3417
  - order_item_id (number of items included in the same order), increasing by one it increases the payment value by 0.3049
  - payment_installments, increasing by one it increases the payment value by 0.1054
 
 

Amazon Dataset:

 - From the exploratory data analysis we already identified that 
     - the number of sales and average price differ a lot depending on the category
     - identified top-selling categories
     - identified that the average ratings don't differ a lot, all are between 4 and 5
 - After checking the correlation we identified that there is no strong correlation with any variables and we would need more data to be able to conduct a more informative statistical analysis
  - Some correlation was discovered between the number of reviews and the number of answered questions, average review rating, description len. The focus of the analysis is not shifting from sales to the number of reviews.
 - Conducting various hypothesis testing on price, number of reviews and average rating. Main findings:
     - Out of 3 most selling categories, only Hobbies, has a significantly different average price.
     - There is a significant difference between the number of reviews in Hobbies and Die-Cast & Toy Vehicles categories.
     - From the visual inspection, we saw that the average ratings were similar, but thanks to the test we realized that there is actually a significant difference between the 3 top categories.
- Identified that the number of ratings is biased. Conducted bayesian rating average which is a lot more aligned.
- Inspecting price confidence intervals for the top 3 selling categories we are 95% sure that: 
    - the population mean lies within the range of lower 2.07 and upper 2.524 limit
    - the mean for Hobbies lies within the range of lower 2.644 and upper 3.07 limit
    - the mean for Die-Cast & Toy Vehicles lies within the range of lower 2.668 and upper 3.055 limit
    - the mean for Figures & Playsets lies within the range of lower 2.625 and upper 3.0 limit
- After conducting linear regression model on the number of reviews we can see that this model has a very low R-squared value — 0.032, meaning that this model explains only 3.2% of the variance in our dependent variable. After plotting the results we can see that our prediction is almost always too high. So even if the pvalue is lower than 0.05 we can't trust the results of this model.
- After a few more attempts (one of which was linear regression on sales per category) it is concluded that we would need to have more data to be able to conduct better analysis. 
 
 
 
 ## Next Steps
 
 - It would be interesting to collect more variables about the users and their behavior on site. To predict which users are more likely to buy
 - Also to get the data of transactions to be able to predict the revenue and identify the variables that have the biggest impact on sales
 - Have the monthly data and check how the sales are changing depending on the months (seasonalities)