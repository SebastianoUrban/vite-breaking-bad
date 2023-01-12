<template>
  <div>
    <select v-model="selected">
      <option v-for = "type in archetypes" :value="type">  
        {{ type }} 
      </option>
    </select>
  </div>
</template>

<script>

  export default {
    data() {
      return {
        archetypes : ['Alien', 'Laval', 'Vylon', 'Inzektor', 'Umi', 'Gusto'],
        selected : ''
      }
    },
    methods: {

    },
    created () {
    },
    components : {
    }
  }
</script>

<style lang="scss" >

  
</style>