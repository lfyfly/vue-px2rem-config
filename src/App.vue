<template>
  <div id="app">
    <img class="logo" src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
html {
  font-size: calc(100vw / 3.75);
}
.logo {
  width: 100px;
  display: block;
  margin: 0 auto;
}
#app {
}
</style>
