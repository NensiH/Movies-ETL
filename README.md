# Movies-ETL
## Overview:
Amazing Prime wants to keep all data updated on a daily basis and create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. The purpose of this project was to gather movie data from both wikipedia and kaggle and create a database that students can use to preform there own analysis. In order to do these, we used the following breakdown:

1. Write an ETL function to read three data files
2. Extract and transform the Wikipedia data
3. Extract and transform the Kaggle and rating data
4. Load the data to a PostgreSQL Movie Database

## Resources:
**Software:**

- Python v3.x
    - pandas, json, numpy, re, sqlalchemy, psychopg2, time

- PostgreSQL
  - pgAdmin
  
**Files:**

[movies_metadata.csv](https://github.com/NensiH/Movies-ETL/blob/main/Resources/movies_metadata.csv)

[ratings.csv](https://github.com/NensiH/Movies-ETL/blob/main/Resources/ratings.csv)

[wikipedia-movies.json](https://github.com/NensiH/Movies-ETL/blob/main/Resources/wikipedia-movies.json)

## Results:

After completing the extract, transform, and load process, I had a database with two tables: one for movies and one for ratings. The movies table has  6052 raws.

<img width="419" alt="movies_query" src="https://user-images.githubusercontent.com/92277581/146122822-a8218e13-b258-46c0-a1d3-274640e29c56.png">

The ratings table consists of 5 different columns holding a range of information on over 26 million individual user ratings.

<img width="399" alt="ratings_query" src="https://user-images.githubusercontent.com/92277581/146122830-4e9a6635-7b86-4613-9072-e3a19cc38f3f.png">

## Summary:
The ETL function collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
