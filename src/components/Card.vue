<template>
  <div class="card">
    <img :src="image" :alt="title" class="card-image" />
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
.card {
  border: 1px solid #ddd;
  border-radius: 5px;
  padding: 20px;
  width: 300px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin: 10px;
  text-align: center;
}
.card-image {
  width: 100%;
  height: auto;
  border-radius: 5px;
}
.card h3 {
  margin-top: 10px;
}
</style>
