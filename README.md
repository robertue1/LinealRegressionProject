# Predicting Worldwide Total Gross of movies. 
by Roberto Linares



## Abstract

Deciding on which movies distributions rights to acquire, is a harder task during these times of change, 
that's why, my goal is to analyze more than 1000 movies and their lifetime performance in the worldwide box office, and determine
which are the most influential factors that yield to higher numbers in the box office. The result will be a linear model that will
provide a prediction of the amount of money a movie will earn on the worldwide scene. 

## Design

To reach the prediction goal of this project, I decided to analyze features like budget, runtime, MPPA rating, the distributor, and the genres a movie belongs to. For the data acquisition task, web-scraping was used to obtain an initial dataset of movies, but as data was missing, I used Selenium to go over all of the movies (in the Wikipedia website) titles with missing values to impute the missing values. 
Since there were categorical non-ordinal features, the implementation of dummy variables was needed. Once different models' performance were compared, 
I chose a Lasso Regression model for making predictions.
## Data

Main sources of data for this project:
- [BoxOfficeMojo](http://boxofficemojo.com/)
- [Wikipedia](https://en.wikipedia.org/wiki/Main_Page)

From BoxOfficeMojo I was able to extract the bulk of the data, but, as it is almost always the case, data was missing. That is why, I scraped the movie titles with missing values from Wikipedia in an attempt to impute the data.

One row of data for this project holds: Title, domestic opening, domestic lifetime gross, worldwide lifetime gross, budget, duration, release date, 
distributor, and genre for each one of the movies. 

## Algorithms

* Data Acquisition: Using web-scraping tools to obtain the data. 
* Data Exploration: Observation of the data and its characteristics, looking for missing or unexpected values. 
* Data Cleaning: Done initially and almost throughout the entire process.
* Data Transformation: Creating dummy variables for the categorical non-ordinal features and standardization of the numeric ones for use in the regularized models.
* Data Visualization: Studying the performance of the models via graphs. 


## Models

Linear and Polynomial regression, Ridge and Lasso. 

Model Evaluation and Selection

Initially, a simple train/validation/test was used for the selection of the model, but then, I used a more rigorous cross-validation scheme. 
The best performing model was used, but due to the amount of features that were considered, a Lasso Regression implementation was used to make the predictions. 


## Tools

* BeautifulSoup and Selenium for web-scraping (data acquisition)
* Numpy and Pandas for data manipulation
* Scikit-learn for modeling
* Matplotlib and Seaborn for plotting

## Communication

Submitted PDF slides and 5 minutes presentation. 
