<script setup lang="ts">
const name = "商品名";
const price = 1000;
const link = "https://google.com";
</script>

<template>
  <a :href="link" target="_blank">
    <p>{{ name }}</p>
    <p>{{ price }}円</p>
  </a>
</template>

<style scoped>
a {
  display: flex;
  border-radius: 8px;
  justify-content: space-between;
  text-decoration: none;
  color: white;
  background-color: #1a1a1a;
  padding: 10px 20px;
}
</style>
