<template>
  <b-container fluid>
    <top-nav />
    <main-header />
    <under-header/>
    <carousel :slides="slides"/>
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
    return {
      slides: [
        {
          title: "table of contents",
          alt: "table of contents",
          img1: "../assets/images/tableOfContents.jpg",
          img2: "../assets/images/yearOfNewNormal.jpg"
        }
      ]
    };
  },
  methods: {},
};
</script>

 <style>
#app .container-fluid {
  padding: 0;
}
</style>