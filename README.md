# movie-recommendation-system
python project that recommends 5 other movies you might like based on your favorite movie
# Features:
What your system can do:
Recommend movies based on a selected movie.
Uses content features: genre, decade, runtime, IMDB rating.
Cleaned and preprocessed movie dataset with one-hot encoding for categorical features and scaling for numeric features.
Optional: could be extended to include directors and stars.
# Dataset:
imdb top 1000 best movies
Number of movies after cleaning: 749.
Features included: Genre, Runtime, IMDB Rating, Decade, etc.
cleaning steps: 
dropped Poster_Link, Certificate, Overview
scaled released_year, Runtime, genre, imdb_rating, meta_score into readable and usable formats.
# How it works:
Step-by-step explanation:
Cleaned and preprocessed dataset (drop irrelevant columns, handle NaNs, extract features).
Encode categorical features (genre, decade) as one-hot vectors.
Scale numeric features (runtime, rating) to 0–1.
Combine features into a single movie vector.
Compute cosine similarity between all movie vectors.
Recommend top-N most similar movies for a selected movie.
# How to use:
example: input: the godfather
output:
You might also like:
- The Godfather: Part II
- Taxi Driver
- One Flew Over the Cuckoo's Nest
- A Clockwork Orange
- The Sting
## Requirements
- Python 3.10+
- Packages:
  - pandas
  - numpy
  - scikit-learn
  - jupyter
