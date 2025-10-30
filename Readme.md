# 🎧 Analyzing the Evolution of Music: A Spotify Data Case Study (1980–2020)

## 🧭 Overview
This project explores **how popular music has evolved** over four decades using Spotify track-level data (1980–2020).  
By analyzing musical attributes like *energy, danceability, acousticness, loudness, tempo,* and *duration*, the goal is to uncover how trends in modern music have shifted and what that means for the streaming era.

---

## ⚙️ Tech Stack
| Tool | Purpose |
|------|----------|
| **Python (Pandas, NumPy)** | Data cleaning & transformation |
| **SQL (SQL Server)** | Querying, grouping, and aggregations |
| **SQLAlchemy** | Python ↔ SQL connectivity |
| **Seaborn / Matplotlib / Plotly** | Data visualization |
| **Streamlit (optional)** | Interactive dashboard |
| **Jupyter Notebook** | EDA & analysis environment |

---

## 📂 Project Workflow

### 1️⃣ Data Acquisition
- Source: Spotify Dataset (~100K tracks).  
- Loaded into SQL Server via Pandas `.to_sql()`.

### 2️⃣ Data Cleaning
- Removed duplicates and missing values.  
- Created `duration_min` and `release_year` columns.  
- Filtered only tracks from 1980 onward.  
- Standardized column names to snake_case.

### 3️⃣ Data Analysis & SQL Integration
- Connected SQL → Python via SQLAlchemy.  
- Performed decade-wise and rolling average analysis on key metrics.  
- Investigated **duration**, **energy**, **acousticness**, **loudness**, **danceability**, and **tempo**.

### 4️⃣ Exploratory Data Analysis (EDA)
- 📈 Trends over time (1980–2020)  
- 🎹 Musical key distributions by decade  
- 🔥 Popularity & explicit content trends  
- 🎤 Top artists and defining styles  
- 🔗 Correlation matrix between core musical features

### 5️⃣ Visualizations
- Line charts for temporal trends  
- Grouped bar charts for key distribution  
- Heatmap for feature correlations  
- Boxplots for outlier analysis  
- Interactive (Plotly/Streamlit) versions for dashboard deployment

---

## 📊 Key Insights
- **Songs have become shorter:** average duration dropped from 4.3 → 3.2 minutes.  
- **Energy & loudness peaked** around 2010, then slightly declined.  
- **Acousticness decreased** post-2010 → rise of digitally produced music.  
- **Explicit content increased ~3×** since 2010 — reflects hip-hop & trap culture.  
- **Minor keys gained presence**, suggesting moodier, emotional tones.  
- **Popularity weakly correlates** with audio features — success depends on more than sound metrics.

---

## 💡 Business Implications for Spotify
- Personalize recommendations using **listener era preferences** (’80s nostalgia vs. Gen-Z upbeat tracks).  
- Leverage **acoustic vs. energetic balance** for mood-based playlists.  
- Optimize **short-form, high-energy songs** for modern users with shorter attention spans.  
- Incorporate **explicit track segmentation** for better content curation and ad targeting.


