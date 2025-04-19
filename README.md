# 🎬 Movie Recommendation System

This is a content-based movie recommendation system built using Python, Pandas, Scikit-learn, and Streamlit. It uses metadata such as genres, keywords, overview, cast, and crew to recommend movies similar to a user's favorite.

## 🚀 Live Notebook
👉 [View the full notebook on Kaggle](https://www.kaggle.com/code/atripal2029/movie-recommendation-system)

---

## 📂 Project Overview

### 🧠 How it works:
- Extracts important textual features from the TMDB 5000 Movie Dataset.
- Combines selected metadata into a single "tags" column.
- Applies **CountVectorizer** to convert tags into numerical vectors.
- Computes **cosine similarity** between all movie vectors.
- Retrieves the top 5 similar movies based on user selection.
- Fetches posters using the TMDB API for a visual experience.

### 📺 Frontend
- Built with **Streamlit** for a clean and interactive UI.
- Users select a movie title from a dropdown.
- Displays poster thumbnails of recommended movies.

---

## 📊 Dataset

- **Source:** [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Includes: movie titles, overviews, genres, keywords, cast, crew, etc.

---

## 📦 Tech Stack

- Python
- Pandas
- Numpy
- Scikit-learn
- Streamlit
- Pickle
- TMDB API

---

## 📁 Files

| File | Description |
|------|-------------|
| `movie_recommendation_system.ipynb` | Jupyter notebook containing the full code |
| `movies.pkl` | Processed movie data with combined features |
| `similarity.pkl` | Precomputed cosine similarity matrix |
| `app.py` | Streamlit application code (optional if converted) |

---

## 📌 Installation (Optional for Local Use)

```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
pip install -r requirements.txt
streamlit run app.py
