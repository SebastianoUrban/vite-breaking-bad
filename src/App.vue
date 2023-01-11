<script setup>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
</script>

<template>
    <header class="d-flex justify-content-center align-items-center">
      <AppHeader/>
    </header>

    <main class="d-flex justify-content-center align-items-center">
      <AppMain/>
    </main>

</template>

<style lang="scss">
  @import "/node_modules/bootstrap/scss/bootstrap";

  .wrapper {
    width: 80%;
  }
</style>