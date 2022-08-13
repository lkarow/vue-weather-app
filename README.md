# VUE Weather App

## Description

A weather app created with VUE that lets the user search for a city and then displays the current weather and temperature. There is also a forecast for 24 and 48 hours. Depending on the current weather, the background image changes to show the weather. The app retrieves the weather data through a backend that handles the calls to the [OpenWeather API](https://openweathermap.org/api), or you can set it up to retrieve data directly from the OpenWeather API.

Preview:

<image src="./public/normal.png" width="400px">
<image src="./public/hot.png" width="400px">

## Set up for direct calls to the OpenWeather API

To use the OpenWeather API, you must obtain an API key. You can sign up [here](https://home.openweathermap.org/users/sign_up). Once you have a key, create an environment variable called VUE_APP_API_KEY with your API key.

Then update the following lines in WeatherView:

```
api_key: process.env.VUE_APP_API_KEY,
url_base: 'https://api.openweathermap.org/data/2.5/',
```

Also update the fetchWeather method accordingly.

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Lints and fixes files

```
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
