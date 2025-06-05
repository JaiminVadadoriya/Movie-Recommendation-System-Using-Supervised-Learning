# 🎬 Movie Recommendation Classifier using PyTorch

A binary classification machine learning project built with PyTorch, using the MovieLens 100k dataset. The model predicts whether a user will like a movie (rating ≥ 4) based on user and movie IDs using embeddings and a feedforward neural network.

---

## 🚀 Project Highlights

- 🔍 Supervised Learning: Binary classification (`like` or `not like`)
- 📊 Real-world Dataset: [MovieLens 100k](https://grouplens.org/datasets/movielens/100k/)
- 🧠 Deep Learning with PyTorch:
  - Learned embeddings for user and movie IDs
  - Feedforward neural network (MLP)
  - Uses `BCEWithLogitsLoss` for numerical stability
- 💡 Optional optimizers: SGD with momentum or Adam
- ✅ Includes full training, evaluation, and classification metrics

---

## 🧠 Model Overview

- Input:
  - `user_id`, `movie_id` (encoded and embedded)
- Architecture:
  - `Embedding(user_id)` + `Embedding(movie_id)` → `Concat` → `FC → Dropout → FC → Output`
- Output:
  - Probability that a user will like a given movie
- Loss:
  - `BCEWithLogitsLoss` (sigmoid applied at prediction time)

---

## 📁 Files

| File | Description |
|------|-------------|
| `Movie_Recommendation_System.ipynb` | Full model, training and evaluation pipeline |
| `README.md` | Project overview and instructions |

---
