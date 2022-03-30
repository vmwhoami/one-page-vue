<template>
  <section class="my-3">
    <b-container class="conainer">
      <h1 class="pb-2">
        Learn More
      </h1>
      <p>
        Find out the risk to your users from today’s biggest cyber threats in
        our eighth annual State of the Phish report.
      </p>
    </b-container>
  </section>
</template>


<script>
export default {
  name: "LearnMore",

  props: {},

  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
.conainer {
  min-height: 460px;
  background-image: url(../assets/images/learnMore.jpg);
  background-repeat: no-repeat;
  /* transform: scaleX(-1); */
  object-fit: cover;
  background-color: #0097d8;
}

  h1 {
    color: white;
    max-width: 500px;
  }

p {
  color: white;
  font-size: 18px;
  max-width: 420px;
}
</style>
