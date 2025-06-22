# Movie Recommendation System using KNN and Cosine Similarity

This project demonstrates a simple yet effective approach to building a **movie recommendation system** using the MovieLens 100k dataset. The system recommends similar movies based on genre similarity and popularity using **cosine similarity** and **K-Nearest Neighbors (KNN)** logic.

## 📁 Dataset Used

- **MovieLens 100k** dataset:
  - `u.data`: Contains user ratings for movies
  - `u.item`: Contains metadata including genre and title

## 📌 Features

- Calculates average ratings and number of user ratings for each movie
- Computes **popularity** scores by normalizing the number of ratings
- Merges movie metadata with ratings for enriched recommendations
- Computes **distance** between movies using:
  - Cosine similarity on genre features
  - Popularity difference
- Retrieves `k` most similar movies to a given movie

## 🛠️ Libraries Used

- `pandas`, `numpy` — Data manipulation and analysis
- `matplotlib`, `seaborn` — Data visualization
- `scipy` — Cosine similarity calculation

## 🚀 Usage

1. Place the MovieLens dataset inside a folder named `ml-100k`.
2. Run the main script to build the movie metadata and rating matrices.
3. Use the `similarMovie(movie_id, k)` function to get the top `k` recommendations for any movie.

## 💡 Example

```python
similarMovie(50, 10)
```

Output:
```
10 Nearest Movies to Star Wars (1977)
Sr.No  Ratings  Movie Name
1.     4.01     Return of the Jedi (1983)
2.     4.21     Empire Strikes Back, The (1980)
...
```

## 📊 Result

- Recommendations are intuitive and aligned by genre and popularity.
- Flexible to scale with more features such as tags, content, or collaborative filtering.

## 📌 Author

Developed by Harsh Tyagi as a part of an educational project on recommender systems.
