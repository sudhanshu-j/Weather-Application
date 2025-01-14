# Weather Application 🌦️☀️🌧️

Welcome to the **Weather Application**! This is a modern, interactive web app that allows users to get the **current weather** and a **5-day forecast** for any city in the world 🌍. Users can search for weather data by typing a city name or using their **current location** for personalized weather updates. 🌤️📍

---

## Features ✨

- **🌞 Current Weather**: See the current temperature, wind speed, humidity, and weather description for your chosen city.

- **📅 5-Day Forecast**: Get a 5-day weather forecast with temperature, wind speed, and humidity for each day.

- **🔍 City Search**: Search weather by entering a city name 🌆 (e.g., New York, Tokyo, Paris).

- **📡 Geolocation Support**: Fetch weather based on your **current location** using geolocation 🌍.

- **📱 Mobile Friendly**: Fully responsive design that works great on both desktop and mobile devices 📱💻.

- **🔄 Auto Refresh**: Automatically refreshes weather data based on user actions.

---

<!-- ## Screenshots 📸

![Weather App Screenshot](./images/screenshot.png) -->

## How It Works ⚙️

This application fetches real-time weather data from the **OpenWeatherMap API** to provide the current weather and a 5-day forecast. Here's a breakdown of how it works:

### HTML 📝

- The `index.html` file defines the structure of the webpage. It includes:
  
  - A **header** with the app name and icon.
  
  - An **input field** where users can type the name of a city.
  
  - A **search button** to submit the city name for weather information.
  
  - A **location button** to fetch weather based on the user's current location.
  
  - Sections for displaying **current weather** and the **5-day forecast**.

### CSS 🎨

- The `style.css` file provides styling for the weather app, including:
  
  - A visually appealing **background image** and **color scheme**.
  
  - Styling for the **weather input fields**, **buttons**, and **forecast cards**.
  
  - **Responsive design** using media queries to ensure the app looks good on all screen sizes, from desktop to mobile.
  
  - Custom font styling using **Google Fonts** for a modern, clean look.

### JavaScript ⚡

- The `script.js` file powers the interactivity of the app:
  
  - **Fetching Weather Data**: It retrieves data from the OpenWeatherMap API using the city name or geolocation coordinates.
  
  - **Dynamic Content Update**: The weather data is dynamically injected into the page, creating weather cards for the current weather and the 5-day forecast.
  
  - **Geolocation**: It uses the browser’s **geolocation API** to get the user's current location and show the weather for that location.
  
  - **Error Handling**: In case of an error (e.g., no city found, or permission denied for geolocation), appropriate error messages are displayed to the user.

---

## Getting Started 🚀

### Prerequisites 📋

Before you get started, make sure you have the following:

- A modern web browser (Chrome, Firefox, Safari, Edge, etc.).

- An internet connection to fetch weather data from the OpenWeatherMap API 🌐.

### Installation 📥

1. **Clone this repository** to your local machine:
    ```bash
    git clone https://github.com/yourusername/weather-app.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd weather-app
    ```
3. Open the `index.html` file in your preferred web browser to start using the app. 🎉

### API Key 🔑

This app uses **OpenWeatherMap** API to fetch weather data. You will need your own **API key**. Here's how you can get one:

1. Go to [OpenWeatherMap API](https://openweathermap.org/api) and sign up for a free account.

2. Generate a new API key and copy it.

3. Replace the `YOUR_API_KEY` placeholder in the `script.js` file with your API key:
   
   ```javascript
   const API_KEY = "YOUR_API_KEY"; 
   ```

### Example of API URL 📡:

The app makes requests to the OpenWeatherMap API to fetch weather data based on the city name or geolocation coordinates

   ```plaintext
   https://api.openweathermap.org/data/2.5/forecast?lat={latitude}&lon={longitude}&appid={API_KEY}
   ```

---

## File Structure 📂

```bash
/weather-app
  ├── index.html         # The structure of the webpage
  ├── style.css          # The styles for the webpage
  ├── script.js          # JavaScript logic for fetching and displaying weather data
  ├── /images            # Folder containing background and icon images
  └── README.md          # This file
```

---

## How It Works Under the Hood 🔧

### 1. Weather Data Fetching 🌦️

- **City-based search**: When a user types in a city name and presses the search button, the app sends a request to the **OpenWeatherMap geolocation API** to fetch the coordinates (latitude & longitude) of the city.

- **Weather details**: Using these coordinates, the app fetches weather data for that city from the **OpenWeatherMap weather API** and displays the results (temperature, humidity, wind speed, and weather description).

### 2. Geolocation 🌍

- The app can also fetch weather data based on the user’s current location. When the "Use Current Location" button is clicked, the app uses the **geolocation API** to get the user’s coordinates and then fetches weather data using those coordinates.

### 3. Dynamic Weather Cards 📅

- The current weather and 5-day forecast are displayed in separate sections. The data for each day in the 5-day forecast is displayed in a **card format**, with a visual icon representing the weather condition (e.g., clear sky, rain, clouds).

### 4. Error Handling ⚠️

- The app gracefully handles errors, such as incorrect city names or location permission denials, by showing appropriate alerts to the user.

## Contributing 🤝

We welcome contributions to improve this project! Here's how you can contribute:

1. **Fork** this repository to your GitHub account.

2. **Clone** the repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/weather-app.git
    ```

3. **Create** a new branch for your feature:
    ```bash
    git checkout -b feature-branch
    ```

4. **Make** your changes and **commit** them:
    ```bash
    git commit -m 'Add new feature or fix bug'
    ```

5. **Push** your changes to your forked repository:
    ```bash
    git push origin feature-branch
    ```

6. **Open** a pull request from your fork to the main repository.

We will review your changes and merge them if everything looks good! 🎉

---

## Acknowledgements 🙏

- Thanks to **OpenWeatherMap** for providing the weather data API 🌦️.

- Special thanks to **Google Fonts** for providing the beautiful font (**Roboto Condensed**) used in this app.

- Thanks to **FontAwesome** for the weather-related icons used in the UI 🌐.

---

Enjoy using the **Weather Application** and stay updated on the weather wherever you are! 🎉🌈
