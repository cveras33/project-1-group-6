# Listen Up! 

Project 1 for Rutgers Data Science Bootcamp

### [See Full Project Presentation Here!](https://docs.google.com/presentation/d/1eVjDKqgjQVe1cIoBrewCYrsibdxyrrMSaR-AypFru4M/edit#slide=id.ga4a3d46c77_0_274)

# Team Members

* [Ben Kramskoi](https://github.com/kramskb1)
* [Chloe Veras](https://github.com/cveras33)
* [Jennifer Dean](https://github.com/Jen-Dean) 
* [Jordan Chatman](https://github.com/JordanChat)
* [Saroja Shreenivasan](https://github.com/Shreeniv)

# Data Sources & APIs

### [Spotify Web API](https://developer.spotify.com/documentation/web-api/)

##### Questions to answer:

1. How music changed over time? 
  * Danceability, energy, liveliness, etc
  
2. Genre popularity over the course of history

3. Are there areas in the world where Spotify is less available than others?
 
  *Note: Spotify was founded in April 23, 2006*


## Supplementary Data Sources

#### [Kaggle](https://www.kaggle.com/leonardopena/top-spotify-songs-from-20102019-by-year)

#### [Spotipy](https://github.com/plamere/spotipy)

#### [ISO.org](https://www.iso.org/obp/ui/#search)

#### [jupyter-gmaps](jupyter-gmaps.readthedocs.io)

#### [Google Maps API](https://developers.google.com/places/web-service/overview)

#### [Google Maps Public Data](https://developers.google.com/public-data/docs/canonical/countries_csv)

## Song Attributes Definitions

[(View on Spotify Documentation)](https://developer.spotify.com/documentation/web-api/reference/object-model/#audio-features-object)

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

# Findings

## Attribute Correlations

![attribute correlation](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/Attribute_correlation.png)

* Attributes with “HOT” colors have a high correlation
* Attributes with “COLD” colors have a lower correlation
* Attributes with high correlation:
  * bpm : Energy
  * Energy : Loudness
  * liveness : bpm
  * Valence : Loudness

## Attributes over time

![trends over time](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/trends_by_year.png)

* Over the years, there has been relatively flat levels of song attributes over time.
* “BPM” is slightly trending DOWN
* “Energy” is slightly trending DOWN
* “Liveness” is slightly trending DOWN
* “Valence” is slightly trending DOWN
* “Dance” is slightly trending UPWARDS
* “Acousticness” is slightly trending UPWARDS
* “Loudness” is very flat.

## Music Availability

![Spotify Music Availability](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Country_Availability/Music_Availability.png)
![Availabilty pie chart](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Country_Availability/Available%20Music%20Per%20Country%20Pie%20Chart.png)


* The data implies heavily that Spotify is currently available to 1st world, highly developed countries, and avoids more economically poor third world countries.   
* Despite a very large user base (300 million users) - Their market reaches only 37% of countries available.
* Almost 63% of the world (in countries, not population) have access to Spotify.  And almost full continents (Africa) have almost no access.
* The next steps are to discover what the implications are… is this due to GDP wealth?  Or population density? What about political/ government types? Cultural differences?
* What would the implications be on Spotify’s user growth/ revenue if they could break into more countries - like China?

## Attribute Breakdown by Decade

![BPM](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/bpm_scatter_plot.png)

![Loudness](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/dB_scatter_plot.png)

![Danceability](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/danceability_scatter_plot.png)

![Valence](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Attribute_Trends/val_scatter_plot.png)


## Top Genres by Decade

![Top Genres Over the Decade](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Genre_Trends/genre_by_year.png)
![Top Genres Over the Decade Bar Plot](https://github.com/cveras33/project-1-group-6/blob/main/Output%20Data/Genre_Trends/Top_Genre_by_Year%20bar_plot.png)

* dance-pop has been the most popular genre from 2010 until 2018. In 2019 pop is more popular than dance-pop
* Every single year some form of “pop” dominates the top genre charts. 
* Popular non-pop genres include: Big Room, Neo Mellow, British Soul, Permanent Wave, Canadian R&B, EDM
* The implication of our findings is that pop, along with “loudness/ danceability/ valence” attributes.  Fast, happy “pop-y” songs have been dominant throughout the decade.   The masses really love pop!
* Is there a correlation to the availability of the music (mostly 1st world countries?) If Spotify expanded to other countries and cultures, would there be a genre shift?  

# Data & Python Code

## Resources & CSVs

#### [Top Songs Over the Decade](https://github.com/cveras33/project-1-group-6/blob/main/Resources/cleaned_data.csv)

 *Pulled from Kaggle*
 
#### [Iso Country Codes](https://github.com/cveras33/project-1-group-6/blob/main/Resources/ISO_Country_Codes.csv)

*Pulled from ISO.org*

#### [Country Latitude and Longitudes](https://github.com/cveras33/project-1-group-6/blob/main/Resources/Country_Lat_Long.csv)

*Pulled from Google Maps Developer Sources*

## Python Code

#### [Spotify Token Authorization Generation](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/0_Base_Auth.ipynb)

#### [Code to Pull Album Data from Spotify's New Releases](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/1_New_Releases_Pull.ipynb)

#### [Generating the Song Attribute Trends Over the Decade](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/3_Song_Trends_Over_The_Decade.ipynb)

#### [Generating Song Attributes per Year](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/5_Decade_Attribute_Breakdown.ipynb)

#### [Generating the Top Genres per Individual Year](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/4_Top_Genres_per_Decade.ipynb)

#### [Generating the Top Genres Over the whole Decade](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/6_top_genre_by_year.ipynb)

#### [Generating Country Availability](https://github.com/cveras33/project-1-group-6/blob/main/Python%20Files/2_Country_Data_Availability.ipynb)


# Thank You!
