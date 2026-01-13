# 🎵 Music Trends, Emotion Analysis & Recommendation System (1950–2019)

## 📌 Project Overview

This project performs **exploratory data analysis (EDA), genre-wise trend analysis, lyrics-based emotion analysis, correlation analysis**, and builds a **content-based music recommendation system** using song metadata and textual features.

The dataset spans **1950 to 2019**, enabling long-term trend analysis of music genres, emotions, and audio characteristics.

---

## 🎯 Objectives

* Analyze **music trends over decades**
* Perform **genre-wise audio feature analysis**
* Understand **lyrics-based emotional patterns**
* Identify **correlations between emotions, audio features, and song age**
* Build a **content-based recommendation system** using TF-IDF & cosine similarity

---

## 🗂 Dataset

* **Source:** `tcc_ceds_music.csv`
* **Records:** 28,372 songs
* **Time Span:** 1950–2019
* **Key Columns:**

  * Metadata: `artist_name`, `track_name`, `release_date`, `genre`
  * Lyrics-based emotions: `sadness`, `violence`, `romantic`, `feelings`, etc.
  * Audio features: `danceability`, `energy`, `valence`, `loudness`, etc.

---

## 🛠 Tech Stack & Libraries

* **Python**
* **Pandas, NumPy** – Data processing
* **Matplotlib, Seaborn** – Data visualization
* **Scikit-learn** – TF-IDF vectorization & cosine similarity

---

## 📊 Exploratory Data Analysis (EDA)

### ✔ Genre Analysis

* Top genres by song count
* Songs per genre distribution
* Artist-wise song frequency

### ✔ Temporal Trends

* Distribution of songs across release years
* Energy and emotion trends over song age

### ✔ Audio Feature Analysis

* Genre-wise averages of:

  * Danceability
  * Energy
  * Valence
  * Acousticness
  * Instrumentalness
  * Loudness

### ✔ Lyrics-Based Emotion Analysis

* Genre-wise comparison of:

  * Sadness
  * Violence
  * Romantic themes
  * Feelings
* Lyrics length vs emotional intensity

---

## 🔥 Correlation Analysis

* Heatmap of correlations between:

  * Audio features
  * Lyrics emotions
  * Song length
  * Song age
* Key insights:

  * **Valence** positively correlates with **danceability & energy**
  * **Sadness** negatively correlates with **valence**
  * Older songs show distinct energy trends

---

## 🤖 Recommendation System

### 🔧 Methodology

* **Content-Based Filtering**
* Feature construction using:

  * Genre
  * Artist name
  * Track name
* **TF-IDF Vectorization**
* **Cosine Similarity** for similarity scoring

### 📌 Example

```python
get_recommendations("cry", df, tfidf_matrix, top_n=10)
```

### 🎯 Output

* Returns top 10 songs similar to the given track
* Based on textual similarity, not popularity bias

---

## 📈 Visualizations

* Genre distribution plots
* Audio feature comparison charts
* Emotion trends by genre
* Correlation heatmaps
* Recommendation result bar charts

---

## ⚙️ Installation & Usage

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/music-analysis-recommendation-system.git
cd music-analysis-recommendation-system
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements(MR).txt
```

### 3️⃣ Run the Notebook

Open Jupyter Notebook and run:

```bash
jupyter notebook
```

---

## 📌 Future Improvements

* Lyrics-based semantic embeddings (Word2Vec / BERT)
* Hybrid recommendation system
* Streamlit / Flask deployment
* User-personalized recommendations
* Mood-based playlist generation

---

## ⭐ Acknowledgements

* Kaggle / CEDS Music Dataset
* Scikit-learn documentation
* Seaborn & Matplotlib visualization tools

---
Just tell me.
