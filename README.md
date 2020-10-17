# Listen Up! 

Project 1 for Rutgers Data Science Bootcamp

# Team Members

* [Ben Kramskoi](https://github.com/kramskb1)
* [Chloe Veras](https://github.com/cveras33)
* [Jennifer Dean](https://github.com/Jen-Dean) 
* [Jordan Chatman](https://github.com/JordanChat)
* Khush Patel
* Saroja Shreenivasan

# Data Sources & APIs

## [Spotify Web API](https://developer.spotify.com/documentation/web-api/)

#### 1) Music Preference History

1. How music changed over time? 
  * Danceability, energy, liveliness, etc
  
2. Genre popularity over the course of history

3. Genre popularity vs Location

#### Music Deserts

1. Are there areas in the world where Spotify is less available than others?

2. Does Country Availability differ by artist/genre/ etc?
  * Does attribute popularity vary by country?
  
3. Does that availability differ with popularity 
  * i.e. - if heavy metal isn’t largely available in China, does it still have some level of popularity?
  
#### Time of Year

1. Do certain genres become more popular at specific times of the year? 
  * i.e - Does Christmas music get more popular around December?
  
2. Do certain genres maintain popularity all year long? 

3. Do certain attributes have a corelation with the time of year?

#### Bonus Questions

1. Based on loudness - do people skip songs or listen to them? 
  * ie: if the song is a lower loudness or volume, do people listen to it or skip it?

## Supplementary Data Sources

#### [Kaggle](https://www.kaggle.com/)

#### [Spotipy](https://github.com/plamere/spotipy)


# [Attributes](https://developer.spotify.com/documentation/web-api/reference/object-model/#audio-features-object)


**acousticness** - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.

**danceability** - Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.

**duration_ms** - The duration of the track in milliseconds.

**energy** - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.

**instrumentalness** - 	Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.

**key** - The key the track is in. Integers map to pitches using standard Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on.

**liveness** - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.

**loudness** - 	The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.

**mode** - 	Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.

**speechiness** - Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.

**tempo** - The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.

**time_signature** - An estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure).

**valence** - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).

