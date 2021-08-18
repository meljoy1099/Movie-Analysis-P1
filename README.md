# IMDB Movies Analysis

**Authors**: Melody Bass

## Overview

The focus of this project is to analyze determining factors in what makes a movie successful. We will define success as a film being profitable and well received by critics and users. The original data source comes from Kaggle and can be found [here](https://www.kaggle.com/soumyasacharya/imdb-movies-dataset).  The dataset contains information on over 75,000 movies from IMDB. We will first focus on investigating the dataset and cleaning and wrangling the data into analysis format. The next sections contain questions and answers pertaining to the properties and characteristics that have made films successful over the past 20 years and the modeled data as follows:
* Movie length 
* Movie release month
* Production budget
* Genres
* Directors
* Actors 

Finally, I will evalate my results and make recommendations to Microsoft's new movie studio about what types of movies will be successful in today's atmosphere.  

## Business Problem

Microsoft wants to get into the movie business, and I have been tasked with making recommedations about what types of films to create.

***
Questions we will answer:

1- What characteristics are associated with the most successful movies?
  * What movie length generates the most profits?
  * What movie length is the highest rated by users and critics?
  * What months are the most profitable movies released?
  * Do higher production budgets lead to higher profits?
  * Do higher production budgets lead to higher user and critic reviews?
  * Do higher production budgets lead to higher ROI?

2- What genres are most profitable and highly rated overall and over time?
  * What is the most profitable genre?
  * What genre is the highest rated by users and critics?
  * What is our top overall genres?

3- Who are the people who make the most successful films?
  * What director generates the highest average profit?
  * What directors have the highest user and critic ratings?
  * What directors have the highest average ROI?
  * What popular actors make the most profitable movies?
  * What popular actors have the highest user and critic reviews?
  * What popular actors have the highest average ROI?
***

## Data

The dataset used for this analysis was found on [Kaggle](https://www.kaggle.com/soumyasacharya/imdb-movies-dataset). It is a compiled dataset containing information about 75,000 movies from IMDB. I will only use movies from the dataset that contain gross income, production budget, user and critic ratings, and were released in the United States from the year 2000 - present. I calculated profit ($M) and ROI (%) to use as some of my parameters to measure movie success.  The variables that will be used to evaluate a movie's success will be profit ($M), audience reviews, critic reviews, and in some cases, ROI (%).  I will compare the mean of these variables to movie length, release month, production budgets, genres, directors, and actors.

## Methods

The model used for processing and analyzing the dataset was descriptive analysis. Movie data was used from the last 21 years to give us a good representation of what is doing well now and over time.  Movies were only included in the dataset if they were released in the United States to avoid currency conversion errors.  Financial data used to calculated statistics has not been adjusted for inflation.

To determine a movie's success, I not only wanted to use gross income and profit, but also take into account user and critic reviews as a secondary measure.  The movie length most likely to succeed was determined by finding a range of movie length times containing the maximum average profit, user and critic ratings runtime.  The best months to release movies was calculated by comparing average profit generated vs month of release.  Correlation coefficients were calculated on production budget's effect on profit, ROI, user and critic ratings.

The top overall genres to create today were determined by compiling movies by genre and comparing to the average profits generated, user ratings, and critic ratings.  I took a closer look at the top 5 genres of these categories and compared each genre to the compiled genre profit mean and noted the overall effect outliers have on the dataset.

To measure a director's success in making movies, the dataset was grouped by director and compared against the mean of profit, user ratings, critic ratings, and ROI.  I only wanted to include directors who are consistently successful, so directors had to meet of criteria of directing more than 5 films.  The actors were analyzed and evaluated in the same fashion as directors, except they had to meet a criteria of appearing in more than 10 films.  

## Results

Based on the exploration and analysis of the IMDB movies dataset:

1) The following are characteristics and properties of movies that lead to higher profits, audience, and critic reviews:
  * Movie length between 152 - 165 minutes([Illustrated here](./images/length_profit.png))..
  * A high production budget ([Illustrated here](./images/budget_profit.png)). 
  * Movie released in December ([Illustrated here](./images/profit_month.png)).

2) The best overall movie genres to create today are Animation and Adventure. Both Animation and Adventure have higher production budgets, but also [higher profits and gross income](./images/genre_profit_budget_income.png) than other genres.  Animation is the [most profitable genre](./images/genre_profit.png), but typically not in the top of user and critic reviews.  Animation has a tighter range of profit generated, and most is higher than the mean of overall genre profit.  There are also few outliers in the Animation category. Adventure is the second most profitable genre but there are far more [outliers in the data](./images/genre_profit_box.png), meaning there are several Adventure films that generated massive profits that drive the mean up.  Adventure movies are generally rated higher by the [audience](./images/genre_user_ratings.png) and [critics](./images/genre_critic_ratings.png).

