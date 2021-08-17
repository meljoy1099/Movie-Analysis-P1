# IMDB Movies Analysis

**Authors**: Melody Bass

## Overview

The focus of this project is to analyze determining factors in what makes a movie successful. We will define success as a film being profitable and well received by critics and users. The original data source comes from Kaggle and can be found here and contains information of over 75,000 movies from IMDB. We will first focus on investigating the dataset and cleaning and wrangling the data into analysis format. The next sections contain questions and answers pertaining to the properties and characteristics that have made films successful over the past 20 years and the modeled data as follows:
* Movie length 
* Best month to release movies
* Production budget
* Genres
* Directors
* Actors 

## Business Problem

Microsoft wants to get into the movie business, and I have been tasked me making recommedations about what types of films to create.


***
Questions we will answer:

1- What characteristics are associated with the most successful movies?
* What movie runtime generates the most profits?
* What movie runtime is the highest rated by users and critics?
* What months are the most profitable movies released?
* Do higher production budgets lead to higher profits?
* Do higher production budgets lead to higher user and critic reviews?
* Do higher production budgets lead to higher ROI?

2- What genres are most profitable and highly rated overall and over time?
* What is the most profitable genre?
* What genre is the highest rated by users and critics?
* What is our top overall genres?

3- Who are the people who make the most successful films?
* What director generates the most profit?
* What directors have the highest user and critic ratings?
* What directors have the highest average ROI?
* What popular actors make the most profitable movies?
* What popular actors have the highest user and critic reviews?
* What popular actors have the highest average ROI?
***

## Data

The dataset used for this analysis was found on Kaggle. It is a compiled dataset containing information about 75,000 movies from IMDB. I will only use movies from the dataset that contain gross income, production budget, user and critic ratings, and were released in the United States from the year 2000 - present. I calculated profit ($M) and ROI to use as some of my parameters of movie success.  The variables that will be used to evaluate a movie's success will be profit, audience reviews, and critic reviews.

## Methods

The model used for processing and analyzing the dataset was descriptive analysis. Movie data was used from the last 21 years to give us a good representation of what is doing well now and over time.

## Results

Present your key results. For Phase 1, this will be findings from your descriptive analysis.

***
Questions to consider:
* How do you interpret the results?
* How confident are you that your results would generalize beyond the data you have?
***

Here is an example of how to embed images from your sub-folder:

### Visual 1
![graph1](./images/viz1.png)

## Conclusions

Provide your conclusions about the work you've done, including any limitations or next steps.

***
Questions to consider:
* What would you recommend the business do as a result of this work?
* What are some reasons why your analysis might not fully solve the business problem?
* What else could you do in the future to improve this project?
***

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-template.ipynb) or our [presentation](./DS_Project_Presentation.pdf).

For any additional questions, please contact **name & email, name & email**

## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```
