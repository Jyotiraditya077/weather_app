# Weather App

## Description
This is a simple Weather App built using HTML, CSS, and JavaScript. It fetches real-time weather data from a weather API and displays key weather details for a specified location.

## Features
- Search for weather details by city name
- Display current temperature, humidity, wind speed, and weather conditions
- Dynamic weather icons based on conditions
- Responsive design for various screen sizes

## Technologies Used
- HTML
- CSS
- JavaScript
- Weather API

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/weather-app.git
   ```
2. Navigate to the project folder:
   ```bash
   cd weather-app
   ```
3. Open `index.html` in a browser.
4. Enter a city name in the search box and press Enter.
5. View the weather details for the entered location.

## API Used
This app fetches data from a weather API. You may need to obtain an API key from a weather service provider (e.g., OpenWeatherMap, WeatherAPI) and configure it in your JavaScript file.

## Setup API Key
1. Sign up on a weather API provider's website and get an API key.
2. Locate the JavaScript file (`script.js`).
3. Replace `YOUR_API_KEY` with your actual API key in the API request URL.

## Example Code for Fetching Weather Data
```javascript
const apiKey = 'YOUR_API_KEY';
const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=London&appid=${apiKey}&units=metric`;

fetch(apiUrl)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error fetching weather data:', error));
```

## Future Improvements
- Add a feature to fetch weather based on the user's location.
- Improve UI with animations and better styling.
- Show a 5-day weather forecast.

## Author
- **Jyotiradiya Swain** - Developer

## License
This project is licensed under the Apache License.

