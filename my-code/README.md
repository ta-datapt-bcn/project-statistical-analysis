# Statistical Analysis Project
# by Jordi Marsal

*Ironhack's Data Part-Time | Barcelona | September 2019*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-/-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)



## Project Description
* In this project we take a look about a set of data from votations in a web site called __"Metacritic"__ where their users vote and review games.



## Hypotheses / Questions
* It is possible found relations between votes and genres?
* There are relations over users types and their votations? 
* This project is presented to a bunch of data-coleagues in game industry.



## Dataset
* This dataset has been obtained from Kagle.com
* Metacritic games stats 2011-2019
* https://www.kaggle.com/skateddu/metacritic-games-stats-20112019
```
    metacritic_games.csv (554.8 KB)
    4018 rows x 15 columns
```

| Column name | Description | Type |
| :--- | :--- | :--- |
| game | game name | descriptive |
| platformgame | platform | categorical |
| developer | game developers | descriptive |
| genre | game genre | categorical |
| number_players | number of players | categorical |
| rating | game rating | numeric |
| release_date | release date | numeric |
| positive_critics | number of positive reviews by critic| numeric |
| neutral_critics | number of neutral reviews by critic | numeric |
| negative_critics | number of negative reviews by critic | numeric |
| positive_users | number of positive reviews by users | numeric |
| neutral_users | number of neutral reviews by users | numeric |
| negative_users | number of negative reviews by users | numeric |
| metascore | mean critic score | numeric |
| user_score | mean users score | numeric |




## Cleaning
* Detect nulls.
* Denull some columns: developer and genre.
* Substitution of NaN by UNKNOWN.
* Grouping values of columns for number_players.



## Analysis
* General Info.
* Correlation for numerical fields.
* Boxplots and Histograms for fields.
* Scatterplot (pairplot) between numerical variables to find interesting relations. 
* Calculations for Highlighted Variables:

      Linear Regression.

      r-squared (covering variance).

      p-value (hypothesis test).

      Correlation.

      Plot with Regression Line.

* Confidence Intervals for Highlighted Variables.
* Hypothesis Test for Highlighted Variables.
* Logistic Regression:

      Score.

      Confussion matrix.

      Plot for both.



## Model Training and Evaluation
* Logistic Regression:

      Score.

      Confussion matrix.
    
      Plot for both.

      The dataset has been splitted to train / test sets. Almost all categorios has been predicted with this model. 


## Conclusion
* Results of Linear Regression are similar to correlations found. They are weak and poor.
* No one variable hits same mean value. All H0 has been rebuked.



## Future Work
* This data set can be fullfilled with other complementary data. It can bring more clarity than this one alone.



## Workflow
* Discovering data:

      ploting pairplots, boxplots and histograms.

      info.

      correlation matrix.


* Testing succes with metrics from sklearn



## Organization
* Git
* Visual Code
* Jupyter Notebooks
* Trello



## Links

* [Repository](https://github.com/jordimarsal/project-statistical-analysis)  
* [Trello](https://trello.com/b/n0R83yqA/dapt-bcn-module-2-planning-students)  
