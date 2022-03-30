<template>
  <section class="my-3">
    <b-container
      class="container d-flex align-items-center justify-content-end">
      <div class="d-flex flex-column p-5">
        <h1 class="pb-2">Learn More</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
          bibendum porttitor purus et sollicitudin.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
          bibendum porttitor purus et sollicitudin.
        </p>
      </div>
    </b-container>
  </section>
</template>


<script>
export default {
  name: "LearnMore", 
};
</script>


<style scoped>
.container {
  min-height: 460px;
  position: relative;
  background-image: url(../assets/images/learnMore.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

h1 {
  color: white;
  max-width: 500px;
}

p {
  color: white;
  font-size: 16px;
  max-width: 420px;
}
</style>
