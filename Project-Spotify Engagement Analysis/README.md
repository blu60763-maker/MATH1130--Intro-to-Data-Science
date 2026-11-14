# Spotify Track Performance & Listener Engagement Analysis

---

## Introduction

### Business Context
The digital music streaming industry relies heavily on understanding listener engagement and evolving audio trends[cite: 4, 15, 16]. Streaming platforms and record labels continuously seek data-driven strategies to optimize album releases, improve playlist recommendation engines, and guide artists on collaborative ventures to maximize audience reach and streaming performance[cite: 16].

This project was conducted as part of **Data Science 1130** by **Tien Hoang, Brandon Lu, Zisheng Yuan, Jiyao Yin, and Hassan Khalid**[cite: 3, 15]. Using Spotify track-level data, the study investigates how breakout hits influence the broader consumption of album tracks and how artist collaborations alter core musical characteristics[cite: 4, 15].

---

### Business Problem
The primary objective is to evaluate listener behavior patterns and track composition to answer two strategic industry challenges:
1. **The Album "Halo Effect":** Determine whether the presence of a breakout hit lifts engagement and popularity across other tracks within the same album, and evaluate how genre diversity mediates this dynamic[cite: 4, 15].
2. **Collaboration Dynamics:** Evaluate how foundational audio features (e.g., danceability, energy, speechiness, valence, tempo) shift when artists collaborate compared to when they release solo work[cite: 1, 4, 15].

---

### Analytical Context
The analysis utilizes a comprehensive Spotify dataset (`dataset.csv`) comprising approximately **114,000 tracks** spanning across **114 unique genres**[cite: 1, 17]. 

**Key Dataset Attributes Include:**
* **Metadata:** `track_id`, `track_name`, `album_name`, `artists`, `track_genre`[cite: 1, 2]
* **Engagement & Performance:** `popularity` (0–100 scale), `duration_ms`[cite: 1, 2]
* **Acoustic & Audio Features:** `danceability`, `energy`, `loudness`, `speechiness`, `acousticness`, `instrumentalness`, `liveness`, `valence`, `tempo`[cite: 1, 2]

**Core Analytical Tasks:**
1. **Data Cleaning & Preprocessing:** Filter duplicates, handle missing values, aggregate multi-genre track instances, and remove spoken-word audio (`speechiness >= 0.66`)[cite: 1, 2, 4].
2. **Engagement & Dispersion Modeling:** Analyze correlation matrices, measure popularity deltas relative to album peaks, and compare broad vs. niche album distributions[cite: 2, 4].
3. **Statistical Hypothesis Testing:** Conduct two-sample independent t-tests across individual genres to identify statistically significant attribute shifts between solo and collaborative tracks[cite: 1, 6].

---

### Research Questions
This project investigates the following primary questions:

1. **Album Engagement & Spillover:** Does a high-popularity track positively correlate with the overall average popularity of an album, and does it drive broader listener exploration of adjacent songs[cite: 2, 4, 15]?
2. **Genre Breadth vs. Niche Appeal:** How does the spread of track popularity differ between genre-diverse albums (e.g., *Greatest Hits*) and single-genre niche albums (e.g., *The Complete Hank Williams*)[cite: 2, 4, 7]?
3. **Solo vs. Collaborative Audio Profiles:** Which musical attributes (such as danceability, valence, or energy) show statistically significant changes when artists collaborate compared to solo releases[cite: 1, 6, 15]?
4. **Top Genre Consistency:** Do collaborative shifts in musical features remain consistent across Spotify's top 10 most popular genres[cite: 1, 6]?
