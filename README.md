# movie-recommender-system-tmdb-dataset
A content based movie recommender system using cosine similarity.
A content-based movie recommender system built using the TMDB 5000 Movies Dataset. This project suggests similar movies based on the movie you like, using NLP and cosine similarity techniques.

## Features

- Recommend top 5 similar movies
- TMDB poster and overview integration via API
- Preprocessing of movie metadata including genres, cast, director, keywords
- Pickle-based model for fast predictions
- Streamlit web app interface for interactive usage

## Dataset

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

Source: [Kaggle - TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## How It Works

- Extracts key features: genres, cast, crew, keywords
- Combines into a single textual "tag" for each movie
- Vectorizes tags using CountVectorizer
- Calculates similarity scores using cosine similarity
- Returns top N most similar movies

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/yug54475/movie_rec_system.git
   cd movie_rec_system
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the app

bash
Copy
Edit
streamlit run app.py
Note: The similarity matrix file (similarity.pkl) has been excluded due to GitHub's 100 MB file size limit. You’ll need to re-run the notebook or script to generate it.

Tech Stack
Python

Pandas, NumPy, Scikit-learn

Natural Language Processing (NLP)

Streamlit

Pickle (for saving models)
