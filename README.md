# movie-recommendation-system
Content-based movie recommender using NLP
# 🎬 Movie Recommendation System (Content-Based)

A content-based movie recommendation system built using **Natural Language Processing (NLP)** techniques on movie plot summaries.  
The system recommends movies similar to a given movie based on semantic similarity of their overviews.

---

## 🚀 Project Overview

This project uses the **TMDB 5000 Movies Dataset** to build a recommendation engine that suggests movies based on textual similarity of plot summaries.

Key techniques used:
- TF-IDF Vectorization
- Sigmoid Kernel similarity
- Data preprocessing and feature engineering
- Visualization of similarity relationships

---

## 📊 Dataset

- **tmdb_5000_movies.csv**
- **tmdb_5000_credits.csv**

Source: TMDB (The Movie Database)

Each movie includes metadata such as:
- Title
- Overview (plot summary)
- Genres
- Cast & Crew
- Popularity and ratings

---

## 🧠 Methodology

### 1. Data Cleaning & Merging
- Merged movie and credit datasets
- Removed irrelevant columns
- Retained only useful textual and metadata features

### 2. Text Vectorization
- Used **TF-IDF Vectorizer**
- Removed stopwords
- Used unigrams, bigrams, and trigrams

### 3. Similarity Computation
- Applied **Sigmoid Kernel** to compute pairwise similarity between movies
- Generated similarity matrix

### 4. Recommendation Function
- Given a movie title, the system:
  - Finds its index
  - Computes similarity scores
  - Returns the top 10 most similar movies

---

## 📈 Visualizations

The project includes:
- Similarity heatmaps
- Dimensionality reduction (PCA / t-SNE)
- Cluster visualization of similar movies

These visuals help **explain why movies are recommended**, not just what is recommended.

---

## 🧪 Example

```python
give_recommendations("Avatar")
