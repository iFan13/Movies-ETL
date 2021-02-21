# Overview

This repository hosts an Extract, Transform, and Load for a database on Movies cross referencing Wikipedia and MovieLens.org. Wikipedia extract is saved as a reference in the resources folder as [wikipedia-movies.json](/Resources/wikipedia-movies.json). The movies' meta data and ratings from MovieLens.org is downloaded from [Kaggle](https://www.kaggle.com/rounakbanik/the-movies-dataset). A snapshot of the data was taken for the week of February 15, 2021 and are included in this repository in the resources folder as [movies_metadata.csv](/Resources/movies_metadata.csv) and [ratings.csv](/Resources/ratings.csv).

The data is read using Python in Jupyter Notebooks and cleaned up using knowledge of Pandas. It is then uploaded into a PostgreSQL database (specifically, PGAdmin).

A total of 6052 movies are imported into the database and raw data for the ratings is also added (totalling 26,024,289 ratings across all movies) as proven by the below queries

![query-movies](/Resources/movies_query.png)

![query-ratings](/Resources/ratings_query.png)
