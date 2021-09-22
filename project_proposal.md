# Web-scraping and lineal regression
## Roberto Linares


# Question/need:

By developing this project, we will be able to provide the buyers of distributions rights (of motion pictures), the safest bets for the acquisition of films with a higher estimated lifetime gross. 

# Data description:

The main source of data to achieve this project's goal will be the website [Box Office Mojo](https://www.boxofficemojo.com) and the data will be obtained by using web-scraping techniques. 
The data for this project will be the titles (and other characteristics like genre, actors, budget, etc) of films. 

# Tools:

BeautifulSoup will be used for web-scraping. 
Pandas will be used to storage and clean data. 
Matplotlib and seaborn will provide us with visualizations for presenting the results, but also to perform the initial EDA. 
The lineal regression module from sklearn will be used to create the model. 


# MVP Goal:

For this project, we will aim to predict international gross of newly released films (if possible, a targeted prediction based on specific regions of the world), by analyzing previous data of domestic (USA) and worldwide lifetime gross, genre, actors, director, writer, franchise or domestic distributor, budget, running time and MPPA, of approximately 1000 films. 

