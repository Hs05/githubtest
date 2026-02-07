# recommendation system in python
# Movie Recommendation System

A simple movie recommendation system using Python and machine learning.

## What it does

- **Demographic Filtering**: Finds popular, well-rated movies using a weighted rating system
- **Content-Based Filtering**: Recommends movies similar to ones you like based on plot descriptions

## Requirements

```bash
pip install numpy pandas matplotlib scikit-learn
```

## Dataset

Download the TMDB 5000 Movie Dataset and place in a `dsn1` folder:
- `tmdb_5000_credits.csv`
- `tmdb_5000_movies.csv`

[Get dataset from Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## Usage

```bash
python movie_recommendation.py
```

Enter a movie name when prompted to get 5 similar recommendations.

## How it works

**Demographic Filtering**: Uses IMDB's weighted rating formula to balance popularity with quality, preventing movies with few votes from ranking unfairly high.

**Content-Based Filtering**: 
1. Converts movie descriptions to numbers using TF-IDF
2. Calculates similarity scores between all movies
3. Returns the most similar movies to your input

## Example

```
Enter the Name of the Movie: The Dark Knight

Recommendations:
- Batman Begins
- The Dark Knight Rises  
- Batman Returns
- The Prestige
- Inception
```
