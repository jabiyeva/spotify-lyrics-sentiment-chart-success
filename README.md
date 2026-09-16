# 🎵 What Makes a Hit Stick? Lyrics vs. Chart Longevity

Projekt-Status: ✅ Completed

## 📌 The Question

Does what a song *says* — its lyrics — predict how long it survives on the charts, 
or is chart success driven purely by other factors? This project investigates the 
relationship between lyrical properties and chart performance across 8,000+ songs (2013–2026).

## 🛠 Tech Stack & Tools

- **Language:** Python
- **Data Manipulation:** Pandas
- **Visualization:** Matplotlib
- **NLP / Sentiment:** VADER (vaderSentiment)

## 📑 Table of Contents

- Part 1: Does Chart Longevity Predict Total Streams?
- Part 2: Does Peak Position Predict Total Streams?
- Part 3: Does Lyric Length Relate to Streaming Success?
- Part 4: Does Lyrical Sentiment Relate to Chart Success?
- Summary of Findings
- Recommendations
- Limitations

## 🔑 Key Findings

1. **Peak position** is the strongest predictor of total streams — songs reaching the top 20 
   dominate streaming totals, with a sharp drop-off as peak position worsens.
2. **Chart longevity** (weeks charted) shows a positive but noisy relationship with streams — 
   duration alone doesn't reliably predict success.
3. **Lyric length** shows a "sweet spot" — songs with roughly 200-500 words are overrepresented 
   among the highest-streaming tracks.
4. **Lyrical sentiment** shows no meaningful relationship with streaming success — songs across 
   the full emotional spectrum achieve both low and very high results.

*Full analysis, charts, and interpretation are in [the notebook](spotify-lyrics-sentiment-chart-success.ipynb).*

## 💡 Recommendations

- **Playlist curators / A&R:** Prioritize identifying early breakout potential (peak position) 
  over betting on chart longevity alone.
- **Songwriters/producers:** Lyric length around 200-500 words aligns with historically 
  higher-streaming songs — worth testing further, not a guaranteed formula.
- **Marketing teams:** Emotional tone in lyrics need not be a strategic constraint — dark, 
  upbeat, and neutral songs all show equal potential to become hits.

## ⚠️ Limitations

- Sentiment scoring used VADER, an English-language tool not built specifically for song lyrics; 
  non-English songs and songs missing punctuation may have less reliable scores.
- Findings show correlation, not causation — peak position itself may be driven by factors 
  (marketing, artist fame) not captured in this dataset.

## 🔗 Data Source

[Spotify Global Chart Totals & Lyrics](https://www.kaggle.com/datasets/batudev/spotify-global-chart-totals-and-lyrics) — Kaggle, by batudev. Download and place in a `data/` folder to reproduce this analysis.