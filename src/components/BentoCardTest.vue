<template>
  <div class="bento-card" :style="gridStyles">
    <slot />
  </div>
</template>

<script setup lang="ts">
import { computed, onMounted, onBeforeUnmount, ref } from "vue";

interface ResponsiveSpan {
  col: number;
  row: number;
}

const props = defineProps<{
  responsiveSpan: {
    desktop: ResponsiveSpan;
    tablet: ResponsiveSpan;
    mobile: ResponsiveSpan;
  };
}>();

const currentSize = ref<"desktop" | "tablet" | "mobile">("desktop");

const updateScreenSize = () => {
  const width = window.innerWidth;
  if (width <= 480) {
    currentSize.value = "mobile";
  } else if (width <= 768) {
    currentSize.value = "tablet";
  } else {
    currentSize.value = "desktop";
  }
};

const gridStyles = computed(() => {
  const span = props.responsiveSpan[currentSize.value];
  return {
    gridColumn: `span ${span.col}`,
    gridRow: `span ${span.row}`,
  };
});

onMounted(() => {
  updateScreenSize();
  window.addEventListener("resize", updateScreenSize);
});

onBeforeUnmount(() => {
  window.removeEventListener("resize", updateScreenSize);
});
</script>

<style scoped>
.bento-card {
  width: 100%;
  height: 100%;
}
</style>
