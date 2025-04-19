<script setup lang="ts">
const experience = [
  {
    title: "Desarrollador Frontend – Proyecto Personal",
    period: "2023 – Actualidad",
    description: `Desarrollo de aplicaciones SPA usando Vue 3, composición modular de componentes,
    integración con APIs externas y diseño responsive usando CSS puro y Tailwind.`,
  },
  {
    title: "Docente de Tecnología – Taller Comunitario",
    period: "2022 – 2023",
    description: `Enseñanza de herramientas digitales básicas, introducción a la programación con Arduino
    y trabajo colaborativo con jóvenes y adultos en espacios comunitarios.`,
  },
];
</script>

<template>
  <section class="bento-card">
    <h2 class="section-title">Experiencia Laboral</h2>

    <div v-for="(job, index) in experience" :key="index" class="job">
      <h3 class="job-title">{{ job.title }}</h3>
      <p class="job-period">{{ job.period }}</p>
      <p class="job-description">{{ job.description }}</p>
    </div>
  </section>
</template>

<style scoped>
.section-title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 1rem;
}

.job {
  margin-bottom: 1.5rem;
}

.job-title {
  font-size: 1.125rem;
  font-weight: 600;
  margin-bottom: 0.25rem;
}

.job-period {
  font-size: 0.9rem;
  color: #666;
  margin-bottom: 0.5rem;
}

.job-description {
  font-size: 1rem;
  line-height: 1.5;
}
</style>
