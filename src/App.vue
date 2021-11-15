<template>
  <div id="app">
    <Navbar></Navbar>
    <div class="container">
      <albums-container></albums-container>
    </div>
  </div>
</template>

<script>
import AlbumsContainer from './components/AlbumsContainer.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    AlbumsContainer
  }
}
</script>

<style lang="scss">
@import "@/styles/app";
</style>
