
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
git clone (https://github.com/Aryamandev14/Book-Recommender-System.git)
cd Book-Recommender-System
```

2. Activate your virtual environment (if used) and run:

```bash
python main.py
```

3. Open a browser and navigate to `http://127.0.0.1:5001/` to use the app.

---

## 📸 Screenshots

<img width="1915" height="963" alt="image" src="https://github.com/user-attachments/assets/981b15a1-28d1-4850-a8d5-65e2464b9641" />
<img width="1919" height="972" alt="image" src="https://github.com/user-attachments/assets/5f0fb54f-bf26-4c93-b410-06f418454b09" />
<img width="1901" height="920" alt="image" src="https://github.com/user-attachments/assets/fdc0cba7-3e7f-4003-8872-1adf8e37563c" />




---

## 📌 Future Improvements

* Allow user login & save personal recommendations.
* Integrate content-based filtering for cold-start problem.
* Add filter by genre, author, or publication year.

---

## 👨‍💻 Author

* **Aryaman Dev Kumar** 

