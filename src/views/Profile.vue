<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 3 },
      }"
    >
      <div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/avatar-profile.png"
        />
      </div>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 3 },
      }"
    >
      <div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/avatar-profile.png"
        />
      </div>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 3 },
        tablet: { col: 4, row: 3 },
        mobile: { col: 4, row: 4 },
      }"
      ><section :class="sectionStyle['section-card']">
        <p :class="sectionStyle['section-content-strong']">
          Ingeniero Civil Mecatrónico, he adquirido una sólida formación que
          combina aspectos de la ingeniería mecánica, electrónica y de control,
          con enfoque en sistemas de automatización industrial junto con el
          armado y mantenimiento de maquinaria.
          <br /><br />
          Soy una persona apasionada por la tecnología, motivada con adquirir
          nuevos conocimientos y en la búsqueda de desarrollarme
          profesionalmente. Mis intereses están en el sector industrial,
          mantenimiento, automatización y robótica.
        </p>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 4, row: 4 },
        tablet: { col: 4, row: 4 },
        mobile: { col: 4, row: 3 },
      }"
      ><section :class="experienceStyle['section-card']">
        <h2 :class="experienceStyle['section-title']">Experiencia Laboral</h2>
        <div :class="experienceStyle['job-wrapper']">
          <div
            v-for="(job, index) in experience"
            :key="index"
            :class="experienceStyle['job']"
          >
            <div :class="experienceStyle['job-header']">
              <h3 :class="experienceStyle['job-title']">{{ job.title }}</h3>
              <p :class="experienceStyle['job-period']">{{ job.period }}</p>
            </div>
            <ul :class="experienceStyle['job-description']">
              <li v-for="(item, i) in job.description" :key="i">{{ item }}</li>
            </ul>
          </div>
        </div>
      </section>
    </BentoCard>
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoCard from "../components/BentoCard.vue";
import BentoGrid from "../components/BentoGrid.vue";
import imageStyle from "../styles/image.module.css";
import sectionStyle from "../styles/section.module.css";
import experienceStyle from "../styles/experience.module.css";

const experience = [
  {
    title: "MOV Design - Personal Científico Tecnológico",
    period: "Agosto 2024 - Enero 2025",
    description: [
      "Diseño y desarrollo de placas PCB para productos tecnológicos.",
      "Programación de microcontroladores.",
      "Armado de productos electrónicos.",
    ],
  },
  {
    title: "Servicio Técnico Independiente",
    period: "Enero 2023 - Abril 2024",
    description: [
      "Diseño y desarrollo de robots educativos, integrando módulos electrónicos e impresión 3D, junto con programación de microcontroladores.",
      "Fabricación, configuración y mantenimiento de equipos electrónicos, electromecánicos y agroindustriales a medida.",
      "Asesoría técnica en procesos industriales y soporte en instalaciones especializadas.",
    ],
  },
];
</script>

<style module>
.img-card {
  border: 2px solid grey;
  border-radius: 10px;
  height: 100%;
  object-fit: cover;
  width: 100%;
}

.title-card {
  align-self: center;
  font-size: clamp(1.8rem, 4vw, 2.4rem);
  height: 100%;
  margin-bottom: auto;
  margin-top: auto;
  padding: 8px;
  text-align: center;
  width: 100%;
}
</style>
