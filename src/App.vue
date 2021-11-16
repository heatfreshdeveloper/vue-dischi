<template>
  <div id="app">
    <Navbar></Navbar>
    <albums-filter @search="searchAlbums"></albums-filter>
    <div class="container">
      <albums-container></albums-container>
    </div>
  </div>
</template>

<script>
import AlbumsContainer from './components/AlbumsContainer.vue'
import AlbumsFilter from './components/AlbumsFilter.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    AlbumsContainer,
    AlbumsFilter
  },
  methods: {
    searchAlbums() {
      
    }
  }

}
</script>

<style lang="scss">
@import "@/styles/app";
</style>
