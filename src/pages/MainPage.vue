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
          img1: "tableOfContents.jpg",
          img2: "yearOfNewNormal.jpg"
        },
        {
          title: "some text",
          alt: "some-text",
          img1: "header.jpg",
          img2: "fatherDaughter.jpg"
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