# SQL Case Study on Movie Dataset

## Introduction

This repository contains a SQL case study focusing on a movie dataset sourced from Rotten Tomatoes. The dataset provides detailed information about movies, including various metrics on critic and audience ratings.

## Dataset

### Description

The dataset contains comprehensive details about movies available on Rotten Tomatoes, including information on critic reviews, audience ratings, and movie attributes.

### Columns

- `rotten_tomatoes_link`: URL to the Rotten Tomatoes page for the movie
- `movie_title`: Title of the movie
- `movie_info`: Additional information about the movie
- `critics_consensus`: Consensus summary from critics
- `content_rating`: Content rating of the movie
- `genres`: Genres of the movie
- `directors`: Directors of the movie
- `authors`: Authors of the movie (e.g., screenplay writers)
- `actors`: Actors in the movie
- `original_release_date`: Original release date of the movie
- `streaming_release_date`: Date when the movie was made available for streaming
- `runtime`: Duration of the movie in minutes
- `production_company`: Production company that produced the movie
- `tomatometer_status`: Status of the Tomatometer (e.g., Fresh, Rotten)
- `tomatometer_rating`: Rating given by critics (Tomatometer score)
- `tomatometer_count`: Total number of critic reviews
- `audience_status`: Status of the audience rating
- `audience_rating`: Rating given by the audience
- `audience_count`: Number of audience reviews
- `tomatometer_top_critics_count`: Number of reviews from top critics
- `tomatometer_fresh_critics_count`: Number of fresh critic reviews
- `tomatometer_rotten_critics_count`: Number of rotten critic reviews

## SQL Case Study

### Objectives

The SQL case study aims to:
- Analyze the distribution of movie ratings across different genres.
- Compare critic ratings with audience ratings.
- Identify trends in movie ratings over time.
- Explore the relationship between critic reviews and the `tomatometer` rating.

### Approach

1. **Data Cleaning**: Handle missing values and inconsistencies in the dataset.
2. **Data Analysis**: Write SQL queries to extract insights from the dataset.
3. **Visualization**: Generate reports and visualizations based on the SQL query results (if applicable).

## SQL Queries and Findings

### 1. Movies with the Highest Tomatometer Rating

**Query:**
```sql
SELECT movie_title, tomatometer_rating 
FROM movies 
WHERE tomatometer_rating = 100;

