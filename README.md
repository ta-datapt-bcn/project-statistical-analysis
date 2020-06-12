<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100" align="right"/>


#   Project - Statistical Analysis of E-Commerce Data

KRISTINA KUNCEVICIUTE

*Data Part Time Barcelona Dic 2019*


## Content
- [Project Description](#project)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Results](#results)

<a name="project"></a>

## Project Description

The goal of this project is to find the insights that would be useful for future business decisions.
Using Amazon and Brazilian E-Commerce datasets discover if there are particular attributes of the products that may impact their success.

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

- **Exploratory Data Analysis (EDA):**
  - Data Collection
  - Understanding the Dataset
  - Understanding Variables
  - Data Cleaning
  - Data Transformation
  - Analyzing relationships between variables
  - Data Visualization
- **Inferential Statistics:**
  - Hypothesis testing
  - Confidence intervals
- **Bayesian average of ratings per category**
 
 
 **Libraries Used:**

 - Scipy
 - NumPy
 - Pandas
 - Seaborn
 - Plotly Express
 - Matplotlib

 
<a name="results"></a>

## Results

**Brazilian E-Commerce dataset:**

**Results from the Exploratory Data Analysis:**
 - Have 2 years of transactional data between 2016-10 and 2018-08
 - In both cases, the usage and the total value, credit card payment type is the clear leader
 - The majority of customers buy up to 2 products
 - Revenue differ a lot depending on the state, SP generates most revenue
 - We can see a big increase in sales in November 2017 (due to Black Friday), something that could be expected to repeat in 2018
 - Identified top 3 selling categories that generate the biggest part of revenue
 - Identified top voted categories

**Results from the Correlation analysis:**
 - Identified the most correlated variables with the payment value

**Results of the hypothesis testing:**
 - We failed to reject H0, not enough data to state that the averages are statistically different
 
**Results from the confidence interval analysis:**
 - We are 95% sure that the population mean of payment value lies within the range of lower 108.864 and upper 122.856 limit.

**Bayesian average:**
 - Identified that the average of rating score per category is biased. Conducted bayesian average to align it.


<br><br>
**Amazon Dataset:**

**Results fom exploratory data analysis:**
 - the number of sales and average price differ a lot depending on the category
 - identified top-selling categories
 - identified that the average ratings don't differ a lot (all between 4 and 5)
 - After checking the correlation we identified that there is no strong correlation with any variables and we would need more data to be able to conduct a more informative statistical analysis
  - Some correlation was discovered between the number of reviews and the number of answered questions, average review rating, description len.

**Conducting various hypothesis testing on price, number of reviews and average rating. Main findings:**
 - Out of 3 most selling, only Hobbies and Figures & Playsets have statistical significance in average price.
 - There is a significant difference between the number of reviews in Hobbies and Die-Cast & Toy Vehicles categories.
 - From the visual inspection, we saw that the average ratings were similar, but thanks to the test we realized that there is actually a significant difference between the 3 top categories.
 
**After inspecting price confidence intervals for the top 3 selling categories we are 95% sure that:** 
    - the population mean lies within the range of lower 2.218 and upper 2.592 limit
    - the mean for Hobbies lies within the range of lower 2.498 and upper 2.832 limit
    - the mean for Die-Cast & Toy Vehicles lies within the range of lower 2.473 and upper 2.751 limit
    - the mean for Figures & Playsets lies within the range of lower 2.591 and upper 2.892 limit

**Identified that the number of ratings is biased. Conducted bayesian rating average to align it.**

 
 
 
 ## Next Steps
 
 - Collect more data about the users and their behavior on site. Use ML models to predict which users are more likely to buy
 - Get the data of transactions to be able to predict the revenue and identify the variables that have the biggest impact on sales
 - Have the monthly data and check how the sales are changing depending on the months (seasonalities), forecast the future sales