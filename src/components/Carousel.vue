<template>
  <div class="carousel">
    <div class="carousel-item" v-for="(image, index) in images" :key="index">
      <img :src="image" :alt="'Slide ' + (index + 1)" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Carousel',
  data() {
    return {
      images: [
        'https://i.pinimg.com/474x/97/f7/0e/97f70e1843b41be231746d8fafb03516.jpg',
        'https://i.pinimg.com/474x/06/e3/b3/06e3b3e064f59b6586ac5b13165d753c.jpg'
      ]
    };
  }
};
</script>

<style>
.carousel {
  display: flex;
  overflow-x: scroll;
  scroll-snap-type: x mandatory;
  margin: 20px 0;
}
.carousel-item {
  min-width: 100%;
  display: flex;
  justify-content: center; /* Center the image horizontally */
  scroll-snap-align: center;
}
.carousel-item img {
  max-width: 80%; /* Set maximum width for the image */
  height: auto;   /* Maintain aspect ratio */
}
</style>
