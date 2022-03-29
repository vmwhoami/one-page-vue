<template>
  <section fluid class="bg-blue">
    <div class="container pb-4">
      <h3 class="py-3">In this report</h3>
      <div class="row">
        <div class="col">
          <p>The impact of socially engineered attacks</p>
        </div>
        <div class="col">
          <p>Behaviours that could be putting you at risk</p>
        </div>
        <div class="col">
          <p>Tips to make your defences more effective</p>
        </div>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  name: "UnderHeader",

  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
h3 {
  color: white;
  font-weight: 200;
  font-size: 18px;
  font-family: "Roboto-Regula";
  text-transform: uppercase;
  letter-spacing: 5px;
}

p {
  color: white;
  font-weight: 200;
  font-size: 16px;
  max-width: 320px;
  line-height: 20px;
  letter-spacing: 1px;
}

.col:not(:last-child) {
  border-right: 2px solid rgba(255, 255, 255, 0.2);
}

.bg-blue {
  background-color: #0097d8;
}
</style>
