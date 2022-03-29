<template>
  <b-container fluid="xl">
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

    return {
      dismissSecs: 10,
      dismissCountDown: 0,
      showDismissibleAlert: false,
    };
  },
  methods: {
    countDownChanged(dismissCountDown) {
      this.dismissCountDown = dismissCountDown;
    },
    showAlert() {
      this.dismissCountDown = this.dismissSecs;
    },
  },
};
</script>

 