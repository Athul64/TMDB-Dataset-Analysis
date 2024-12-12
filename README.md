# TMDB Movies Dataset Analysis

### Mini Data Analysis Project

| Contents  |
| ------------- | 
| Content Cell  | 
| Dataset Description |
| Columns Description  |
| Questions for Analysis |
| Data Wrangling |
| Data Cleaning |
| Exploratory Data Analysis |
|Built with|

## Dataset Description:

This data set contains information about 10,000 movies extracted from TMDB. The dataset contains movies from 1960 to 2015. Including user ratings and revenue. Original data from Kaggle.

## Columns Description:

* `id`, `imdb_id`: unique id or IMDB id for each movie on TMDB
* `Popularity`: a metric used to measure the popularity of the movie.
* `Budget`: the total budget for the movie is USD.
* `Revenue`: the total revenue of the movie in USD.
* `original_title`: the original title of the movie.
* `cast`: the names of the cast of the movie separated by "|".
* `homepage`: the website of the movie (if it existed).
* `director`:name(s) of the director(s) of the movie (separated by "|" if there are more than one director).
* `tagline`: a catchphrase describing the movie.
* `Keywords`: keywords related to the movie.
* `Overview`: summary of the plot of the movie.
* `runtime`: total runtime of the movie in minutes.
* `genres`: genres of the movie separated by "|".
* `production_companies`:production compan(y/ies) of the movie.
* `release_date`: is the movie's release date.
* `vote_count`: number of voters in the movie.
* `vote_average`: the average user rating of the movie
* `release_year`:release year of the movie (from 1960 to 2015)
* `budget_adj`: the total budget of the movie in USD in terms of 2010 dollars, accounting for inflation over time.
* `revenue_adj`: the total budget of the movie in USD in terms of 2010 dollars, accounting for inflation over time.

## Questions for Analysis:

* Do movies with high popularity achieve high revenue?
* What are the most filmed genres in this whole dataset?
* Is there a correlation between a movie budget and its revenue?

## Data Cleaning:

Main Observations:

1. Our dataset consisted of a total of 10866 rows and 21 columns.
2. We had only 1 duplicated row which had been dropped.
3. Some columns won't be useful in answering our questions so they were dropped.
4. A few columns had many missing values that needed to be handled.
5. Columns cast director genre had values separated with a '|'.
6. release_date's data type needed to be cast.
7. We could append a column for the movie profit using the formula: profit=revenue−budget.
8. vote_average better be presented as a categorical variable that groups multiple rating values.
9. We might also categorize the profit column for better EDA

## Exploratory Data Analysis: 

After finishing our dataset cleaning, we ended up with a total of 10840 records and 10 columns. The dataset now has no duplicates nor null values, and the data types are consistent with suitable categorical variables to address our questions. We then performed some analytics and created some visualizations to answer our targeted questions.


**Q1: Do movies with high popularity achieve high revenue?**
> More popular movies receive way more revenue than less popular movies.

**Q2: What are the most filmed genres in this whole dataset?**
> Drama, Comedy, and Action are the most three filmed genres in a total of 10839 movies in our dataset.
The drama genre alone is filmed 22.6% of the time on our dataset.


**Q3: Is there a correlation between a movie budget and its revenue?**
>There is a positive correlation between budget and revenue, indicating a relation between them with little outliers found.

## Built with:
* google colab
* Python
* Pandas
* Numpy
