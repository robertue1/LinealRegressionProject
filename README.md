# Predicting Worldwide Total Gross of movies. 
by Roberto Linares



## Abstract

Deciding on which movies distributions rights to acquire, is a harder task during these times of change, 
that's why, our goal is to analyze more than 1000 movies and their lifetime performance in the worldwide box office, and determine
which are the most influential factors that yield to higher numbers in the box office. The result will be a linear model that will
provide a prediction of the amount of money a movie will earn on the worldwide scene. 

## Design

To reach the prediction goal of this project, we decided to analyze features like budget, runtime, MPPA rating, the distributor, and the genres a movie belongs to.
Since there were categorical non-ordinal features, the implementation of dummy variables was needed. Once different models' performances were compared, 
we chose Lasso as the tool for making predictions and to determine which factors have positive or negative correlations with the target. 

## Data

Main sources of data for this project:
- [BoxOfficeMojo](http://boxofficemojo.com/)
- [Wikipedia](https://en.wikipedia.org/wiki/Main_Page)

From BoxOfficeMojo we were able to extract the bulk of the data, but, as it is almost always the case, data was missing. That is why, Wikipedia was used 
to impute the missing values. 

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

Initially, a simple train/validation/test was used for the selection of the model, but then, we used a more rigorous Cross-Validation scheme. 
The best performing model was used, but due to the magnitude of features we were considering, a Lasso implementation was done to make the predictions. 


## Tools

* BeautifulSoup and Selenium for web-scraping (data acquisition)
* Numpy and Pandas for data manipulation
* Scikit-learn for modeling
* Matplotlib and Seaborn for plotting

## Communication

Submitted PDF slides and 5 minutes presentation. 
