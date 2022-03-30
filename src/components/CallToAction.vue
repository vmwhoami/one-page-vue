<template>
  <section class="my-3">
    <b-container class="container d-flex align-items-center">
      <div class="d-flex flex-column p-5">
        <h1 class="pb-2">Start Training Your Everyday Cybersecurity Heroes</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer bibendum porttitor purus et sollicitudin.
        </p>
      </div>
    </b-container>
  </section>
</template>


<script>
export default {
  name: "CallToAction",

  props: {},

  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
.container {
  min-height: 460px;
  position: relative;
 

  background-color: rgba(0, 0, 0, 0.5);
}

.container::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url(../assets/images/fatherDaughter.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  z-index: -1;
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
