# WebD_Assignment10

Weather App
This is a simple weather app that displays the current weather and hourly forecast for a given city.
This is a weather application built using React. The application allows the user to search for a city and display the current weather conditions, as well as a five-day forecast for that city.

The code includes multiple components, including a search bar component, a current weather component, a daily weather component, and an hourly weather component. The application also utilizes third-party libraries such as Moment.js for time and date formatting.

The application fetches weather data from an external API and passes that data as props to the various components. The components then render the data in a user-friendly way.

In summary, this is a weather application built using React, which allows users to search for a city and view current weather conditions as well as daily and hourly forecasts

Dependencies
This project requires the following dependencies:

React
React Router DOM
Axios
Moment
File Structure
The file structure for this project is as follows:

java
Copy code
weather-app/
  README.md
  node_modules/
  package.json
  public/
    index.html
    favicon.ico
  src/
    App.js
    WeatherData.js
    Hourly.js
    HourlyCityForecast.js
    HourlyForecast.js
    index.css
    index.js

App.js
This file contains the main component for the weather app. It uses the useState hook to manage state for the search input and the weather data. It also uses the useEffect hook to fetch weather data from the OpenWeatherMap API when the app is loaded or the search button is clicked. The WeatherData component is rendered to display the current weather data.

WeatherData.js
This file contains the component that displays the current weather data for a city. It receives the weather data as props and uses Moment.js to format the date. It also uses the Link component from React Router DOM to navigate to the hourly forecast page.

Hourly.js
This file contains the component that displays the hourly forecast for a given day. It receives the complete weather data for the city as props from the previous page and uses the useState hook to manage state for the filtered weather data. It also uses the useEffect hook to filter the weather data based on the selected day from the URL parameters. The HourlyCityForecast component is rendered to display the hourly weather data.

HourlyCityForecast.js
This file contains the component that displays the hourly weather data for a city. It receives the hourly weather data as props and uses Moment.js to format the date.

index.css
This file contains the styles for the weather app.

index.js
This file contains the code that renders the main App component to the DOM.