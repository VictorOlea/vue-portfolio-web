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

/* @media (max-width: 1024px) {
  .grid {
    grid-template-columns: repeat(4, 1fr);
  }
} */

@media (max-width: 768px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 480px) {
  .grid {
    grid-template-columns: 1fr;
  }
}
</style>
