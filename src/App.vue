<template>
  <WeatherView />
</template>

<script>
import WeatherView from './components/WeatherView.vue';

export default {
  components: {
    WeatherView,
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
</style>
