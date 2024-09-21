# Movie App README

## Introduction

This project is a simple web-based movie search application that allows users to search for movies by title using the [TMDb (The Movie Database) API](https://www.themoviedb.org/documentation/api). Users can input a movie title, and the app fetches the movie details from TMDb and displays the results dynamically.

## Features

- **Movie Search**: Users can search for any movie by entering the title in the search bar.
- **Dynamic Content**: The app fetches and displays movie details such as titles, images, and descriptions using TMDb API.
- **Responsive Design**: The app is designed to work on both desktop and mobile devices.

## Files Overview

### 1. `index.html`
This is the main HTML file that contains the structure of the web page, including the form where users can enter the movie title and the section where movie results are displayed.

### 2. `style.css`
This is the CSS file that defines the styling for the app. It makes the app visually appealing and responsive to different screen sizes.

### 3. `script.js`
This is the JavaScript file that contains the logic for interacting with the TMDb API. It handles form submission, sends requests to the API, and dynamically updates the DOM with the movie data.

## Getting Started

### Prerequisites
1. **API Key**: You need a TMDb API key to make requests. Sign up on the [TMDb website](https://www.themoviedb.org/signup) to obtain your key.

### Steps
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Codewithhaider29/movie-app.git
   ```

2. **Add API Key**: 
   In the `script.js` file, replace the placeholder with your actual TMDb API key.

3. **Run the app**: Open `index.html` in your browser. You can now search for movies using the input field.

### Example

1. Enter the movie title in the search field.
2. Press the **Search** button to get the results.
3. The app will dynamically display movie details like poster, title, and description in the main section of the page.

## API Information

The app uses the TMDb API to fetch movie data based on the user's search input.

- **Base URL**: `https://api.themoviedb.org/3`
- **Endpoint**: `/search/movie`
- **Query Parameters**:
  - `api_key`: Your unique TMDb API key
  - `query`: The movie title entered by the user

For example, to search for "Inception":
```
https://api.themoviedb.org/3/search/movie?api_key=YOUR_API_KEY&query=Inception
```

## Project Structure

```
movie-app/
├── index.html   # Main HTML file
├── style.css    # CSS styles for the app
└── script.js    # JavaScript logic to interact with the TMDb API
```

## Dependencies

- **TMDb API**: The app relies on the TMDb API for fetching movie data.
- **Basic HTML, CSS, and JavaScript**: The app uses vanilla JavaScript, so there are no external libraries or frameworks required.

## Known Issues

- **Search Limitations**: The search is limited to what TMDb offers, which might result in no data for obscure or new movies.

## Future Enhancements

- **Display Additional Details**: Add more information like movie ratings, release dates, etc.
- **Loading Indicator**: Show a loading spinner while fetching data from the API.
- **Error Handling**: Improve error handling for empty searches or failed API requests.

## License

This project is open-source and available under the [MIT License]
