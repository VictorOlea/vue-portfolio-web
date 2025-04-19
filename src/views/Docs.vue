<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
    >
      <a
        href="/CV-Víctor-Olea-Ingeniero-Mecatrónico.pdf"
        target="_blank"
        rel="noopener noreferrer"
        :class="documentStyle['document-link']"
      >
        <section :class="documentStyle['document-card']">
          <div :class="documentStyle['document-icon']">
            <img src="../assets/cv.svg" alt="CV Icon" width="50" height="50" />
          </div>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><a
        href="https://www.linkedin.com/in/victor-olea/"
        target="_blank"
        rel="noopener noreferrer"
        :class="documentStyle['docuement-link']"
      >
        <section :class="documentStyle['document-card']">
          <div :class="documentStyle['document-icon']">
            <img
              src="../assets/linkedin.svg"
              alt="Linkedin Icon"
              width="100"
              height="100"
            />
          </div>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><a
        href="https://github.com/VictorOlea"
        target="_blank"
        rel="noopener noreferrer"
        :class="documentStyle['document-link']"
      >
        <section :class="documentStyle['document-card']">
          <div :class="documentStyle['document-icon']">
            <img
              src="../assets/github.svg"
              alt="Github Icon"
              width="70"
              height="70"
            />
          </div>
        </section>
      </a>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><a
        href="https://portfolio-victor-olea.netlify.app/"
        target="_blank"
        rel="noopener noreferrer"
        :class="documentStyle['document-link']"
      >
        <section :class="documentStyle['document-card']">
          <h2 :class="documentStyle['document-title']">Old Portfolio</h2>
        </section>
      </a>
    </BentoCard>
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoGrid from "../components/BentoGrid.vue";
import BentoCard from "../components/BentoCard.vue";
import documentStyle from "../styles/document.module.css";
</script>
