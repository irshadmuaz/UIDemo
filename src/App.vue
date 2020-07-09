<template>
  <div id="app">
    <h2 class="title">PELOTON</h2>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
body {
  padding: 0;
  width: 1300px;
  margin: 0 auto;
}
.title {
  padding: 20px;
  margin: 0;
  text-align: left;
  background-color:black;
  color: snow;
}
</style>
