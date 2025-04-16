<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 1, row: 3 },
        mobile: { col: 1, row: 3 },
      }"
    >
      <div :class="imageStyle['img-wrapper']">
        <img :class="imageStyle['img-card']" src="../assets/profile.jpg" />
      </div>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-2</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 3 },
        tablet: { col: 2, row: 4 },
        mobile: { col: 4, row: 3 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-3</h2>
      </section>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 3 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-4</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 1 },
        tablet: { col: 4, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-5</h2>
      </section></BentoCard
    >
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoCard from "../components/BentoCard.vue";
import BentoGrid from "../components/BentoGrid.vue";
import imageStyle from "../styles/image.module.css";
import sectionStyle from "../styles/section.module.css";
</script>

<style module>
.img-card {
  width: 100%;
  height: 100%;
  border: 2px solid grey;
  border-radius: 10px;
  object-fit: cover;
}

.title-card {
  font-size: clamp(1.8rem, 4vw, 2.4rem);
  width: 100%;
  height: 100%;
  text-align: center;
  align-self: center;
  padding: 8px;
  margin-top: auto;
  margin-bottom: auto;
}
</style>
