<template>
  <button class="btn button" @click.prevent="prevNext" />
</template>


<script>
export default {
  name: "SlideButton",

  props: {
    direction: {
      type: String,
      default: "left",
    },
  },

  data() {
    return {};
  },
  computed: {},
  methods: {
    prevNext() {
      this.$emit("prevNext", this.direction);
    },
  },
};
</script>


<style scoped>
.button {
  background-image: url(../assets/images/arrow.jpg);
  width: 60px;
  height: 80px;
  background-size: cover;
}
</style>
