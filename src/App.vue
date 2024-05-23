<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <div class="card-container">
      <Card title="Espresso" description="Rich and creamy espresso." image="https://i.pinimg.com/564x/dd/0e/78/dd0e7878169954d00dace05d841265ad.jpg" />
      <Card title="Latte" description="Smooth and velvety latte." image="https://i.pinimg.com/474x/55/f8/7b/55f87b082c2e6f655957e29725e8a0d8.jpg" />
      <Card title="Cappuccino" description="Perfectly balanced cappuccino." image="https://i.pinimg.com/564x/49/97/fb/4997fb5e0d05d54d66bee115f6ba8616.jpg" />
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import Card from './components/Card.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    Card,
    Footer
  }
};
</script>

<style>
.card-container {
  display: flex;
  justify-content: space-around;
  margin: 20px;
  flex-wrap: wrap;
}
</style>
