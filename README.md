
# 📚 Book Recommender System

A machine learning-based book recommender system built using collaborative filtering. This web application helps users discover new books based on user ratings and similarities using a pre-trained recommendation model.

---

## 🚀 Features

* 📈 Recommends books based on user preferences using collaborative filtering.
* 🔥 Displays popular books based on average ratings and number of votes.
* 🧠 Uses a similarity matrix and user-book pivot table for recommendations.
* 🖼️ Shows book title, author, and cover image.
* 🌐 Deployed via Flask with a simple HTML frontend.

---

## 🧾 Dataset

This project uses the [Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset) from Kaggle, which includes:

* **Books.csv** – Metadata about books.
* **Users.csv** – User details.
* **Ratings.csv** – User ratings for books.

---

## 🗂️ Project Structure

```
BOOK-RECOMMENDER/
│
├── env/                      # Python virtual environment (optional)
├── templates/
│   ├── index.html            # Home page with popular books
│   └── Recommender.html      # Page to show recommended books
│
├── books.pkl                 # Book metadata
├── main.py                   # Flask application
├── popular.pkl               # Precomputed popular books
├── pt.pkl                    # User-book pivot table
├── similarity_scores.pkl     # Similarity matrix for recommendations
```

---

## ⚙️ How it Works

1. The **collaborative filtering model** uses user-item interaction matrix (`pt.pkl`) and computes **cosine similarity** between users/books.
2. A query book is selected, and the top similar books are retrieved using `similarity_scores.pkl`.
3. Additional metadata is fetched from `books.pkl` to display book details.
4. Popular books are loaded from `popular.pkl`.

---

## 💡 Dependencies

Make sure to install the following Python packages:

```bash
pip install flask pandas numpy scikit-learn
```

---

## 🖥️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/book-recommender.git
cd book-recommender
```

2. Activate your virtual environment (if used) and run:

```bash
python main.py
```

3. Open a browser and navigate to `http://127.0.0.1:5000/` to use the app.

---

## 📸 Screenshots

> *Add images of `index.html` and `Recommender.html` outputs for better clarity.*

---

## 📌 Future Improvements

* Allow user login & save personal recommendations.
* Integrate content-based filtering for cold-start problem.
* Add filter by genre, author, or publication year.
* Host on cloud platform (e.g., Heroku, AWS, or Render).

---

## 👨‍💻 Author

* **Aryaman Dev Kumar** 

