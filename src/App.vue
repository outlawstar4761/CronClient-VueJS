<template>
  <div id="app">
    <NavBar v-if="$store.state.isAuthenticated"></NavBar>
    <router-view></router-view>
  </div>
</template>

<script>

import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
  }
}
</script>

<style>
/* @import'~bootstrap/dist/css/bootstrap.css'; */
@import '/node_modules/bootstrap/dist/css/bootstrap.css';
@import './assets/styles/style.css';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}

</style>
