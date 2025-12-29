# 🎬 Movie Recommendation System (Content-Based)

### 🚀 Day 11 of 30: Machine Learning Projects Challenge

**Goal:** Build a "Netflix-style" recommendation engine that suggests movies based on content similarity.
**The Problem:** How does a computer know that *Iron Man* is similar to *Captain America*?
**The Solution:** We use **TF-IDF (Term Frequency-Inverse Document Frequency)** to convert movie plots and metadata into mathematical vectors, then measure the angle between them using **Cosine Similarity**.

---

## 🛠️ Tech Stack
* **Python**
* **Scikit-Learn** (TF-IDF, Cosine Similarity)
* **Pandas & NumPy** (Data Manipulation)
* **Difflib** (For handling user spelling mistakes)
* **Matplotlib & Seaborn** (For visualizing the results)

---

## ⚙️ How It Works
1.  **Feature Engineering:** We combine `Genres`, `Keywords`, `Tagline`, `Cast`, and `Director` into a single "Content DNA" string for each movie.
2.  **Vectorization:** We use **TF-IDF** to turn this text into numbers. Unlike simple counting, TF-IDF gives more weight to unique/important words (like "Alien" or "Wizard") and less weight to common words.
3.  **Similarity Matrix:** We calculate the Cosine Similarity between all 4,800 movies.
4.  **Interactive Loop:**
    * The system asks the user for a movie.
    * It uses `difflib` to fix typos (e.g., "Avatar" -> "Avatar").
    * It finds the 10 closest vectors.
    * **Visualization:** It displays a bar chart showing the "Confidence Score" of the recommendations.

---

## 📊 Visualization
The project includes:
* **Word Clouds** to visualize the most common themes in the dataset.
* **Bar Charts** to show the similarity strength of recommended movies.

---

## 📝 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/TomarBondhuRashed/movie-recommender.git](https://github.com/TomarBondhuRashed/movie-recommender.git)
    ```
2.  **Download Data:**
    Download `tmdb_5000_movies.csv` from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) and place it in the folder.
3.  **Run the script:**
    ```bash
    python movie_recommender.py
    ```

---

## 🤝 Connect
Follow my 30-day coding journey!
* **LinkedIn:** [Your Profile Link]
* **GitHub:** [TomarBondhuRashed](https://github.com/TomarBondhuRashed)
