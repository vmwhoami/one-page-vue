<template>
  <b-container fluid>
    <top-nav />
    <main-header />
    <under-header/>
    <carousel/>
  </b-container>
</template>

<script>
import TopNav from "../components/TopNav .vue";
import MainHeader from "../components/MainHeader.vue";
import UnderHeader from "../components/UnderHeader.vue";
import Carousel from "../components/Carousel.vue"

export default {
  name: "MainPage",

  components: {
    TopNav,
    MainHeader,
    UnderHeader,
    Carousel
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

 <style>
#app .container-fluid {
  padding: 0;
}
</style>