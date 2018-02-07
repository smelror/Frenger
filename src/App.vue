<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
body {
  background: #4776E6;
  background: -webkit-linear-gradient(to right, #8E54E9, #4776E6);
  background: linear-gradient(to right, #8E54E9, #4776E6);
  margin: 0;
}

html {
  height: 100%;
  width: 100%;
}

#app {
  padding: 2vh 5vw;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
