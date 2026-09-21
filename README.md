# 🌦️ Thiranex Intern Weather App

A responsive **Weather Dashboard** developed as part of my **Thiranex Internship**. The application uses JavaScript and a RESTful Weather API to retrieve and display real-time weather information based on the user's city search.

## 📌 Project Overview

The **Thiranex Intern Weather App** allows users to search for a city and view its current weather conditions.

The project was developed to practice:

* Asynchronous JavaScript
* Fetch API
* RESTful APIs
* `async/await`
* JSON data handling
* DOM manipulation
* Event handling
* Error handling
* Responsive web design

## ✨ Features

* 🔍 Search weather by city name
* 🌡️ Display current temperature
* 💧 Display humidity
* 💨 Display wind speed
* ☁️ Dynamic weather icons
* ⚡ Fetch real-time weather data using Fetch API
* 📦 Process JSON API responses
* ❌ Display an error for invalid city names
* 📱 Responsive design for different screen sizes
* ⌨️ Search using the Enter key

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* Fetch API
* RESTful API
* Async/Await
* JSON

## 📂 Project Structure

```text
Thiranex-Intern-Weather-App/
│
├── index.html
├── style.css
├── script.js
│
├── images/
│   ├── search-icon.png
│   ├── cloudy.png
│   ├── sunny.png
│   ├── rainy.png
│   ├── misty.png
│   ├── humidity.png
│   └── wind.png
│
└── README.md
```

## 🌐 API

This project uses the **OpenWeatherMap API** to retrieve current weather data.

The API provides information such as:

* City name
* Temperature
* Humidity
* Wind speed
* Weather condition
* Weather icon

### 🔐 API Key Setup

For security reasons, the API key is **not included in this GitHub repository**.

To run the project locally:

1. Create an account on OpenWeatherMap.
2. Generate an API key.
3. Add your API key to the JavaScript configuration.
4. Do not commit or push your API key to GitHub.

Example:

```javascript
const apiKey = "YOUR_API_KEY";
```

Replace `YOUR_API_KEY` with your own API key locally.

> ⚠️ Never publish your actual API key in a public GitHub repository.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Open the project

Open the project folder in **Visual Studio Code**.

### 3. Add your API key

Add your OpenWeatherMap API key to the JavaScript configuration.

### 4. Run the application

Open `index.html` using **Live Server** or your preferred local development server.

### 5. Search for a city

Enter a city name such as:

```text
Lahore
```

Then click the search button or press **Enter**.

## 🔄 How It Works

The application follows this process:

```text
User enters city
       ↓
Search button / Enter key
       ↓
JavaScript function
       ↓
Fetch API request
       ↓
OpenWeatherMap REST API
       ↓
JSON response
       ↓
Process weather data
       ↓
Update the DOM
       ↓
Display weather information
```

## 📚 JavaScript Concepts Practiced

### Async/Await

The project uses `async` and `await` to handle asynchronous API requests.

```javascript
async function checkWeather(city) {
    const response = await fetch(apiUrl);
    const data = await response.json();
}
```

### Fetch API

The Fetch API is used to request weather data from the REST API.

### JSON Parsing

The API response is converted into a JavaScript object using:

```javascript
const data = await response.json();
```

### Nested JSON Data

Weather information is accessed from nested objects such as:

```javascript
data.main.temp
data.main.humidity
data.wind.speed
data.weather[0].main
```

### DOM Manipulation

JavaScript dynamically updates the HTML elements with the latest weather information.

## ❌ Error Handling

If an invalid city is entered, the application displays:

```text
Invalid city name
```

The weather information is hidden when the requested city cannot be found.

## 📱 Responsive Design

The application is designed to work across:

* Desktop
* Laptop
* Tablet
* Mobile devices

## 🎓 Internship Project

This project was developed as part of my **Thiranex Internship** to strengthen my practical skills in JavaScript, asynchronous programming, RESTful APIs, and frontend web development.

## 👩‍💻 Author

**Aqsa Shahzadi**

### GitHub

Add your GitHub profile/repository link here.

### LinkedIn

Add your LinkedIn profile link here.

---

⭐ If you find this project useful, feel free to explore the repository and give it a star.
