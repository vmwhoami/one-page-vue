<template>
  <section class="my-3">
    <b-container class="d-flex justify-content-between align-items-center canvas">
      <div class="images-container d-flex">
        <img :src="secondImagePath" :alt="imageAlt" />
        <img :src="firstImagePath" :alt="imageAlt" />
      </div>
      <slide-button class="left-btn" direction="left" @prevNext="prevNext" />
      <slide-button class="right-btn" direction="right" @prevNext="prevNext" />
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
      default: () => [],
    },
  },

  data() {
    return {
      index: 0,
    };
  },
  computed: {
    firstImagePath() {
      return require(`@/assets/images/${this.slides[this.index].img1}`)
    },

    secondImagePath() {
      return require(`@/assets/images/${this.slides[this.index].img2}`)
    },

    imageAlt() {
      return this.slides[this.index].alt
    },

  },

  methods: {
    prevNext(direction) {
      if (direction === "left") {
        this.prevPictures();
        }else{
        this.nextPictures();
      }
    },
    nextPictures() {
      this.index+=1;
      if (this.index > this.slides.length - 1) {
        this.index = 0;
      }
    },
    prevPictures() {
      this.index-=1;
      if (this.index < 0) {
        this.index = this.slides.length - 1;
      }
    },
  },
};
</script>


<style scoped>
.left-btn {
  position: absolute;
  left: 10px;
  transform: scaleX(-1);
}

.right-btn {
  position: absolute;
  right: 10px;
  transform: scaleX(1);
}

.canvas {
  background-color: #3b3b3b;
  height: 600px;
  position: relative;
}

.images-container {
  height: 90%;
  width: 90%;
}
.images-container > img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}
</style>
