<template>
  <div class="container">
    <select class="form-select" v-model="selected" @change="$emit('search', selected)">
        <option disabled value="">Seleziona un genere preferito</option>
            <option>Rock</option>
            <option>Metal</option>
            <option>Pop</option>
    </select>
  </div>
</template>

<script>
export default {
    name: "AlbumsFilter",
    data() {
        return {
        selected: ''
        }
  }
}
</script>

<style>

</style>