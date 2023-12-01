<template>
  <div id="app">
    <router-view />
    <SsrDemo />
  </div>
</template>

<script>
import SsrDemo from './components/SsrDemo.vue';

export default {
  components: {
    SsrDemo,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  font-size: 2em;
  margin-bottom: 20px;
}

p {
  font-size: 1.5em;
  color: #42b983;
}
</style>
