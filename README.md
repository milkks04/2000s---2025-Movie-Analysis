# 🎬 2000s–2025 Movie Analysis

This project analyzes trending movies released between **2000 and 2025** to see how movie 
ratings, popularity, and release patterns have changed over time. It was created as my 
CIS 2100 final project and as a portfolio piece.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/milkks04/2000s---2025-Movie-Analysis/blob/main/notebooks/FinalProject_Ontiveros_Miles.ipynb)

---

## 📚 Overview

I focused on movies from the 2000s up to 2025 because I love that era and also wanted to see 
what’s happening now that streaming is taking over and theater culture is fading. The notebook 
cleans the dataset, extracts the release year, and looks at trends like:

- How average movie ratings change over time  
- How many movies are released each year  
- Which years and languages have the most high-rated movies (8.0+)  
- How movie ratings are spread out in the streaming era  

Each graph includes a styled HTML “INFO” section that explains what the chart is showing in 
simple terms.

---

## 🎞️ Dataset

- **Rows:** ~10,000 movies  
- **Key columns used:**
  - `title`
  - `original_language`
  - `release_date`
  - `vote_average`
  - `vote_count`
  - `popularity`
- **New column created:**
  - `release_year` (extracted from `release_date`)

---

## ✨ Features

- Reusable cleaning function: `clean_movies(df)`
- Helper function: `get_movies_by_year(df, year)`
- Loop + conditional logic to count how many movies are above the average rating
- Year summary table with:
  - Average rating per year  
  - Number of movies per year  
  - Average popularity per year  
  - Total votes per year  
- Visualizations:
  - Line plot – average rating by year  
  - Bar chart – number of movies released per year  
  - Heatmap – high-rated movies (≥ 8.0) by year and language  
  - Scatter plot – rating vs. release year  
- HTML “INFO” sections under each plot with explanations

---

## 🛠 Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Jupyter Notebook / Google Colab

---

## ▶️ How to Run

1. Clone or download this repository.  
2. Make sure `Trending_Movies.csv` is in the same folder or inside a `data/` folder.  
3. Open `FinalProject_Ontiveros_Miles.ipynb` in Jupyter or Google Colab.  
4. Run all cells in order to see the cleaning steps, visualizations, and conclusions.

---

## 🧠 Key Insights (Quick Summary)

- Average ratings stay mostly between **6.0 and 6.8**, showing that overall movie quality is 
  pretty stable over time.
- The number of movies released per year jumps a lot in the 2020s, especially once streaming 
  platforms become more common.
- High-rated movies (8.0+) appear more often in the 2010s and 2020s.
- Rating spreads get wider in recent years, meaning there are more really good and really bad 
  movies as streaming ramps up.
