<template>
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

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  min-height: 100vh;
}
</style>
