<template>
  <div id="app">
    <img class="logo" src="./assets/logo.png">
    <router-view/>

    <van-tabbar v-model="active">
      <van-tabbar-item icon="shop">标签</van-tabbar-item>
      <van-tabbar-item icon="chat" dot>标签</van-tabbar-item>
      <van-tabbar-item icon="records" info="5">标签</van-tabbar-item>
      <van-tabbar-item icon="gold-coin" info="20">标签</van-tabbar-item>
    </van-tabbar>
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
