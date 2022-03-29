<template>
  <section class="my-3">
    <b-container class="d-flex justify-content-between align-items-center canvas">
       <slide-button /> 
    </b-container>
  </section>
</template>


<script>
import SlideButton from './SlideButton.vue';
export default {
  name: "UnderHeader",

  components: {
    SlideButton,
  },

  data() {
    return {};
  },
  methods: {},
};
</script>


<style scoped>
.canvas {
  background-color: #3b3b3b;
  min-height: 600px;
}
</style>
