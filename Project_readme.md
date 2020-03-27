![N|Solid](https://i1.wp.com/www.alliron.vc/wp-content/uploads/2018/05/logo-ironhack-1.png?w=400)

### Project Data Analytics:
### Statistical Analysis
Miguel Ángel Ávalos
Data Part Time Barcelona Dic 19


### Project Description

The main objective of this project was to conduct an statistical analysis of a world-real dataset. The chosen [dataset](https://www.kaggle.com/nathanlauga/nba-games "NBA match results from 2003 to 2020" was one from the kaggle pltaform which contains the matches results from NBA Basketball League from 2003 to 2020.

### Dateset

The variables in the dataset are:
```
 - GAME_DATE_EST: Date when the match has been played. Rank from 2003-10-05 to 2020-03-01.
 - GAME_ID: Unique identifier of the match
 - GAME_STATUS_TEXT : Contains 'Final'
 - HOME_TEAM_ID: Unique identifier for Home/Local Team
 - VISITOR_TEAM_ID: Unique identifier for the Visitor Team
 - SEASON: Season when the game occured
 - TEAM_ID_home: Unique Identifier of the Home Team (dupplicate of HOME_TEAM_ID)
 - PTS_home: Total points scored by home team
 - FG_PCT_home: Field Goal Percentage Home Team
 - FT_PCT_home: Free Throw Percentage Home Team
 - FG3_PCT_home: Three Point Percentage Home Team
 - AST_home: Assists of the Home Team
 - REB_home: Rebounds of the Home Team
 - TEAM_ID_away: Unique Identifier of the Visitor Team (dupplicate of VISITOR_TEAM_ID)
 - PTS_away: Total points scored by Visitor team
 - FG_PCT_away: Field Goal Percentage Visitor Team
 - FT_PCT_away: Free Throw Percentage Visitor Team
 - FG3_PCT_away: Three Point Percentage Visitor Team
 - AST_away: Assists of the Visitor Team
 - REB_away: Rebounds of the Visitor Team
 - HOME_TEAM_WINS: Boolean indicating if Home Team wins (1) or not (0)
```

### Work Description
The work done in thise project can be summarized in the following points:
1. **Exploratory Data Analysis**: Explore the main variables, and select the one that did not contain duplicated info. Moreover, null values were treated during this process.
2. **Data Analysis**: In this step, it was made a correlation analysis to find relationship between variables. Also, testing some hypothesis about the normality of the distribution as well and two-way ANOVA were performed to explore the significance between Win Rate % and Season / Team as well as Bonferroni Test to assess differences between groups. Finally, the numerical variables were standarized as a data transformation for the following step.
2. **Prediction Models**: A Logistic Regression Model to predict the result of the match (HOME_TEAM_WINS) and, later a Random Forest Regression were used to trying to predict the result of the Home Team and the Visitor Team.

### Results
The results obtained were the different results of the statistical tests as well as the results of the different predictor models.
 

