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

The goal of this project is to practice statistical analysis. Using the Amazon Dataset discover if there are particular attributes of the products that may impact their success per product categories.

<a name="dataset"></a>

## Dataset

Dataset [Amazon_co-ecommerce_sample](https://data.world/promptcloud/fashion-products-on-amazon-com/workspace/file?filename=amazon_co-ecommerce_sample.csv).

<a name="workflow"></a>

## Workflow

 - Select a dataset from a public source.
 - Create a Jupyter notebook to analyze the data
 - Cleaning data
 - Understanding and manipulating data
 - Checking correlation between variables
 - Hypothesis testing
      - Normal distribution (T-Test)
      - Not normal distribution (Mann–Whitney U test)
      - Not normal distribution, between categorical and numeric variables (Kruskal-Wallis H Test)
 - Calculating Bayesian Average of rating per category
 - Confidence intervals
 - Linear regression

 
<a name="results"></a>

## Results

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
    - the mean for Hobbies lies within the range of lower 2.726 and upper 3.101 limit
    - the mean for Die-Cast & Toy Vehicles lies within the range of lower 2.634 and upper 2.989 limit
    - the mean for Figures & Playsets lies within the range of lower 2.679 and upper 3.028 limit
- After conducting linear regression model on the number of reviews we can see that this model has a very low R-squared value — 0.032, meaning that this model explains only 3.2% of the variance in our dependent variable. After plotting the results we can see that our prediction is almost always too high. So even if the pvalue is lower than 0.05 we can't trust the results of this model.
- After a few more attempts (one of which was linear regression on sales per category) it is concluded that we would need to have more data to be able to conduct better analysis. 
 
 
 
 ## Next Steps
 
 - It would be interesting to collect more variables about the users and their behavior on site. To predict which users are more likely to buy
 - Also to get the data of transactions to be able to predict the revenue and identify the variables that have the biggest impact on sales
 - Have the monthly data and check how the sales are changing depending on the months (seasonalities)