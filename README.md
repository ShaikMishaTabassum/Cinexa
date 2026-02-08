# Cinexa

**Cinexa** is a Netflix-style movie & TV recommendation platform that delivers personalized content suggestions using collaborative filtering, content-based filtering, and a hybrid recommendation approach. The project demonstrates an end-to-end, production-style recommendation system built on real-world data and exposed via a cloud-ready REST API.

---

##  Features

* Personalized movie & TV recommendations
* Collaborative filtering using user-item interactions
* Content-based filtering using movie metadata
* Hybrid recommendation model for improved accuracy
* RESTful API for serving recommendations
* Scalable, cloud-deployable architecture

---

##  Recommendation Approaches

### 1. Collaborative Filtering

Learns user preferences based on historical user–item interactions. Users with similar behavior receive similar recommendations.

* Technique: Matrix Factorization (SVD)
* Strength: Strong personalization
* Limitation: Cold-start problem

### 2. Content-Based Filtering

Recommends items similar to what a user already likes based on item features.

* Technique: TF-IDF + Cosine Similarity
* Features: Genres, metadata
* Strength: Works for new users/items

### 3. Hybrid Model

Combines collaborative and content-based recommendations to overcome individual limitations and improve overall recommendation quality.

---

##  Dataset

* **MovieLens Dataset** (GroupLens)
* Contains real-world movie ratings and metadata

Files used:

* `ratings.csv` / `ratings.dat`
* `movies.csv` / `movies.dat`

---

##  System Architecture

1. Data ingestion & preprocessing
2. Model training (Collaborative & Content-based)
3. Hybrid recommendation logic
4. API layer for serving recommendations
5. Cloud deployment

---

##  Tech Stack

* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn, Surprise
* **API Framework:** FastAPI
* **Deployment:** Docker, Cloud (AWS/Azure/GCP)

---

##  Project Structure

```
cinexa/
│
├── data/               # Dataset files
├── models/             # Trained models
├── notebooks/          # Experiments & EDA
├── app.py              # FastAPI application
├── recommender.py      # Recommendation logic
├── requirements.txt
├── Dockerfile
└── README.md
```

---

##  API Endpoints

* `GET /recommend/{user_id}`
  Returns top-N personalized movie recommendations for a given user.

---

##  Evaluation Metrics

* RMSE (Root Mean Square Error)
* Precision@K
* Recall@K

---

##  Future Improvements

* Real-time recommendations
* User profile embeddings
* Deep learning–based recommenders
* Frontend web or mobile app
* A/B testing for recommendation quality

---

##  Use Cases

* Movie & TV streaming platforms
* Content discovery applications
* Personalized media platforms

---

##  Resume Description

> **Cinexa — Netflix-style Recommendation Platform**
> Built a hybrid recommendation system using collaborative and content-based filtering on real-world data. Deployed a scalable recommendation API using FastAPI and cloud infrastructure.

---

## 👤 Author

Shaik Misha
Jogula Roy

---

⭐ If you find this project interesting, feel free to star the repository!