3) The following are people that have been the most successful at acting and directing films in the past 20 years:
  * Directors - The top directors by [profit](./images/director_profit.png) and [ratings](./images/director_critic_ratings.png) are Gore Verbinski and Sam Raimi. Paul Thomas Anderson and Clint        Eastwood score high with the critics. Anne Fletcher, Robert Luketic, and Tim Story are less known directors who have         shown to have tremendous potential based on their [ROI](./images/director_roi.png).
  * Actors - [Paul Bettany](./images/actor_profit.png) is the top overall actor of every success category, followed by Robert Downy Jr and Chris Hemsworth.     Josh Gad and Alan Tudyk are highly profitable due to their appearance in several Disney movies, but those profits did not     translate to user and critic ratings.  Natalie Portman and Gwyneth Paltrow are the actors with highest [critic reviews](./images/actor_critic_ratings.png) not     appearing in the Avengers and Frozen movies, while still scoring high with the critics. Diedrich Bader and Danny Glover       have the highest [ROI](./images/actor_roi.png).

## Conclusions

We have determined some of the properties and characteristics that make a movie successful recently. I will propose some recommendations and guidelines to start a movie studio based on the work of this project as follows: 

1) The studio should create high budget films that are 152 - 165 minutes long and release these films in December.

2) The studio should focus on creating Animation and Adventure films. Animation is a good choice if a less risky investment is preferred, as higher profits are seen with less outliers in the data (Movies that generated huge profits). If developing a global presence while maintaining high profits is preferred, I recommend creating Adventure films. There is more risk involved in making Adventure films, but there is also the potential to make huge profits and produce critically acclaimed films.

3) The studio should look at the results of the director and actor analysis and hire a director and actors based on the end goal of the film.
  * Directors - The top directors by profit and ratings are Gore Verbinski and Sam Raimi. Paul Thomas Anderson and Clint           Eastwood are good choices for director if looking to make critically acclaimed films. Anne Fletcher and Robert Luketic,       known for "chick flicks" are top choices if looking for a director to provide high ROI.
  * Actors - Paul Bettany is the top overall actor of every success category, followed by Robert Downy Jr and Chris Hemsworth.     Natalie Portman and Gwyneth Paltrow should be enlisted if interested in making critically acclaimed films.  Diedrich Bader       and Danny Glover are good choices for actors who provide high ROI.

Determining top directors and actors by genre would be an interesting extension to this project, but is beyond the scope of this work for now. This was a small sample of movies that were selected based on the new movie studio's current situation. There are thousands upon thousands more films that could be analyzed to give us a true global picture of what makes movies successful. We are also evolving to a new world where streaming services are the new box office. We would have to come up with an effective way to quantify the profits each individual movie released through streaming services generates. This would be an interesting followup project when more data is available.

## For More Information

Please review my full analysis in [my Jupyter Notebook](./IMDB_movies_analysis.ipynb) or my [presentation](./IMDB_movies_analysis_presentation.pdf).

For any additional questions, please contact **Melody Bass @ meljoy1099@gmail.com**

## Repository Structure

```
├── README.md                           <- The top-level README for reviewers of this project
├── IMDB_movies_analysis.ipynb.ipynb    <- Narrative documentation of analysis in Jupyter notebook
├── IMDB_movies_analysis_pres.pdf       <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
└── code.                               <- Both sourced externally and generated from code
```
