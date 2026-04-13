# 🎬 CineMatch — Movie Recommendation System

A full-featured movie recommendation system with 5000+ movies, built with Python, NLP (TF-IDF + Cosine Similarity), and a beautiful dark-themed Tkinter GUI.

---

## ✨ Features

- **5000+ movies** — Hindi, English, Korean, Japanese & more
- **Genre filter** — Action, Drama, Thriller, Comedy, Romance, Sci-Fi & 15+ genres
- **Language filter** — Hindi / English / All (mix)
- **Combined filter** — Genre + Language together
- **Smart search** — Real-time autocomplete as you type
- **Similar movies** — Click any movie → get 9 similar recommendations instantly
- **Movie details popup** — Story, Cast, Director, Rating all in one view
- **NLP engine** — TF-IDF Vectorizer + Cosine Similarity
- **Beautiful UI** — Cinema-inspired dark gold theme

---

## 📁 Project Structure

```
cinematch/
│
├── main.py            ← Full Tkinter GUI (run this!)
├── recommender.py     ← NLP engine (TF-IDF + cosine similarity)
├── movies.csv         ← 5000+ movies dataset
├── generate_data.py   ← Script used to generate the dataset
├── requirements.txt   ← Python dependencies
└── README.md
```

---

## 🚀 Setup & Run

### Step 1 — Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/cinematch.git
cd cinematch
```

### Step 2 — Create virtual environment
```bash
python -m venv venv

# Windows
venv\Scripts\activate

# Mac / Linux
source venv/bin/activate
```

### Step 3 — Install dependencies
```bash
pip install -r requirements.txt
```

### Step 4 — Run
```bash
python main.py
```

---

## 🧠 How It Works

1. Movie metadata (genres, language, cast, director, overview) is merged into a single text tag per movie
2. **TF-IDF Vectorizer** converts these tags into weighted numerical vectors (8000 features)
3. **Cosine Similarity** computes similarity between every pair of movie vectors
4. When you search a movie, the engine returns the top 9 most similar ones
5. Genre + Language filters are applied on top of similarity scores

---

## 🎯 Try These Searches

| Search | You'll get |
|--------|-----------|
| `Inception` | Interstellar, Tenet, Memento, The Prestige |
| `3 Idiots` | Dangal, PK, Taare Zameen Par, Lagaan |
| `Parasite` | Snowpiercer, Burning, Oldboy, Train to Busan |
| `The Dark Knight` | Batman Begins, Joker, Se7en, The Prestige |
| `Gangs of Wasseypur` | Black Friday, Dev D, Gulaal, Udta Punjab |
| `Spirited Away` | Princess Mononoke, Your Name, Howl's Moving Castle |

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| pandas | Data loading & manipulation |
| scikit-learn | TF-IDF Vectorizer + Cosine Similarity |
| tkinter | Desktop GUI (built-in, no install needed) |

---

## 📸 Screenshots

*Cinema-inspired dark gold theme with genre color-coded cards, sidebar filters, and detailed movie popups.*
