![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Statistical Analysis

## Overview

The goal of this project is to practice statistical analysis using the iterative data analysis process and combine it with interactive data visualization libraries such as plotly or ipywidgets. For this project, we have used the FilmAffinity dataset that we had scrapped in previous projects. The main information is in the `pelis_fa_pr06.csv` dataset, but there is another file already filtered through SQL also from a previous project with the top 10 actors by average movie rating per decade in the `SQL-top10actores_puntuacion.csv` file.

---

## Statistical analyisis

The 3 statistical analysis are contained in the `Proyecto_slides.ipynb` workbook:

* **ANOVA**: in this visualization it is possible to see the pvalue of applying the ANOVA method to the distributions of the ratings of all movies for 3 different actors. The program will inform us if there are significant differences in their rating distributions.

* **Confidence intervals**: _if we decide to hire a specific actor, we can ensure with a given confidence interval that the rating of the movie will be between A and B_. The goal of this visualization is to answer this questions, i.e. calculate both A and B values given any actor and confidence interval.

* **Two-sample independent test**: _is it worth hiring that actor?_ This is the question we are trying to answer by applying a two-sample independent test in which we compare the rating distributions of a given actor's rating with the rest of the ratings in the dataset for those movies that might be comparable. To do that, the program will filter all the rest of the movies in the dataset that share the same activity years of that actor and the main genre.

## Prediction: linear regression

The prediction with linear regression is also contained in the `Proyecto_slides.ipynb` workbook. The goal of this program is to predict a movie's rating depending on its main director, its main genre and its origin, having reduced the last one to US, Europe or rest of the world.

Since most of our variables are categorical, we needed to apply the `pd.get_dummies()` function that converts categorical variables into numerical by adding all values into new columns that contain 0 or 1.

To avoid ending up with a dataframe with thousands of columns, we reduced our dataset by keeping only those movies directed by the top 10 most prolific directors.

The categorical values of our predictor have been reduced to the following fields:

* Director: the top 10 most prolific directors

* Genre: drama, comedy, horror, action, sci-fi or thriller

* Country: United States, Europe or rest.

## Prediction: time series

Our interactive predictor with time series is contained in the workbook `TimeSeries.ipynb`. The objective of this visualization is to have an overview of the number of movies in the last 100 years by genre and predict the number of movies in the upcoming years by genre.

Since the number of movies decreased a lot in the last years due to Covid-19, this program will allow the user the option to see how the prediction would have been if this effect would not have existed, i.e. filtering the movies from 1920 to 2018, instead of 
considering the entire dataset until 2020.