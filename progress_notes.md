# Current Tasks

### Jen 
- Pull ISO Country Code & Create a .CSV & Dataframes based on country (done)
- Create Python Code to pull Genre Popularity Based on Country
- Alter code to be able to find the same data based on country & year

### Jordan 
- Find the top 10,000 songs played per year Spotify has data (since 2006)

### Ben 
- Find the top 10 Genres played per year Spotify has data (since 2006)

### Chloe 
- Setting up base class to get spotify authorization to retrieve API access code 
  - Base class will allow easy regeneration of access code (possibly even regenerate on its own after expiration)
  
### Saroja
- 


# Finding the Popularity by Country 
###### See Jen for more information:

### Initial Problems:

* Spotify API does NOT let you “browse by popularity”
* Spotify API does NOT let you “browse by Genre”
* Spotify API does NOT let you “browse by country”

### Outline of solution??

1. Use [BROWSE API](https://developer.spotify.com/documentation/web-api/reference-beta/#category-browse)
  * Get a List of the New Releases (Albums)
  * Collect the [album_IDs] from the new releases
2. Use [ALBUMS API](https://developer.spotify.com/documentation/web-api/reference-beta/#category-albums) - Most Popular Countries
  * Get the [available_markets] (aka countries) and [genres] from the list of [album_IDs]
  * Count the volume of each [available_market] to find the top 50 countries.
  * Run a loop to get the [popularity] of the [album_ID] per top 50 [available_market]
  * Graph the results.
3. Use [ALBUMS API](https://developer.spotify.com/documentation/web-api/reference-beta/#category-albums) - Least Popular Countries
  * Count the volume of each [available_market] to find the bottom 50 countries.
  * Run a loop to get the [popularity] of the [album_ID] per bottom 50 [available_market]
  * Graph the results.
