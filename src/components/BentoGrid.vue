<template>
  <div class="grid">
    <slot />
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.grid {
  display: grid;
  width: 100%;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 100px;
  gap: 10px;
}
</style>
