# 🎮 Game Recommender System

This project is a **video game recommendation system** built with Python and collaborative filtering techniques. 

---

## 📁 Dataset

The dataset (`3A.tsv`) contains detailed information about video games, including:

| Column Name       | Description                               |
|-------------------|-------------------------------------------|
| `Name`            | Game title                                |
| `Platform`        | Platform (e.g., PS4, Xbox, Wii)           |
| `Year_of_Release` | Release year                              |
| `Genre`           | Game genre                                |
| `Publisher`       | Game publisher                            |
| `NA_Sales`        | North America sales (in millions)         |
| `EU_Sales`        | Europe sales                              |
| `JP_Sales`        | Japan sales                               |
| `Other_Sales`     | Sales in other regions                    |
| `Global_Sales`    | Total global sales                        |
| `Critic_Score`    | Score from critics (0–100)                |
| `User_Score`      | Score from users (0–10)                   |
| `Rating`          | ESRB Rating (E, T, M, etc.)               |

---

## 🧠 Recommendation Approach

I use a **User-Based Collaborative Filtering** method:

- Build a user-game rating matrix
- Calculate similarity between users (cosine similarity)

Alternative approaches like item-based filtering and matrix factorization (e.g., SVD) can also be explored.

---

## 🛠️ Implementation Overview

1. **Data Preprocessing**  
   - Load and handling anomalies TSV file  

2. **Similarity Calculation**  
   - Cosine similarity to find similar users

3. **Recommendation Generation**  
   - Recommend top-5 games
