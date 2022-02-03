# Videogame Sales Analysis

Over the last couple of years videogames have grown to become the largest industry in the entertainment sector, with it's projected worth being 145 billion dollars globally. A single game such as Minecraft can sell over 238 million copies while there are some that completely flop on release, costing companies millions in development. Therefore, it would extremely beneficial to be able to uncover some sort of relationship between characteristics of a videogame and the sales that sales numbers generated by those titles.


## Project Overview
The objective of the Videogame Sales Analysis is to create insights as to what variables affect a videogames sales in order to help publishing companies when deciding what potential projects to prioritize for maximum returns and additionally help projects decide what publisher to go to if multiple offers are on the table. To accomplish this I used a chi-square test to look for substantial differences in the ratings given to certain genres, an ANOVA to investigate the effect the genre and publisher have on a videogames global sales, and linear regression to measure the impact of the predictors individually and when viewed together.



## Resources
Data Source: https://www.kaggle.com/rush4ratio/video-game-sales-with-ratings

Software: RStudio

## Defining Successful Videogames
Videogame success is measured in two ways: Critical reception and financial success. Financial success is self explanatory, videogames are sold and the more units sold the more revenue produced. Critical reception is harder to gauge but for that we have Metacritic. Metacritic aggregates the scores of critics and users and assigns games two scores, the "Meta Score" and "User Score". Our exploratory analysis on these variables gave us the tables below:

<p align="center">
  <img src="https://github.com/esalcedo1/videogame-analysis/blob/draft/1-defining-successful-videogames/genre-usercritic-score.png?raw=true" alt="Genre vs. User and Meta Score" height="250"/>
  <img src="https://github.com/esalcedo1/videogame-analysis/blob/draft/1-defining-successful-videogames/genre-region-sales.png?raw=true" alt="Sales by Genre and Region" height="250"/>
</p>

From the first table we can see that on average RPGs, Sports, and Strategy games all get higher than average Meta scores while on the user-side RPGs score particularly high. The second table shows us that genres have different levels of popularity and reception in different regions of the world. In North America Shooter and Platforming games sell best while in Japan Puzzle and RPGs sell best. 


## Chi-Square Analysis

The objective of this analysis was to prove that there exists a substantive difference between the genres on the ratings the games were given. Before conducting the analysis itself we first visualize the distributions of ratings within each genre using a stacked bar chart.
(For an explanation of the variables used, please refer to the README file located in the chi-square folder.)

<p align="center">
  <img src="https://github.com/esalcedo1/videogame-analysis/blob/draft/2-chi-square-analysis/Picture1.png?raw=true" alt="stacked bar chart" width="400">
</p>

After this intial investigation, a chi-square test was run resulting in the following data table:

<p align="center">
  <img src="https://github.com/esalcedo1/videogame-analysis/blob/draft/2-chi-square-analysis/Figure2.png" alt="chi-square table">
</p>

At an alpha of 0.05, we are able to reject the null hypothesis and conclude that there is both a statstical and substantive significant association between genre and the ESRB rating assigned to it.

## ANOVA Analysis
An ANOVA analysis assumes 5 things:

1. Each group sample is drawn from a normally distributed population
2. All populations have a common variance
3. All sampels are drawn independently of each other
4. within each sample, the observations are sampled randomly and independently of each other.
5.  Factors effects are additive

## Linear Regression
The point of linear regression is to measure the impact of predictors indvidually and if their impact is increased when combined


