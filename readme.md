# 🎵 Spotify Music Analysis (1980–2020)

### 📊 Data Cleaning | Exploratory Data Analysis | SQL | Python | Visualization

This project explores **Spotify music trends from 1980 to 2020** — analyzing how music characteristics have evolved across decades and what drives a song’s popularity in the modern streaming era.

---

## 🧠 Project Overview

**Goal:**  
To uncover how musical features (energy, danceability, loudness, etc.) changed over time, and how these affect a track’s popularity.  
This helps understand *listener behavior, artist evolution,* and how platforms like **Spotify** can improve recommendation systems.

**Key Objectives:**
- Clean and preprocess raw Spotify track data.
- Store and query data efficiently using **SQL Server**.
- Analyze trends in **duration, energy, acousticness, loudness, and popularity**.
- Understand correlations between audio features.
- Derive **actionable insights** for Spotify’s curation and recommendation teams.

---

## 🧹 Step 1: Data Cleaning

| Task | Description |
|------|--------------|
| 🔄 Remove Duplicates | Cleaned redundant track entries. |
| 🧾 Handle Missing Values | Dropped nulls in key numeric fields (energy, duration, popularity). |
| ⏱️ Unit Conversion | Converted `duration_ms` → `duration_min` for better readability. |
| 📅 Extract Year | Extracted `release_year` from release date. |
| 🎚️ Filter Outliers | Removed songs with unrealistic durations (>10 mins). |
| 🗄️ Storage | Stored cleaned dataset in **SQL Server** and exported a CSV for reproducibility. |

> ✅ The cleaned dataset (`spotify_tracks_cleaned.csv`) is used for all further analysis.

---

## 📈 Step 2: Exploratory Data Analysis (EDA)

### 🔹 1. Duration Trends
- Average song duration dropped from **~4.3 minutes (1980s)** to **~3.3 minutes (2020s)**.  
- Reflects *shorter attention spans* and rise of short-form content (TikTok, Reels).

### 🔹 2. Energy, Loudness, and Danceability
- Significant rise in **energy and loudness** post-2000.  
- Tracks are becoming more **energetic, danceable, and electronically produced**.  
- Strong correlation (**r = 0.74**) between *energy* and *loudness.*

### 🔹 3. Key Distribution
- **C# minor, D major, and G major** are among the most common keys —  
  indicating a dominance of *guitar- and synth-friendly tones.*

### 🔹 4. Explicit Content
- Only **15% of total tracks** are explicit.  
- But nearly **40% of popular songs** (popularity > 80) are explicit —  
  showing a clear modern preference for expressive lyrical content.

### 🔹 5. Popularity by Decade
| Decade | Avg Popularity |
|---------|----------------|
| 1980s | 37.7 |
| 1990s | 44.2 |
| 2000s | 49.7 |
| 2010s | 57.6 |
| 2020s | 64.3 |

> Popularity increased steadily — partly due to broader accessibility and global music platforms.

---

## 👥 Step 3: Artist-Level Insights

| Rank | Artist | Total Tracks | Avg Popularity |
|------|--------|---------------|----------------|
| 1 | Taylor Swift | 207 | 58 |
| 2 | Red Hot Chili Peppers | 196 | 48 |
| 3 | Eminem | 167 | 55 |
| 4 | BTS | 132 | 68 |
| 5 | Michael Jackson | 126 | 53 |
| 6 | Drake | 122 | 61 |
| 7 | Madonna | 111 | 48 |

> These artists defined eras of energetic, electronically produced pop and hip-hop — mirroring global listening trends.

---

## ⚙️ Tools & Technologies

| Category | Tools Used |
|-----------|-------------|
| 🧮 Data Analysis | Python, Pandas, NumPy |
| 📊 Visualization | Seaborn, Matplotlib, Plotly |
| 🗄️ Database | SQL Server, SQLAlchemy |
| 🧹 Data Cleaning | Pandas, Regex |
| 💻 IDEs | Jupyter Notebook, VS Code |

---

## 📉 Key Correlations

| Relationship | Correlation | Interpretation |
|---------------|--------------|----------------|
| Energy ↔ Loudness | **+0.74** | Louder songs tend to be more energetic |
| Acousticness ↔ Loudness | **–0.56** | Acoustic tracks are generally quieter |
| Danceability ↔ Loudness | **+0.27** | Slightly more danceable songs are louder |
| Popularity ↔ Energy | **+0.04** | Weak correlation – popularity not only about energy |

---

## 🧩 Actionable Insights for Spotify

1. **Personalized Recommendations:**  
   - Gen-Z prefers shorter, louder, energetic songs.  
   - Older listeners can be targeted with acoustic, lower-energy playlists.

2. **Curation Strategy:**  
   - Create playlists around trending keys (C#, D, G major).  
   - Blend explicit & non-explicit versions for user preference.

3. **Artist Support:**  
   - Artists producing high-energy music see higher engagement.  
   - Encourage focus on short, catchy intros and hooks.

4. **Platform Growth:**  
   - Rising loudness/energy aligns with algorithmic optimization —  
     use in future “vibe-based” discovery features.

---

## 💾 Project Structure

