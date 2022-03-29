<template>
  <section class="my-3">
    <b-container class="d-flex justify-content-between align-items-center canvas">
      <div class="images-container">
        
      </div>
      <slide-button class="left" direction="left" />
      <slide-button class="right" direction="right" />
    </b-container>
  </section>
</template>


<script>
import SlideButton from "./SlideButton.vue";
export default {
  name: "UnderHeader",

  components: {
    SlideButton,
  },

  props: {
    slides: {
      type: Array,
      default: () => []
    },
  },

  data() {
    return {

    };
  },
  methods: {},
};
</script>


<style scoped>
.left {
  position: absolute;
  left: 10px;
  transform: scaleX(-1);
}

.right {
  position: absolute;
  right: 10px;
  transform: scaleX(1);
}

.canvas {
  background-color: #3b3b3b;
  min-height: 600px;
  position: relative;
}
</style>
