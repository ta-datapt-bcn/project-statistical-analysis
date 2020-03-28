![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Statistical Analysis

Dinis Oliveira Costa
Data Part-time Dec 2019

### Analysis of 20 years of data on Kobe Bryants's swishes and misses

## Content
- [Project Description](#project)
- [Data](#data)
- [Workflow](#workflow)
- [Results](#results)


## Project Description

- The goal of this project was to practice practice statistical analysis using the iterative data analysis process.
- It is meant to identify the most important features, shot charactheristics and relations between the variables that influence the Kobe's shot accuracy.
- The commands assume a basic understanding of the Pandas, Matplotlib and Seaborn libraries.

## Data

The data used in this project was collected from:

- `Kobe Bryant Shot Selection` - a free dataset from Kaggle originally from a competition meant to practice classification basics, feature engineering, and time series analysis.



## Workflow

The project follows three essential steps: 
- **1) Data Collection and Exploration** 
- **2) Data Analysis and Visualization** and 
- **3) Data Visualization**

### Step 1 - ` Data Cleaning`

- using the given dataset, it is possible to get a clear idea of how each row is characterised given the original column names; 

- since the objective is to interpretate his shots' accuracy, we will begin by checking which columns exist, what values do they admit and what they relate to.

1.1 - Import Libraries and important functions
1.2 - Loading the dataset
1.3 - Adjusting the variables
1.4 - Looking for Nan values



### Step 2: `Data Analysis and Visualization`:

- resorting to a few shot's features, it is possible to draw conclusions by comparing their average and run statistical tests

- identifying potential correlations between variables; 

- identify trends between his accuracy per zone, shot type and season by plotting the distribution of his shots and comparing differences between the average accuracy across these features;

2.1 - Statistical Tests
2.2 - Plotting Location variables
2.3 - Plotting shot accuracy per location
2.4 - Plotting shot accuracy per distance
2.5 - Plotting shots per type, season, period and zone
2.6 - Plotting shot accuracy per type and zone
2.7 - Plotting accuracy across his career 

### Step 3: `Correlations and Data Prediction`:

- The goal of this section is to draw conclusions in regards to which features influence the target variable **shot_made_flag** the most, and to build a model that can predict its missing values
- The two methods chosen are Logisitc Regression and LDA

3.1 - Heatmap of all the variables
3.2 - One Hot Encoding
3.3 Dimensionality Reduction and Logistic Regression
3.4 Linear Discriminant Analysis

## Results

- Clean data set containing all the shots features and Logistic Regression model for shot_made_flag
- Set of figures that help visualize the results and draw conclusions about the dataset


## Deliverables
- `data.csv` - with all the data collected from Kaggle
- `Kobe_Bryant_Project.ipynb` - containing all the code that built the project
- `figures` - containing the product of all the visualization that supported the project
- https://view.genial.ly/5e7e97d35ad5150d93c92bb6/guide-statistical-analysis
