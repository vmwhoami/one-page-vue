<template>
  <div id="app">  
    <main-page/>    
  </div>
</template>

<script>
import MainPage from './pages/MainPage.vue'
 

export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>
@font-face {
  font-family: "FjallaOne";
  src: local("fonts"),
   url(./assets/fonts/FjallaOne-Regular.ttf) format("truetype");
}
</style>