<template>
  <div id="slider">
    <img :src="imgSrc" alt="" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
      images: ["2.jpg", "3.jpg", "4.jpg", "10.jpg"]
    };
  },
  computed: {
    imgSrc() {
      return require(`../assets/${this.images[this.count]}`);
    }
  },
  methods: {
    changeImage() {
      setInterval(() => {
        if (this.count < this.images.length - 1) {
          this.count++;
        } else {
          this.count = 0;
        }
      }, 5000);
    }
  },
  mounted() {
    this.changeImage();
  }
};
</script>

<style scoped>
#slider {
  position: relative;
  top: 10vh;
  width: 100%;
  z-index: 500;

}

img {
  width: 100%;
}
</style>
