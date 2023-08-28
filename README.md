# Movie App

https://composer0.github.io/Movie-App/

The "Movie App" script allows users to discover and search for movies using The Movie Database (TMDb) API. This documentation outlines the script's components, functions, and their roles in fetching and displaying movie information.

### Script Components

1. **API URLs**
   - `API_URL`: The URL for retrieving a list of popular movies from TMDb API.
   - `IMG_PATH`: The base URL for retrieving movie poster images.
   - `SEARCH_API`: The URL for searching movies based on user input.

2. **HTML Elements**
   - `main`: The main container element where movie information is displayed.
   - `form`: The form element for submitting search queries.
   - `search`: The input element where users can enter search terms.

3. **Functions**
   - `getMovies(url)`: Fetches movie data from the provided URL and displays the movies using the `showMovies` function.
   - `showMovies(movies)`: Displays a list of movies in the `main` container by creating HTML elements for each movie.
   - `getClassByRate(vote)`: Returns a CSS class based on the movie's vote average, determining if it's 'green', 'orange', or 'red'.

### Fetching and Displaying Movies

The `getMovies` function fetches movie data from TMDb API using the provided URL and displays the movies using the `showMovies` function. The `showMovies` function creates HTML elements for each movie and populates them with relevant information like title, poster image, vote average, and overview.

### Movie Rating Classes

The `getClassByRate` function returns a CSS class based on the movie's vote average. It helps style the vote average based on its value, allowing ratings to be color-coded as 'green' for high ratings, 'orange' for moderate ratings, and 'red' for low ratings.

### User Interaction

The script handles user interaction through the following event listeners:

- `form.addEventListener('submit', (e) => {...})`: Listens for form submissions to trigger movie searches. If a search term is entered, it fetches and displays movies based on the search term. If the search term is empty, the page is reloaded.

### Conclusion

The "Movie App" script demonstrates how to interact with the TMDb API to fetch and display movie data based on user preferences and search queries. Developers can customize and extend this script to create their own movie discovery applications, integrating additional features and styling to enhance the user experience.
