# Spotify Dataset Analysis

This project is an exploratory data analysis (EDA) of a processed **Spotify** dataset containing information on 85,000 music tracks. The analysis covers the time period from **2015 to 2025** and focuses on studying popular genres, track metrics, artist activity, and factors influencing streaming performance and overall popularity.

---

## 📌 Dataset Overview

* **Dataset Size:** 85,000 records and 33 columns[cite: 1].
* **Time Span:** January 1, 2015 – December 31, 2025[cite: 1].
* **Data Types:** Categorical (genres, keys, modes), numeric (duration, popularity, loudness, stream count), temporal (release date), and boolean (explicit content, weekend release)[cite: 1].

---

## 📊 Key Metrics & Data Structure

The table below describes the primary attributes included in the dataset:

| Category | Columns | Description |
| :--- | :--- | :--- |
| **Identification** | `track_id`, `track_name`, `artist_name`, `album_name` | Unique identifiers and track/artist metadata[cite: 1] |
| **Release Info** | `release_date`, `release_year`, `release_quarter`, `is_weekend_release` | Release date and temporal indicators[cite: 1] |
| **Audio Features** | `danceability`, `energy`, `loudness`, `tempo`, `key_name`, `mode_name` | Acoustic and structural track attributes[cite: 1] |
| **Popularity** | `popularity`, `stream_count`, `log_stream_count`, `popularity_category` | Popularity scores and streaming metrics[cite: 1] |
| **Artist Metrics** | `artist_track_count`, `upbeat_score`, `explicit` | Artist activity metrics and track flags[cite: 1] |

---

## 📈 Key Insights

**1. Genre Distribution & Popularity**
* **Top Genres by Streams:** **Hip-Hop** leads with an average of ~266,308 streams per track, followed by **R&B** (~229,478) and **EDM** (~222,381)[cite: 1].
* **Average Popularity by Genre:** Popularity score averages remain fairly even across genres (ranging between ~47.8 and 48.3)[cite: 1].

**2. Yearly Trends**
* Track release counts are evenly distributed across the years (~7,468 to ~7,940 tracks per year)[cite: 1].
* Average popularity levels remain stable throughout 2015–2025 (~48.0–48.4)[cite: 1].

**3. Correlation Analysis**
* A positive correlation exists between `popularity` and stream volume (`stream_count`, $r \approx 0.358$)[cite: 1].
* Audio features (`danceability`, `energy`, `loudness`, `tempo`) show weak linear correlation with raw popularity scores[cite: 1].

---

## 🛠 Tech Stack

* **Python 3.x**
* **Pandas** — Data loading, cleaning, aggregation, and feature manipulation[cite: 1]
* **NumPy** — Mathematical and vectorized operations[cite: 1]
* **Matplotlib / Seaborn** — Data visualization and correlation heatmaps[cite: 1]

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/data-analys-spotify-artists.git](https://github.com/your-username/data-analys-spotify-artists.git)
   cd data-analys-spotify-artists
