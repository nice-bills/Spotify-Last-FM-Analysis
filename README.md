# Music Analysis Project

This project analyzes music listening patterns and song characteristics using personal Spotify data. It combines music information and listening history to provide insights about musical preferences and popular keywords/tags associated with frequently played songs.

## Data Sources

The data used in this project is sourced from a Kaggle dataset containing Spotify music + Last.fm information and user listening patterns.

The project uses two main data files:
- `Music Info.csv`: Contains detailed information about songs including:
  - Track information (ID, name, artist)
  - Audio features (danceability, energy, tempo, etc.)
  - Tags and genres
  - Spotify-specific metadata

- `User Listening History.csv`: Contains personal listening history including:
  - Track IDs
  - User IDs
  - Playcounts

## Features

The analysis includes:
1. Most common keywords/tags in popular songs
2. Listening pattern analysis (time of day, day of week)
3. Audio feature analysis of popular songs
4. Tag co-occurrence in frequently played music
5. Correlation between audio features
6. Popularity distribution across different music tags

## Requirements

Required Python libraries:
```
pandas
numpy
matplotlib
seaborn
```
Required datasets from [Million Song Dataset + Spotify + Last.fm](https://www.kaggle.com/datasets/undefinenull/million-song-dataset-spotify-lastfm)

## Usage

1. Ensure both CSV files are in their respective directories:
   - `Music Info.csv/Music Info.csv`
   - `User Listening History.csv/User Listening History.csv`

2. Run the analysis code to see:
   - Visualizations of popular tags
   - Audio feature correlations
   - Listening pattern distributions
   - Tag relationships in popular songs

## Visualizations

The analysis produces several visualizations:
- Bar plots of top keywords
- Correlation heatmaps of audio features
- Distribution plots of listening patterns
- Tag co-occurrence networks

## Data Structure

### Music Info Dataset Columns:
- track_id
- name
- artist
- spotify_preview_url
- spotify_id
- tags
- genre
- year
- duration_ms
- Audio features (danceability, energy, etc.)

### Listening History Dataset Columns:
- track_id
- user_id
- playcount

## Analysis Components

1. **Tag Analysis**
   - Frequency counting
   - Popularity weighting
   - Co-occurrence patterns

2. **Audio Feature Analysis**
   - Feature correlations
   - Popular song characteristics
   - Genre-specific patterns

3. **Listening Pattern Analysis**
   - Temporal patterns
   - Favorite artists/genres
   - Play count distributions 