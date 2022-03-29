<template>
  <header class="w-100 p-3">
    <h2>Main header</h2>
  </header>
</template>


<script>
export default {
  name: "MainHeader",

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
