<template>
  <h1>Weather App</h1>
  <WeatherView />
  <FooterView />
</template>

<script>
import WeatherView from './components/WeatherView.vue';
import FooterView from './components/FooterView.vue';

export default {
  name: 'App',
  components: {
    WeatherView,
    FooterView,
  },
  data() {
    return {};
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

:root {
  --text-color: rgb(33, 33, 33);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  margin: 0 auto;
  display: flex;
  flex-flow: column;
  height: 100%;
  min-height: 100vh;
  font-family: 'montserrat', sans-serif;
  background-image: url('./assets/bg.jpg');
  background-size: cover;
  background-position: center;
  transition: background-image 0.4s;
}

#app.hot {
  background-image: url('./assets/hot.jpg');
}

#app.rain {
  background-image: url('./assets/rain.jpg');
}

#app.snow {
  background-image: url('./assets/snow.jpg');
}

h1 {
  color: var(--text-color);
  font-size: 40px;
  font-weight: 700;
  text-align: center;
  margin: 20px;
}
</style>
