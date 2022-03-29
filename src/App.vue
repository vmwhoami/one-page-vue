<template>
  <div id="app">
    <main-page />
  </div>
</template>

<script>
import MainPage from "./pages/MainPage.vue";

export default {
  name: "App",
  components: {
    MainPage,
  },
};
</script>

<style>
@font-face {
  font-family: "FjallaOne";
  src: local("assets/fonts"),
    url(./assets/fonts/FjallaOne-Regular.ttf) format("truetype");
}
@font-face {
  font-family: "Roboto-Regula";
  src: local("assets/fonts"),
    url(./assets/fonts/Roboto-Regular.ttf) format("truetype");
}
  h1 {
    font-family: "FjallaOne";
  }

  p {
    font-family: "Roboto-Regula";
  }

 
</style>