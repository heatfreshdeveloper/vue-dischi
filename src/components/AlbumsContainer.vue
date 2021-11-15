<template>
  <div class="row row-cols-1 row-cols-md-4 g-4">
      <div class="col" v-for="albums in albumsList" :key="albums.id">
        <albums
          :poster="albums.poster"
          :title="albums.title"
          :author="albums.author"
          :year="albums.year"
        ></albums>
      </div>
    </div>
</template>

<script>
import axios from "axios";
import Albums from './Albums.vue';


export default {
  name: "AlbumsContainer",
  components: { Albums },
  data() {
        return {
        albumsList: []
        }
  },
  methods: {
      mounted() {
          axios.get("https://flynn.boolean.careers/exercises/api/array/music").then(resp => {
              this.albumsList = resp.data.response;
          })
      }
  }
}
</script>

<style>

</style>