<template>
  <b-container fluid class="mt-3 footer">
    <b-nav class="px-5 py-4">
      <b-container class="d-flex align-items-center">
        <a href="#">
          <img class="logo-img" src="../assets/images/proofpoint.png" />
        </a>
      </b-container>
    </b-nav>
  </b-container>
</template>


<script>
export default {
  name: "MainFooter",
  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
.footer {
  width: 100%;
  background-color: #10181c;
  box-shadow: 0 3px 7px 0 rgba(0, 0, 0, 0.17);
}
.footer img {
  filter: brightness(0) invert(1);
}
</style>
