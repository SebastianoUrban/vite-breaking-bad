<template>
  <div class="wrapper">
    <div>
      <MainSearch/>
    </div>
    <div>
      <MainCards />
    </div>
  </div>
</template>

<script>
  import MainCards from './MainCards.vue';
  import MainSearch from './MainSearch.vue';

  export default {
    data() {
      return {
      }
    },
    methods: {
    },
    components : {
      MainCards,
      MainSearch
    }
  }
</script>

<style lang="scss" >

  
</style>