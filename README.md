# 🎬 Movie Recommendation System

A simple Movie Recommendation web application built with **Flask**, **Pandas**, and **Scikit-learn**.  
The app computes movie similarity (based on user ratings) and returns the top recommended titles for a given movie.

---

## 🔧 Features
- Search for a movie (exact or approximate) and get top similar movies
- Uses **cosine similarity** on a user–movie ratings matrix
- Lightweight Flask web interface (`index.html` + `recommend.html` templates)

---

## 🗂 Repository structure
movie_recommendation_system/
│
├── app.py # Main Flask app (entry point)
├── movies.csv # Movie dataset (titles & movieId)
├── ratings.csv # Ratings dataset (userId, movieId, rating)
├── requirements.txt # Python dependencies
├── templates/
│ ├── index.html
│ └── recommend.html
├── static/ # (optional) CSS / images
└── README.md

---

## ⚙️ Requirements
Tested with Python 3.8+.

Recommended `requirements.txt` (add this file if not present):


Flask
pandas
scikit-learn
openpyxl # optional, only if you have .xlsx files

You can create this by running:
```bash
pip freeze > requirements.txt
How to run (locally — Windows)

Open a terminal in the project folder (the folder that contains app.py).

In File Explorer: open the folder → click the address bar → type powershell → Enter

Or Shift + Right-click in the folder → Open PowerShell window here

Or use VS Code: File → Open Folder then Terminal → New Terminal

(Optional but recommended) Create and activate a virtual environment:

PowerShell:

python -m venv venv
.\venv\Scripts\Activate.ps1
Command Prompt:

python -m venv venv
venv\Scripts\activate
Install dependencies

pip install -r requirements.txt
If you don't have requirements.txt, run:

pip install flask pandas scikit-learn openpyxl
Verify dataset files are present
Ensure movies.csv and ratings.csv are in the same folder as app.py. If your datasets are named differently (e.g., train.csv), either rename them or update app.py at the top where MOVIE_CSV and RATINGS_CSV are defined.

Run the app

python app.py


You should see:

 Flask app running... Visit http://127.0.0.1:5000


Open the app in your browser
Go to: http://127.0.0.1:5000
