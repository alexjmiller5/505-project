# DataFrames Overview

## song_metadata_df
This DataFrame contains the metadata of each song:
- **spotify_id**: Spotify ID of the song.
- **artist**: Artist name of the primary artist.
- **name**: Song title.
- **popularity**: Popularity of the song (Range: 0-100).
- **release_date**: Release date of the song (Format: YYYY-MM-DD).
- **genres**: Genre of the song.
- **explicit**: Whether the song is tagged by Spotify as explicit.
- **Duration_ms**: The duration of the track in milliseconds.
- **featured_artists**: Featured artists on the song.

## song_sentiment_df
This DataFrame contains data that could be related to the sentiment of each song:
- **spotify_id**: Spotify ID of the song.

#### Spotify's sentiment features
- **valence**: Measures the musical positiveness (Range: 0.0 to 1.0).
- **danceability**: Suitability for dancing (Range: 0.0 to 1.0).
- **energy**: Measure of intensity and activity (Range: 0.0 to 1.0).

#### MUSE's sentiment features
- **number_of_emotion_tags**: Number of emotion tags associated (Range: 1, 40).
- **valence_tags**: Valence tags from the MUSE dataset (Range: 0.23 to 8.48).
- **arousal_tags**: Arousal tags from the MUSE dataset (Range: 0.11 to 7.27).
- **dominance_tags**: Dominance tags from the MUSE dataset (Range: 0.23 to 7.44).

#### Spotify's musical element features
- **tempo**: Estimated tempo in BPM (Range: 50-200 BPM).
- **key**: Key of the track using Pitch Class notation (0 to 11).
- **mode**: Modality of the track (0 for minor, 1 for major).

#### Other spotify features
- **instrumentalness**: Predicts if a track contains no vocals (Range: 0.0 to 1.0).
- **liveness**: Detects presence of an audience (Range: 0.0 to 1.0).
- **speechiness**: Presence of spoken words (Range: 0.0 to 1.0).
- **acousticness**: Measure of the acoustic nature (Range: 0.0 to 1.0).
- **loudness**: Overall loudness in dB (Range: -60 to 0 dB).


## song_lyrics_df
This DataFrame contains the lyrics of each song:
- **spotify_id**: Spotify ID of the song.
- **lyrics**: The raw, unprocessed lyrics of the song.