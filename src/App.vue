<script setup lang="ts">
import Counter from "./components/Counter.vue";
</script>

<template>
  <div class="body"><Counter /></div>
</template>

<style scoped>
.body {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: #e8f2fe;
}
</style>
