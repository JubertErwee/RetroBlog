<script setup lang="ts">
const version = 2 + 1
</script>

<template>
  <div class="hello">
    Hello Nuxt {{ version }}!
  </div>
  <li><nuxt-link to="/about" class="btn">About</nuxt-link></li>
</template>

<style scoped>
.hello {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 3rem;
  padding: 2rem;
}
</style>
