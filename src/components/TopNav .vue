<template>
  <b-nav class="px-5 py-4 nav-container">
    <b-container class="d-flex justify-content-between align-items-center">
      <a href="#">
        <img class="logo-img" src="../assets/images/proofpoint.png" />
      </a>
      <b-button squared class="red-bg">Contact Us</b-button>
    </b-container>
  </b-nav>
</template>


<script>
export default {
  name: "TopNav",
  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
.nav-container {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1;
  width: 100%;
  background-color: white;
  box-shadow: 0 3px 7px 0 rgba(0, 0, 0, 0.17);

}
.red-bg {
  background-color: #ee3124;
  border: none;
}
</style>
