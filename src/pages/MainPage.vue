<template>
  <b-container fluid>
    <top-nav />
    <main-header />
  </b-container>
</template>

<script>
import TopNav from "../components/TopNav .vue";
import MainHeader from "../components/MainHeader.vue";

export default {
  name: "MainPage",

  components: {
    TopNav,
    MainHeader,
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