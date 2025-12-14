# Book Recommender System 📚

This project is a **Flask-based Book Recommender System** that suggests similar books based on user input.  
It integrates machine learning outputs into a simple web application to demonstrate how recommendation logic can be served through a browser interface.

The project focuses on clarity, structure, and practical backend integration rather than heavy UI design.

---

## Overview

The application allows users to:
- View a list of popular books on the homepage
- Enter a book title
- Receive recommendations for similar books

The recommendations are generated using **collaborative filtering**, with similarity scores precomputed and stored using pickle files.

---

## Tech Stack

- **Python**
- **Flask**
- **NumPy**
- **Pandas**
- **Scikit-learn**
- **HTML (Jinja Templates)**

---

book_recommender_system/
│
├── app.py
├── requirements.txt
├── popular.pkl
├── pt.pkl
├── books.pkl
├── similarity_scores.pkl
│
├── templates/
│   ├── index.html
│   └── recommend.html
│
└── static/
    ├──style.css
    ---

## How It Works

1. Book data and similarity matrices are preprocessed and stored as pickle files.
2. Flask loads these files at startup.
3. The homepage displays popular books.
4. When a user submits a book name:
   - Similar books are identified using the similarity matrix
   - Book details such as title, author, and image are retrieved
   - Recommendations are displayed on a separate page

---

## Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/niishaparashar/book_recommender_system.git
cd book_recommender_system

 2. Create a virtual environment (optional but recommended)

python -m venv venv
venv\Scripts\activate   # Windows
3. Install dependencies

pip install -r requirements.txt
4. Run the application

python app.py
5. Open in browser

http://127.0.0.1:5000
```
#Notes:

1.Book titles are case-sensitive and must match the dataset.

2.All pickle files must remain in the root directory for the application to work correctly.

3.The project prioritizes backend functionality over UI design.

## Live Demo

The application is deployed and accessible here:  
🔗 https://booknet-9eos.onrender.com/




