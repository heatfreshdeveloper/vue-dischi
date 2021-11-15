<template>
  <div class="card">
    <img class="card-img-top" :src="poster" alt="..." />
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <div class="card-text">
        <ul>
          <li>{{ author }}</li>
          <li>{{ year }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Albums",
  props: ["poster", "title", "author", "year"],
};
</script>