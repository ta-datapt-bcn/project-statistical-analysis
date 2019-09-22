<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Title of My Project
*[Hernando Cardenas]*

*[Your Cohort, Campus & Date]*

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

<a name="project-description"></a>

## Project Description
En este proyecto vamos a analizar los datos de la premiere league desde el año 1993 al año 2018 para tratar de predecir que equipo va a ganar mas partidos, cual recibe mas goles y cual anota mas goles durante la temporada. 

<a name="hypotheses-/-questions"></a>

## Hypotheses / Questions
* Es realmente el 2-0 o 0-2 el resultado mas remontable? 
* Ser el equipo con mas goles te hace mas propenso a ganar la competicion? 
* Ser el equipo con menos goles en contra te hace mas propenso a ganar la competicion?  
*

<a name="dataset"></a>

## Dataset
*Este data set fue descargado de kaggle https://www.kaggle.com/thefc17/epl-results-19932018.
   * los datos a manejar son los siguientes y cada uno significa lo siguiente
    Div = Division donde se juega
    Date = Fecha de los partidos
    HomeTeam = Equipo local
    AwayTeam = Equipo visitante
    FTHG = Goles equipo local al final del partido
    FTAG = Goles equipo visitante al final del partido
    FTR = Resultado final del partido
    HTHG = Goles equipo local medio tiempo
    HTAG = Goles equipo visitante medio tiempo
    HTR = Resultado medio tiempo
    Season = Temporada.
* If the question cannot be answered with the available data, why not? What data would you need to answer it better?

<a name="cleaning"></a>

## Cleaning
Los datos del año 1993 a 1995 en las columnas HTHG HTAG HTR estan con valores NaN por tanto seran borradas ya que no va a servir para el tipo de estudio que se desea realizar.

<a name="analysis"></a>

## Analysis
* Revisar si realmente el mito de el resultado 2-0 o 0-2 es el mas traicionero para los equipos.
* Tratar de dar un estimado de cual equipo tiene mas chance de ganar la liga.
* Saber como en que condicion le son mas favorables los partidos a el top 5 de los equipos. 
* Saber con que probabilidad el resultado 2-0 o 0-2 es empatado o remontado.
*

<a name="model-training-and-evaluation"></a>

## Model Training and Evaluation
*Include this section only if you chose to include ML in your project.*
* Describe how you trained your model, the results you obtained, and how you evaluated those results.

<a name="conclusion"></a>

## Conclusion
* Summarize your results. What do they mean?
* What can you say about your hypotheses?
* Interpret your findings in terms of the human-understandable question you try to answer.

<a name="future-work"></a>

## Future Work
Address any questions you were unable to answer, or any next steps or future extensions to your project.

<a name="workflow"></a>

## Workflow
Outline the workflow you used in your project. What were the steps?
How will you test the success of our analysis or algorithm?

<a name="organization"></a>

## Organization
How did you organize yourself? Did you use any tools?

<a name="links"></a>

## Links
Include the links to your repository, slides and trello. Feel free to include any other links associated to your project. 

[Repository](https://github.com/)  
[Slides](https://slides.com/)  
[Trello](https://trello.com/en)  