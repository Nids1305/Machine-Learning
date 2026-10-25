# About Dataset

## Overview

A synthetic music dataset containing **10,000 tracks spanning 2010–2025**. It includes Spotify-style audio features and clearly defined target variables for machine learning.

## Why This Dataset?

Existing music datasets often lack a clearly defined target or involve licensing complexities. This dataset provides a clean, fully populated benchmark with realistic, genre-specific audio distributions.

## Target Variables

- **`viral`** — Classification target: `1` if the track's weighted audio feature score exceeds a predefined threshold; otherwise, `0`.
- **`streams`** — Regression target representing the number of streams.

The current viral rate is approximately **20–25%**.

## Columns

| Category | Columns |
|---|---|
| Identifiers | `track_id`, `track_name`, `artist`, `genre`, `release_year` |
| Audio Features | `duration_sec`, `danceability`, `energy`, `valence`, `tempo_bpm`, `acousticness`, `instrumentalness`, `speechiness`, `liveness`, `loudness_db` |
| Target Variables | `streams`, `viral` |

## Suggested Machine Learning Tasks

1. **Viral Track Prediction (Classification):** Predict `viral` using audio features.
2. **Stream Prediction (Regression):** Predict `streams`, exploring log transformation to handle skewness.
3. **Genre Analysis:** Identify genres that have disproportionately high or low virality rates.
4. **Feature Importance:** Investigate which audio features contribute most to predicting virality.

