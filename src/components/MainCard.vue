<template>
  <div class="card">
    <img :src="image" alt="" class="card-image-top">
    <div class="card-body">
      <h3 class="card-title">{{ name }}</h3>
      <h5 class="card-text">{{ archetype }}</h5>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
      }
    },
    methods: {
    },
    props : {
      name : String,
      archetype : String,
      image : String
    }
  }
</script>

<style lang="scss" scoped>
  .card {
    width: calc((100% / 5) - 20px);
    h3.card-title {
    font-size: 1rem;
    height: 80%;
    }
    h5.card-text {
    font-size: 0.9rem;
    }
  }

  



</style>