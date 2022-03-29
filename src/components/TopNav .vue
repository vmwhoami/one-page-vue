<template>
  <b-nav class="w-100 p-3">
    <b-container fluid="xxl">
      <h2>Navigation</h2>
        <a href="index.html">
          proofpoint
        </a>
        <b-button squared>Contact Us</b-button>
    </b-container>
  </b-nav>
</template>


<script>
export default {
  name: "TopNav",

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


<style scoped>
.bg-red {
  background-color: red;
}
</style>
