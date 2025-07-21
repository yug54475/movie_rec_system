# 🎬 Movie Recommender System (TMDB Dataset)

A **content-based movie recommender system** built using the TMDB 5000 Movies Dataset. This project suggests similar movies based on the one you like — using NLP and cosine similarity techniques.

---

## 📌 Features

- 🔍 Recommend top 5 similar movies
- 🖼️ TMDB poster and overview integration via API
- 🧠 Preprocessing of movie metadata (genres, cast, director, keywords)
- 💾 Fast predictions using pickled models
- 🌐 Interactive Streamlit web app

---

## 📂 Dataset

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

**Source**: [TMDB 5000 Movie Dataset on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## ⚙️ How It Works

- Extracts features like **genres**, **cast**, **crew**, and **keywords**
- Combines them into a single "tag" string per movie
- Vectorizes these tags using **CountVectorizer**
- Computes similarity using **cosine similarity**
- Returns top N most similar movies

---

## 🚀 Run Locally

1. **Clone the repository**
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
⚠️ model/similarity.pkl is excluded from the repo due to GitHub's 100 MB file limit. You’ll need to re-run the notebook to regenerate it.

🛠 Tech Stack
Python

Pandas, NumPy, Scikit-learn

Natural Language Processing (NLP)

Streamlit

Pickle (for model storage)

