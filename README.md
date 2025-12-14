# 🎓 CS50 AI Project 0 — Degrees

This repository contains my solution to **Project 0: Degrees** from **CS50’s Introduction to Artificial Intelligence with Python** — a project that computes the number of degrees of separation between two actors using a breadth-first search algorithm in Python. :contentReference[oaicite:1]{index=1}

---

## 🧠 Project Overview

Inspired by the classic *“Six Degrees of Kevin Bacon”* concept, this program determines the **shortest connection path** between two actors through the movies they’ve starred in. Each step in the path connects two actors who appeared together in a film. :contentReference[oaicite:2]{index=2}

For example:
Emma Watson → Brendan Gleeson via “Harry Potter and the Order of the Phoenix”
Brendan Gleeson → Michael Fassbender via “Trespass Against Us”
Michael Fassbender → Jennifer Lawrence via “X-Men: First Class”

The degrees of separation here would be 3. :contentReference[oaicite:3]{index=3}

---

## 🚀 Features

✔ Loads actor and movie data from CSV files  
✔ Computes the **shortest path** between two actors  
✔ Uses a **Breadth-First Search (BFS)** algorithm  
✔ Returns a sequence of `(movie_id, person_id)` pairs  
✔ Command-line interface for user interaction :contentReference[oaicite:4]{index=4}

---

## 📁 Repository Structure


CS50_AI_P0_Degrees/
├── degrees.py # Main application
├── people.csv # Actors dataset
├── movies.csv # Movies dataset
├── stars.csv # Actor-movie relationships
├── util.py # BFS helper classes (Node, Frontier)
├── README.md # Project documentation


*(Datasets may be included separately or downloaded as part of the CS50 distribution code.)* :contentReference[oaicite:5]{index=5}

---

## 🛠️ Requirements

Make sure you have:

- **Python 3.8+**
- The `csv` module (part of the Python standard library)
- The project CSV files (`people.csv`, `movies.csv`, `stars.csv`)

---

## 📦 How to Run

Download or clone this repository and **run the program like this:**

```bash
python degrees.py large
```

You will be prompted to enter two actor names:
Name: Emma Watson  
Name: Jennifer Lawrence

The program will then print out the number of degrees of separation and the connecting path. 
edX

---

🧠 How It Works

Load Data:
CSV files are parsed into dictionaries mapping people to movies and movies to people. 
edX

Breadth-First Search (BFS):
The search algorithm expands neighbors by movie connections, tracking visited actors and building the shortest path. 
edX

Output Path:
If a connection is found, the script prints each movie/actor step in order. If not, it reports no connection. 
edX

