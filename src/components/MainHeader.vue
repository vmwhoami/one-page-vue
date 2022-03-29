<template>
  <header fluid class="bg-blue">
    <b-container class="header-bg d-flex flex-column justify-content-center">
      <h1>Everyone gets phishing emails. Not everyone falls for them.</h1>
      <p>
        Find out the risk to your users from today’s biggest cyber threats in
        our eighth annual State of the Phish report.
      </p>
    </b-container>
  </header>
</template>


<script>
export default {
  name: "MainHeader",

  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
  h1 {
    color: white;
    max-width: 500px;
  }

p {
  color: white;
  font-size: 18px;
  max-width: 500px;
}

.bg-blue {
  background-image: url(../assets/images/learnMore.jpg);
  background-position-y: 86px;
  background-repeat: no-repeat;
  object-fit: cover;
  background-color: #0097d8;
}

.header-bg {
  padding-top: 90px;
  min-height: 600px;
}
</style>
