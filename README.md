# 🎬 Movie Recommendation System (Content-Based Filtering)

## 🚀 Overview

This project is a **Movie Recommendation System** built using **Content-Based Filtering** techniques. It recommends movies similar to a given movie based on features like **genre, keywords, cast, and crew**.

The model is trained on the **TMDB 5000 Movies Dataset**, and it helps users discover movies aligned with their interests.

---

## 🎯 Key Features

* 🔍 Recommend top 10 similar movies
* 🧠 Uses NLP techniques for feature extraction
* ⚡ Fast similarity search using cosine similarity
* 🎥 Clean and interactive UI (Streamlit)
* 📊 Real-world dataset (TMDB 5000)

---

## 🧠 How It Works

1. **Data Collection**

   * Dataset: TMDB 5000 Movies & Credits

2. **Data Preprocessing**

   * Merged movie and credit datasets
   * Selected important features:

     * Genres
     * Keywords
     * Cast
     * Director
   * Handled missing values

3. **Feature Engineering**

   * Combined all relevant features into a single column (`tags`)
   * Applied text preprocessing (lowercase, stemming)

4. **Vectorization**

   * Used **TfisdVectorizer** to convert text into numerical vectors

5. **Similarity Calculation**

   * Used **Cosine Similarity** to measure similarity between movies

6. **Recommendation**

   * Based on similarity score, top 5 closest movies are returned

---

## 🛠️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Streamlit

---

## 📂 Project Structure

```
Movie-Recommender-System/
│
├── app.py                # Streamlit app
├── movie_dict.pkl       # Movie data
├── TMDB_dataset.zip
└── README.md
```

---

## ▶️ How to Run Locally

1. Clone the repository

```
git clone https://github.com/your-username/movie-recommender.git
```

2. Install dependencies

```
pip install -r requirements.txt
```

3. Run the app

```
streamlit run app.py
```

---

## 💡 Sample Output

Input: *Avatar*
Output:

* Guardians of the Galaxy
* John Carter
* Star Trek
* Jupiter Ascending
* Avengers

---

