<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
const countUp = () => count.value++;
const reset = () => (count.value = 0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="countUp">count is {{ count }}</button>
    <button type="button" @click="reset">reset</button>
  </div>
</template>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
</style>
