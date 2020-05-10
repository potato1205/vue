<!--
 * @Author: your name
 * @Date: 2020-05-05 18:22:11
 * @LastEditTime: 2020-05-10 14:44:57
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /learn-basic/vue-source-code/src/App.vue
 -->
<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <wt-carousel @swiper="swiper">
      <div class="carousel-item">
        <img src="https://ss3.bdstatic.com/iPoZeXSm1A5BphGlnYG/skin/822.jpg" />
      </div>
      <div class="carousel-item">
        <img src="https://ss3.bdstatic.com/iPoZeXSm1A5BphGlnYG/skin/823.jpg" />
      </div>
      <div class="carousel-item">
        <img src="https://ss3.bdstatic.com/iPoZeXSm1A5BphGlnYG/skin/824.jpg" />
      </div>
      <div class="carousel-item">
        <img src="https://ss3.bdstatic.com/iPoZeXSm1A5BphGlnYG/skin/825.jpg" />
      </div>
    </wt-carousel>
    <!-- <Swiper></Swiper> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Form from "./components/form";
import Swiper from "./components/swiper/swiper";

export default {
  name: "App",
  components: {
    // HelloWorld,
    // Form
    'wt-carousel': Swiper
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
